# Comparing `tmp/openbb_nightly-4.1.7.dev202405070009.tar.gz` & `tmp/openbb_nightly-4.1.7.dev202405080008.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.7.dev202405070009.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.7.dev202405080008.tar", max compression
```

## Comparing `openbb_nightly-4.1.7.dev202405070009.tar` & `openbb_nightly-4.1.7.dev202405080008.tar`

### file list

```diff
@@ -1,792 +1,791 @@
--rw-r--r--   0        0        0     6818 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/README.md
--rw-r--r--   0        0        0       19 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7189 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    18672 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-05-07 00:09:32.044285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1908 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/api_settings.py
--rw-r--r--   0        0        0     1035 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3875 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      502 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1054 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/field.py
--rw-r--r--   0        0        0      694 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      474 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     5669 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9094 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1477 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0      801 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/python_settings.py
--rw-r--r--   0        0        0       37 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     4044 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    21268 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    23086 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10402 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3511 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7595 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1948 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    65939 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2224 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     8142 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0     1377 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/available_indicators.py
--rw-r--r--   0        0        0      630 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-05-07 00:09:32.048285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1246 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     3722 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/country_profile.py
--rw-r--r--   0        0        0     1591 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1886 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/economic_indicators.py
--rw-r--r--   0        0        0     1750 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      912 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      939 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-05-07 00:09:32.052285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3083 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3474 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9699 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.056285 openbb_nightly-4.1.7.dev202405070009/core/openbb_core/py.typed
--rw-r--r--   0        0        0       34 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0       31 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3848 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.060285 openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0       37 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0       32 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0    11799 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-05-07 00:09:32.064285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.068285 openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0       29 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0       35 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16738 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    19706 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/relative_rotation.py
--rw-r--r--   0        0        0    64220 2024-05-07 00:09:32.072285 openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0    19798 2024-05-07 00:09:32.076285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-05-07 00:09:32.076285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    40926 2024-05-07 00:09:32.076285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-05-07 00:09:32.076285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-05-07 00:09:32.076285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     8068 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58532 2024-05-07 00:09:32.092285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228579 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12381 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0       25 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
--rw-r--r--   0        0        0     8555 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    19572 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3300 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5697 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6877 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3547 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    25006 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-05-07 00:09:32.116285 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0    26843 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0       32 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/__init__.py
--rw-r--r--   0        0        0      603 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/colors.py
--rw-r--r--   0        0        0     3462 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0     3491 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0    20295 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
--rw-r--r--   0        0        0     2493 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0    16657 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
--rw-r--r--   0        0        0     1440 2024-05-07 00:09:32.120286 openbb_nightly-4.1.7.dev202405070009/openbb/__init__.py
--rw-r--r--   0        0        0  1214504 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/assets/reference.json
--rw-r--r--   0        0        0     2813 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/__extensions__.py
--rw-r--r--   0        0        0       50 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/__init__.py
--rw-r--r--   0        0        0     3299 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/crypto.py
--rw-r--r--   0        0        0     6468 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    13823 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/currency.py
--rw-r--r--   0        0        0     6360 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12047 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    65529 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/economy.py
--rw-r--r--   0        0        0    12355 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27558 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity.py
--rw-r--r--   0        0        0    18353 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2807 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    25823 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    40717 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   163982 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30431 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26606 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3710 2024-05-07 00:09:32.124286 openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    75407 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/etf.py
--rw-r--r--   0        0        0     4538 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    19470 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7001 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26229 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    10857 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11744 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/index.py
--rw-r--r--   0        0        0    15304 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/regulators.py
--rw-r--r--   0        0        0    16379 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/package/regulators_sec.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12452 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    17979 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9801 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-05-07 00:09:32.128286 openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-05-07 00:09:32.132286 openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-05-07 00:09:32.140286 openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      805 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/__init__.py
--rw-r--r--   0        0        0       21 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/available_indicators.py
--rw-r--r--   0        0        0    12504 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/country_profile.py
--rw-r--r--   0        0        0    18643 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/economic_indicators.py
--rw-r--r--   0        0        0       24 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/__init__.py
--rw-r--r--   0        0        0    22209 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/helpers.py
--rw-r--r--   0        0        0    24368 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/indicator_countries.json
--rw-r--r--   0        0        0     5244 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
--rw-r--r--   0        0        0    66758 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/multipliers.json
--rw-r--r--   0        0        0    87109 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/scales.json
--rw-r--r--   0        0        0    73815 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
--rw-r--r--   0        0        0    90624 2024-05-07 00:09:32.188286 openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/units.json
--rw-r--r--   0        0        0      716 2024-05-07 00:09:32.192286 openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-05-07 00:09:32.192286 openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-05-07 00:09:32.192286 openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-05-07 00:09:32.192286 openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-05-07 00:09:32.200286 openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-05-07 00:09:32.200286 openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-05-07 00:09:32.200286 openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-05-07 00:09:32.200286 openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-05-07 00:09:32.200286 openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9573 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.256287 openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8255 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6076 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5308 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6768 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3607 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-05-07 00:09:32.260287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2270 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10603 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3938 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     6297 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3521 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.264287 openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6656 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-05-07 00:09:32.284287 openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-05-07 00:09:32.288287 openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-05-07 00:09:32.288287 openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-05-07 00:09:32.288287 openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5269 2024-05-07 00:09:32.288287 openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-05-07 00:09:32.288287 openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-05-07 00:09:32.288287 openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5393 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22763 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     9061 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     9071 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2376 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7327 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8417 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9694 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5090 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3357 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8901 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6513 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     8655 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-05-07 00:09:32.292287 openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6330 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5157 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-05-07 00:09:32.300287 openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2247 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     6961 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6283 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6255 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6125 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     9753 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/currency_snapshots.py
--rw-r--r--   0        0        0     7150 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     6142 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3734 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.308287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-05-07 00:09:32.312287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-05-07 00:09:32.312287 openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1658 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0    10150 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     3154 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2681 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    39078 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2766 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2051 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2900 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3498 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1796 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    12574 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7587 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.328287 openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-05-07 00:09:32.416288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-07 00:09:32.420288 openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6302 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5162 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4647 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8843 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5455 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12451 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5085 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8409 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9651 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-05-07 00:09:32.428288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10325 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5986 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5133 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-05-07 00:09:32.432288 openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6582 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9222 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10325 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-05-07 00:09:32.528289 openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-05-07 00:09:32.532289 openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     5122 2024-05-07 00:09:32.532289 openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-05-07 00:09:32.532289 openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-05-07 00:09:32.532289 openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4144 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     2036 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5858 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10102 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10144 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6017 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-05-07 00:09:32.536289 openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     7005 2024-05-07 00:09:41.060372 openbb_nightly-4.1.7.dev202405070009/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202405070009/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-05-08 00:08:32.549458 openbb_nightly-4.1.7.dev202405080008/README.md
+-rw-r--r--   0        0        0       19 2024-05-08 00:08:32.549458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    18672 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1908 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9094 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21268 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23086 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10402 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7595 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1948 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    65939 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2224 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-05-08 00:08:32.553458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2581 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8142 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0     1377 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/available_indicators.py
+-rw-r--r--   0        0        0      630 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1246 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     3722 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/country_profile.py
+-rw-r--r--   0        0        0     1591 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      423 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1680 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/economic_indicators.py
+-rw-r--r--   0        0        0     1750 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      912 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-05-08 00:08:32.557458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3073 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3474 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9699 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.561458 openbb_nightly-4.1.7.dev202405080008/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-05-08 00:08:32.565458 openbb_nightly-4.1.7.dev202405080008/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-08 00:08:32.565458 openbb_nightly-4.1.7.dev202405080008/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3848 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-05-08 00:08:32.569458 openbb_nightly-4.1.7.dev202405080008/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0    12007 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-08 00:08:32.573458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-05-08 00:08:32.577458 openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    63911 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0    21550 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    40926 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-05-08 00:08:32.581458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58532 2024-05-08 00:08:32.601458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228579 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-05-08 00:08:32.621458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    25006 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    26843 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3491 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20295 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0    16657 2024-05-08 00:08:32.625458 openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
+-rw-r--r--   0        0        0     1440 2024-05-08 00:08:32.629458 openbb_nightly-4.1.7.dev202405080008/openbb/__init__.py
+-rw-r--r--   0        0        0  1227796 2024-05-08 00:08:32.629458 openbb_nightly-4.1.7.dev202405080008/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2813 2024-05-08 00:08:32.629458 openbb_nightly-4.1.7.dev202405080008/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0     3299 2024-05-08 00:08:32.629458 openbb_nightly-4.1.7.dev202405080008/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6468 2024-05-08 00:08:32.629458 openbb_nightly-4.1.7.dev202405080008/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    13823 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/currency.py
+-rw-r--r--   0        0        0     6360 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12047 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    65869 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/economy.py
+-rw-r--r--   0        0        0    12355 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27558 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity.py
+-rw-r--r--   0        0        0    18353 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2807 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    25823 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    40717 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   163990 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30431 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26606 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3710 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75407 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/etf.py
+-rw-r--r--   0        0        0     4538 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    19470 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7001 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26229 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    10857 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11744 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/index.py
+-rw-r--r--   0        0        0    20588 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/package/regulators.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12452 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-05-08 00:08:32.633458 openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    17979 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9801 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-05-08 00:08:32.637458 openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4831 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     7796 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-05-08 00:08:32.641458 openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-05-08 00:08:32.645458 openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      805 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/available_indicators.py
+-rw-r--r--   0        0        0    12504 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/country_profile.py
+-rw-r--r--   0        0        0    20324 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/economic_indicators.py
+-rw-r--r--   0        0        0       24 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/__init__.py
+-rw-r--r--   0        0        0    22209 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/helpers.py
+-rw-r--r--   0        0        0    24368 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/indicator_countries.json
+-rw-r--r--   0        0        0     5244 2024-05-08 00:08:32.693459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
+-rw-r--r--   0        0        0     8156 2024-05-08 00:08:32.697459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/main_indicators.py
+-rw-r--r--   0        0        0    66758 2024-05-08 00:08:32.697459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/multipliers.json
+-rw-r--r--   0        0        0    87109 2024-05-08 00:08:32.697459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/scales.json
+-rw-r--r--   0        0        0    73815 2024-05-08 00:08:32.697459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
+-rw-r--r--   0        0        0    90624 2024-05-08 00:08:32.697459 openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/units.json
+-rw-r--r--   0        0        0      716 2024-05-08 00:08:32.701459 openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-05-08 00:08:32.701459 openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-05-08 00:08:32.701459 openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-05-08 00:08:32.701459 openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-05-08 00:08:32.705459 openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-05-08 00:08:32.705459 openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-05-08 00:08:32.705459 openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-05-08 00:08:32.705459 openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-05-08 00:08:32.705459 openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9573 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.765459 openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8255 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3068 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2955 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5909 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5904 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     2272 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6076 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5918 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6102 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5308 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6493 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3446 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3144 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6768 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3607 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4286 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5050 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5826 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10603 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3521 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4220 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3270 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-05-08 00:08:32.769459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-05-08 00:08:32.773459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.773459 openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6344 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6720 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-05-08 00:08:32.793460 openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-05-08 00:08:32.797459 openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-08 00:08:32.797459 openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-05-08 00:08:32.797459 openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5138 2024-05-08 00:08:32.797459 openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-05-08 00:08:32.797459 openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-08 00:08:32.797459 openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5393 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22763 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     9061 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2211 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     9071 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2376 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4974 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7327 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29027 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8337 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8417 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9694 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5090 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3676 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12539 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3357 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6513 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     8655 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-05-08 00:08:32.801459 openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5157 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-05-08 00:08:32.809460 openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2247 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     7039 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4600 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6283 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6255 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     6204 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     9753 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/currency_snapshots.py
+-rw-r--r--   0        0        0     7150 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6142 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-05-08 00:08:32.817460 openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-05-08 00:08:32.833460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0    10150 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     3154 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2681 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    39078 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2820 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2051 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2916 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3498 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1796 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    12574 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7587 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.837460 openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-05-08 00:08:32.925460 openbb_nightly-4.1.7.dev202405080008/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-08 00:08:32.929460 openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6302 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5162 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4647 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8843 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5455 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12451 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-05-08 00:08:32.937461 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3638 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5085 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8409 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9651 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10329 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5986 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5132 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-05-08 00:08:32.941460 openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6582 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9222 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-08 00:08:33.041461 openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     5122 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4144 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2863 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3450 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3361 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6671 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5858 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3890 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10102 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4711 2024-05-08 00:08:33.045461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4063 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10144 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4646 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4230 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6017 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-05-08 00:08:33.049461 openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     7021 2024-05-08 00:08:41.781528 openbb_nightly-4.1.7.dev202405080008/pyproject.toml
+-rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202405080008/PKG-INFO
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/README.md` & `openbb_nightly-4.1.7.dev202405080008/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/command_runner.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/abstract/singleton.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/api_settings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/field.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/field.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     )
     plot_enable_pywry: bool = True
     plot_open_export: bool = (
         False  # Whether to open plot image exports after they are created
     )
     plot_pywry_height: PositiveInt = 762
     plot_pywry_width: PositiveInt = 1400
-    request_timeout: PositiveInt = 15
+    request_timeout: PositiveInt = 60
     show_warnings: bool = True
     table_style: Literal["dark", "light"] = "dark"
     user_styles_directory: str = str(Path.home() / "OpenBBUserData" / "styles" / "user")
 
     model_config = ConfigDict(validate_assignment=True)
 
     def __repr__(self) -> str:
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/profile.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/python_settings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/python_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/query.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/router.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/package_builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/app/version.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/env.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/available_indicators.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/country_profile.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-"""Economic Indicators Standard Model."""
+"""Historical Attributes Standard Model."""
 
 from datetime import date as dateType
-from typing import Optional, Union
+from typing import List, Literal, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class EconomicIndicatorsQueryParams(QueryParams):
-    """Economic Indicators Query."""
+class HistoricalAttributesQueryParams(QueryParams):
+    """Historical Attributes Query."""
 
-    symbol: str = Field(
-        description=QUERY_DESCRIPTIONS.get("symbol", "")
-        + " The base symbol for the indicator (e.g. GDP, CPI, etc.).",
-    )
-    country: Optional[str] = Field(
-        default=None,
-        description=QUERY_DESCRIPTIONS.get("country", "")
-        + " The country represented by the indicator, if available.",
-    )
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
+    tag: str = Field(description="Intrinio data tag ID or code.")
     start_date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("start_date", ""), default=None
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
     )
     end_date: Optional[dateType] = Field(
-        description=QUERY_DESCRIPTIONS.get("end_date", ""), default=None
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
+    )
+    frequency: Optional[
+        Literal["daily", "weekly", "monthly", "quarterly", "yearly"]
+    ] = Field(default="yearly", description=QUERY_DESCRIPTIONS.get("frequency"))
+    limit: Optional[int] = Field(
+        default=1000, description=QUERY_DESCRIPTIONS.get("limit")
+    )
+    tag_type: Optional[str] = Field(
+        default=None, description="Filter by type, when applicable."
     )
+    sort: Optional[Literal["asc", "desc"]] = Field(
+        default="desc", description="Sort order."
+    )
+
+    @field_validator("tag", mode="before", check_fields=False)
+    @classmethod
+    def multiple_tags(cls, v: Union[str, List[str], Set[str]]):
+        """Accept a comma-separated string or list of tags."""
+        if isinstance(v, str):
+            return v.lower()
+        return ",".join([tag.lower() for tag in list(v)])
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def to_upper(cls, v: str) -> str:
         """Convert field to uppercase."""
         return v.upper()
 
+    @field_validator("frequency", "sort", mode="before", check_fields=False)
+    @classmethod
+    def to_lower(cls, v: Optional[str]) -> Optional[str]:
+        """Convert field to lowercase."""
+        return v.lower() if v else v
 
-class EconomicIndicatorsData(Data):
-    """Economic Indicators Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    symbol_root: Optional[str] = Field(
-        default=None, description="The root symbol for the indicator (e.g. GDP)."
-    )
-    symbol: Optional[str] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("symbol", "")
-    )
-    country: Optional[str] = Field(
-        default=None, description="The country represented by the data."
-    )
-    value: Optional[Union[int, float]] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("value", "")
+class HistoricalAttributesData(Data):
+    """Historical Attributes Data."""
+
+    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date"))
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol"))
+    tag: Optional[str] = Field(
+        default=None, description="Tag name for the fetched data."
     )
+    value: Optional[float] = Field(default=None, description="The value of the data.")
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,54 @@
-"""Historical Attributes Standard Model."""
+"""Revenue by Geographic Segments Standard Model."""
 
 from datetime import date as dateType
-from typing import List, Literal, Optional, Set, Union
+from typing import Dict, Literal, Optional
 
 from pydantic import Field, field_validator
 
-from openbb_core.provider.abstract.data import Data
+from openbb_core.provider.abstract.data import Data, ForceInt
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
-    DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class HistoricalAttributesQueryParams(QueryParams):
-    """Historical Attributes Query."""
+class RevenueGeographicQueryParams(QueryParams):
+    """Revenue by Geographic Segments Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol"))
-    tag: str = Field(description="Intrinio data tag ID or code.")
-    start_date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("start_date")
-    )
-    end_date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("end_date")
-    )
-    frequency: Optional[
-        Literal["daily", "weekly", "monthly", "quarterly", "yearly"]
-    ] = Field(default="yearly", description=QUERY_DESCRIPTIONS.get("frequency"))
-    limit: Optional[int] = Field(
-        default=1000, description=QUERY_DESCRIPTIONS.get("limit")
-    )
-    tag_type: Optional[str] = Field(
-        default=None, description="Filter by type, when applicable."
-    )
-    sort: Optional[Literal["asc", "desc"]] = Field(
-        default="desc", description="Sort order."
-    )
-
-    @field_validator("tag", mode="before", check_fields=False)
-    @classmethod
-    def multiple_tags(cls, v: Union[str, List[str], Set[str]]):
-        """Accept a comma-separated string or list of tags."""
-        if isinstance(v, str):
-            return v.lower()
-        return ",".join([tag.lower() for tag in list(v)])
+    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    period: Literal["quarter", "annual"] = Field(
+        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
+    )
+    structure: Literal["hierarchical", "flat"] = Field(
+        default="flat", description="Structure of the returned data."
+    )  # should always be flat
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def to_upper(cls, v: str) -> str:
+    def to_upper(cls, v: str):
         """Convert field to uppercase."""
         return v.upper()
 
-    @field_validator("frequency", "sort", mode="before", check_fields=False)
+    @field_validator("period", "structure", mode="before", check_fields=False)
     @classmethod
     def to_lower(cls, v: Optional[str]) -> Optional[str]:
         """Convert field to lowercase."""
         return v.lower() if v else v
 
 
-class HistoricalAttributesData(Data):
-    """Historical Attributes Data."""
+class RevenueGeographicData(Data):
+    """Revenue by Geographic Segments Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date"))
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol"))
-    tag: Optional[str] = Field(
-        default=None, description="Tag name for the fetched data."
+    period_ending: dateType = Field(description="The end date of the reporting period.")
+    fiscal_period: Optional[str] = Field(
+        default=None, description="The fiscal period of the reporting period."
+    )
+    fiscal_year: Optional[int] = Field(
+        default=None, description="The fiscal year of the reporting period."
+    )
+    filing_date: Optional[dateType] = Field(
+        default=None, description="The filing date of the report."
+    )
+    geographic_segment: Dict[str, ForceInt] = Field(
+        description="Dictionary of the revenue by geographic segment."
     )
-    value: Optional[float] = Field(default=None, description="The value of the data.")
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/options_chains.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 class OptionsChainsQueryParams(QueryParams):
     """Options Chains Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
 
-    @classmethod
     @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
     def to_upper(cls, v: str) -> str:
         """Return the symbol in uppercase."""
         return v.upper()
 
 
 class OptionsChainsData(Data):
     """Options Chains Data."""
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-"""Revenue by Geographic Segments Standard Model."""
+"""Share Statistics Standard Model."""
 
 from datetime import date as dateType
-from typing import Dict, Literal, Optional
+from typing import List, Optional, Set, Union
 
 from pydantic import Field, field_validator
 
-from openbb_core.provider.abstract.data import Data, ForceInt
+from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
+    DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class RevenueGeographicQueryParams(QueryParams):
-    """Revenue by Geographic Segments Query."""
+class ShareStatisticsQueryParams(QueryParams):
+    """Share Statistics Query."""
 
     symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
-    period: Literal["quarter", "annual"] = Field(
-        default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
-    )
-    structure: Literal["hierarchical", "flat"] = Field(
-        default="flat", description="Structure of the returned data."
-    )  # should always be flat
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
-    def to_upper(cls, v: str):
+    def to_upper(cls, v: str) -> str:
         """Convert field to uppercase."""
         return v.upper()
 
-    @field_validator("period", "structure", mode="before", check_fields=False)
-    @classmethod
-    def to_lower(cls, v: Optional[str]) -> Optional[str]:
-        """Convert field to lowercase."""
-        return v.lower() if v else v
-
 
-class RevenueGeographicData(Data):
-    """Revenue by Geographic Segments Data."""
+class ShareStatisticsData(Data):
+    """Share Statistics Data."""
 
-    period_ending: dateType = Field(description="The end date of the reporting period.")
-    fiscal_period: Optional[str] = Field(
-        default=None, description="The fiscal period of the reporting period."
+    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
+    date: Optional[dateType] = Field(
+        default=None, description=DATA_DESCRIPTIONS.get("date", "")
+    )
+    free_float: Optional[float] = Field(
+        default=None,
+        description="Percentage of unrestricted shares of a publicly-traded company.",
     )
-    fiscal_year: Optional[int] = Field(
-        default=None, description="The fiscal year of the reporting period."
+    float_shares: Optional[float] = Field(
+        default=None,
+        description="Number of shares available for trading by the general public.",
     )
-    filing_date: Optional[dateType] = Field(
-        default=None, description="The filing date of the report."
+    outstanding_shares: Optional[float] = Field(
+        default=None, description="Total number of shares of a publicly-traded company."
     )
-    geographic_segment: Dict[str, ForceInt] = Field(
-        description="Dictionary of the revenue by geographic segment."
+    source: Optional[str] = Field(
+        default=None, description="Source of the received data."
     )
+
+    @field_validator("symbol", mode="before", check_fields=False)
+    @classmethod
+    def to_upper(cls, v: Union[str, List[str], Set[str]]):
+        """Convert field to uppercase."""
+        if isinstance(v, str):
+            return v.upper()
+        return ",".join([symbol.upper() for symbol in list(v)])
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/world_news.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,65 @@
-"""Share Statistics Standard Model."""
+"""World News Standard Model."""
 
-from datetime import date as dateType
-from typing import List, Optional, Set, Union
+from datetime import (
+    date as dateType,
+    datetime,
+)
+from typing import Dict, List, Optional
 
-from pydantic import Field, field_validator
+from dateutil.relativedelta import relativedelta
+from pydantic import Field, NonNegativeInt, field_validator
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.abstract.query_params import QueryParams
 from openbb_core.provider.utils.descriptions import (
     DATA_DESCRIPTIONS,
     QUERY_DESCRIPTIONS,
 )
 
 
-class ShareStatisticsQueryParams(QueryParams):
-    """Share Statistics Query."""
+class WorldNewsQueryParams(QueryParams):
+    """World News Query."""
 
-    symbol: str = Field(description=QUERY_DESCRIPTIONS.get("symbol", ""))
+    limit: NonNegativeInt = Field(
+        default=2500,
+        description=QUERY_DESCRIPTIONS.get("limit", "")
+        + " The number of articles to return.",
+    )
+    start_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("start_date", "")
+    )
+    end_date: Optional[dateType] = Field(
+        default=None, description=QUERY_DESCRIPTIONS.get("end_date", "")
+    )
 
-    @field_validator("symbol", mode="before", check_fields=False)
+    @field_validator("start_date", mode="before")
     @classmethod
-    def to_upper(cls, v: str) -> str:
-        """Convert field to uppercase."""
-        return v.upper()
+    def start_date_validate(cls, v) -> dateType:  # pylint: disable=E0213
+        """Populate start date if empty."""
+        if not v:
+            now = datetime.now().date()
+            v = now - relativedelta(weeks=2)
+        return v
 
+    @field_validator("end_date", mode="before")
+    @classmethod
+    def end_date_validate(cls, v) -> dateType:  # pylint: disable=E0213
+        """Populate end date if empty."""
+        if not v:
+            v = datetime.now().date()
+        return v
 
-class ShareStatisticsData(Data):
-    """Share Statistics Data."""
 
-    symbol: str = Field(description=DATA_DESCRIPTIONS.get("symbol", ""))
-    date: Optional[dateType] = Field(
-        default=None, description=DATA_DESCRIPTIONS.get("date", "")
+class WorldNewsData(Data):
+    """World News Data."""
+
+    date: datetime = Field(
+        description=DATA_DESCRIPTIONS.get("date", "")
+        + " The published date of the article."
     )
-    free_float: Optional[float] = Field(
-        default=None,
-        description="Percentage of unrestricted shares of a publicly-traded company.",
+    title: str = Field(description="Title of the article.")
+    images: Optional[List[Dict[str, str]]] = Field(
+        default=None, description="Images associated with the article."
     )
-    float_shares: Optional[float] = Field(
-        default=None,
-        description="Number of shares available for trading by the general public.",
-    )
-    outstanding_shares: Optional[float] = Field(
-        default=None, description="Total number of shares of a publicly-traded company."
-    )
-    source: Optional[str] = Field(
-        default=None, description="Source of the received data."
-    )
-
-    @field_validator("symbol", mode="before", check_fields=False)
-    @classmethod
-    def to_upper(cls, v: Union[str, List[str], Set[str]]):
-        """Convert field to uppercase."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
+    text: Optional[str] = Field(default=None, description="Text/body of the article.")
+    url: Optional[str] = Field(default=None, description="URL to the article.")
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class TreasuryPricesQueryParams(QueryParams):
     """Treasury Prices Query."""
 
     date: Optional[dateType] = Field(
         description=QUERY_DESCRIPTIONS.get("date", "")
-        + " No date will return the current posted data.",
+        + " Defaults to the last business day.",
         default=None,
     )
 
 
 class TreasuryPricesData(Data):
     """Treasury Prices Data."""
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/core/openbb_core/provider/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/economy/openbb_economy/economy_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,14 +358,18 @@
             + " Use `available_indicators()` to get a list of supported indicators from EconDB.",
             parameters={
                 "symbol": "CPI",
                 "country": "united_states,jp",
                 "provider": "econdb",
             },
         ),
+        APIEx(
+            description="Use the `main` symbol to get the group of main indicators for a country.",
+            parameters={"provider": "econdb", "symbol": "main", "country": "eu"},
+        ),
     ],
 )
 async def indicators(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/relative_rotation.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.7.dev202405080008/extensions/technical/openbb_technical/technical_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,19 +53,14 @@
             code=[
                 "crypto_data = obb.crypto.price.historical("
                 + " symbol='BTCUSD,ETHUSD,SOLUSD', start_date='2021-01-01', provider='yfinance')",
                 "rr_data = obb.technical.relative_rotation(data=crypto_data.results, benchmark='BTCUSD',"
                 + " long_period=365, short_period=30, window=30, trading_periods=365)",
             ],
         ),
-        APIEx(
-            description="Note that the mock data displayed here is insufficient."
-            + " It must contain multiple symbols, with the benchmark, and be daily data at least 1 year in length.",
-            parameters={"benchmark": "SPY", "data": APIEx.mock_data("timeseries")},
-        ),
     ],
 )
 async def relative_rotation(
     data: List[Data],
     benchmark: str,
     study: Literal["price", "volume", "volatility"] = "price",
     long_period: Optional[int] = 252,
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         Return the list of the available technical indicators to use with the `to_chart` method and OHLC+V data.
     table
         Display an interactive table.
     create_line_chart
         Create a line chart from external data.
     create_bar_chart
         Create a bar chart, on a single x-axis with one or more values for the y-axis, from external data.
+    toggle_chart_style
+        Toggle the chart style, of an existing chart, between light and dark mode.
     """
 
     def __init__(self, obbject):
         """Initialize Charting extension."""
         # pylint: disable=import-outside-toplevel
         from openbb_core.app.model.charts.charting_settings import ChartingSettings
 
@@ -230,14 +232,15 @@
             layout_kwargs=layout_kwargs,
             scatter_kwargs=scatter_kwargs,
             normalize=normalize,
             returns=returns,
             same_axis=same_axis,
             **kwargs,
         )
+        fig = self._set_chart_style(fig)
         if render:
             return fig.show(**kwargs)
 
         return fig
 
     def create_bar_chart(
         self,
@@ -294,39 +297,37 @@
         layout_kwargs : Dict[str, Any], optional
             Additional keyword arguments to apply with figure.update_layout(), by default None.
         Returns
         -------
         OpenBBFigure
             The OpenBBFigure object.
         """
-
         fig = bar_chart(
             data=data,
             x=x,
             y=y,
             barmode=barmode,
             xtype=xtype,
             title=title,
             xtitle=xtitle,
             ytitle=ytitle,
             orientation=orientation,
             colors=colors,
             bar_kwargs=bar_kwargs,
             layout_kwargs=layout_kwargs,
         )
-
+        fig = self._set_chart_style(fig)
         if render:
             return fig.show(**kwargs)
 
         return fig
 
     # pylint: disable=inconsistent-return-statements
     def show(self, render: bool = True, **kwargs):
         """Display chart and save it to the OBBject."""
-
         try:
             charting_function = self._get_chart_function(
                 self._obbject._route  # pylint: disable=protected-access
             )
             kwargs["obbject_item"] = self._obbject.results
             kwargs["charting_settings"] = self._charting_settings
             if (
@@ -341,22 +342,25 @@
             )  # pylint: disable=protected-access
             kwargs["extra"] = self._obbject.extra  # pylint: disable=protected-access
 
             if "kwargs" in kwargs:
                 _kwargs = kwargs.pop("kwargs")
                 kwargs.update(_kwargs.get("chart_params", {}))
             fig, content = charting_function(**kwargs)
+            fig = self._set_chart_style(fig)
+            content = fig.show(external=True, **kwargs).to_plotly_json()
             self._obbject.chart = Chart(
                 fig=fig, content=content, format=charting_router.CHART_FORMAT
             )
             if render:
                 fig.show(**kwargs)
-        except Exception:
+        except Exception:  # pylint: disable=W0718
             try:
                 fig = self.create_line_chart(data=self._obbject.results, render=False, **kwargs)  # type: ignore
+                fig = self._set_chart_style(fig)
                 content = fig.show(external=True, **kwargs).to_plotly_json()  # type: ignore
                 self._obbject.chart = Chart(
                     fig=fig, content=content, format=charting_router.CHART_FORMAT
                 )
                 if render:
                     return fig.show(**kwargs)  # type: ignore
             except Exception as e:
@@ -463,28 +467,57 @@
             _kwargs = kwargs.pop("kwargs")
             kwargs.update(_kwargs.get("chart_params", {}))
         try:
             if has_data:
                 self.show(data=data_as_df, render=render, **kwargs)
             else:
                 self.show(**kwargs, render=render)
-        except Exception:
+        except Exception:  # pylint: disable=W0718
             try:
                 fig = self.create_line_chart(data=data_as_df, render=False, **kwargs)
+                fig = self._set_chart_style(fig)
                 content = fig.show(external=True, **kwargs).to_plotly_json()  # type: ignore
                 self._obbject.chart = Chart(
                     fig=fig, content=content, format=charting_router.CHART_FORMAT
                 )
                 if render:
                     return fig.show(**kwargs)  # type: ignore
-            except Exception as e:
+            except Exception as e:  # pylint: disable=W0718
                 raise RuntimeError(
                     "Failed to automatically create a generic chart with the data provided."
                 ) from e
 
+    def _set_chart_style(self, figure: Figure):
+        """Set the user preference for light or dark mode."""
+        style = self._charting_settings.chart_style  # pylint: disable=protected-access
+        font_color = "black" if style == "light" else "white"
+        paper_bgcolor = "white" if style == "light" else "black"
+        figure = figure.update_layout(
+            dict(  # pylint: disable=R1735
+                font_color=font_color, paper_bgcolor=paper_bgcolor
+            )
+        )
+        return figure
+
+    def toggle_chart_style(self):  # pylint: disable=protected-access
+        """Toggle the chart style between light and dark mode."""
+        if not hasattr(self._obbject.chart, "fig"):
+            raise ValueError(
+                "Error: No chart has been created. Please create a chart first."
+            )
+        current = self._charting_settings.chart_style
+        new = "light" if current == "dark" else "dark"
+        self._charting_settings.chart_style = new
+        figure = self._obbject.chart.fig
+        updated_figure = self._set_chart_style(figure)
+        self._obbject.chart.fig = updated_figure
+        self._obbject.chart.content = updated_figure.show(
+            external=True
+        ).to_plotly_json()
+
     def table(
         self,
         data: Optional[Union[pd.DataFrame, pd.Series]] = None,
         title: str = "",
     ):
         """
         Display an interactive table.
@@ -506,15 +539,15 @@
             try:
                 self._backend.send_table(
                     df_table=data_as_df,
                     title=title
                     or self._obbject._route,  # pylint: disable=protected-access
                     theme=self._charting_settings.table_style,
                 )
-            except Exception as e:
+            except Exception as e:  # pylint: disable=W0718
                 warn(f"Failed to show figure with backend. {e}")
 
         else:
             from plotly import (  # pylint:disable=import-outside-toplevel
                 optional_imports,
             )
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/colors.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/colors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/generic_charts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py` & `openbb_nightly-4.1.7.dev202405080008/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/assets/reference.json` & `openbb_nightly-4.1.7.dev202405080008/openbb/assets/reference.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999473738789071%*

 * *Differences: {"'paths'": "{'/currency/search': {'parameters': {'polygon': {5: {'default': None}}}}, "*

 * *            "'/economy/fred_search': {'parameters': {'fred': {4: {'type': "*

 * *            '"Literal[\'frequency\', \'units\', \'seasonal_adjustment\']"}}}}, '*

 * *            '\'/economy/fred_series\': {\'parameters\': {\'fred\': {0: {\'type\': "Literal[\'a\', '*

 * *            "'q', 'm', 'w', 'd', 'wef', 'weth', 'wew', 'wetu', 'wem', 'wesu', 'wesa', 'bwew', "*

 * *            '\'bwem\']"}, 1: {\'type\': "Literal[\'avg\', \'sum\', \'e […]*

```diff
@@ -736,15 +736,15 @@
                         "default": "asc",
                         "description": "Order data by ascending or descending.",
                         "name": "order",
                         "optional": true,
                         "type": "Literal['asc', 'desc']"
                     },
                     {
-                        "default": "",
+                        "default": null,
                         "description": "Sort field used for ordering.",
                         "name": "sort",
                         "optional": true,
                         "type": "Literal['ticker', 'name', 'market', 'locale', 'currency_symbol', 'currency_name', 'base_currency_symbol', 'base_currency_name', 'last_updated_utc', 'delisted_utc']"
                     },
                     {
                         "default": 1000,
@@ -3031,15 +3031,15 @@
                         "type": "Annotated[int, Ge(ge=0)]"
                     },
                     {
                         "default": null,
                         "description": "Filter by an attribute.",
                         "name": "filter_variable",
                         "optional": true,
-                        "type": "Literal[None, 'frequency', 'units', 'seasonal_adjustment']"
+                        "type": "Literal['frequency', 'units', 'seasonal_adjustment']"
                     },
                     {
                         "default": null,
                         "description": "String value to filter the variable by. Used in conjunction with filter_variable.",
                         "name": "filter_value",
                         "optional": true,
                         "type": "str"
@@ -3145,29 +3145,29 @@
             "parameters": {
                 "fred": [
                     {
                         "default": null,
                         "description": "Frequency aggregation to convert high frequency data to lower frequency.       None = No change       a = Annual       q = Quarterly       m = Monthly       w = Weekly       d = Daily       wef = Weekly, Ending Friday       weth = Weekly, Ending Thursday       wew = Weekly, Ending Wednesday       wetu = Weekly, Ending Tuesday       wem = Weekly, Ending Monday       wesu = Weekly, Ending Sunday       wesa = Weekly, Ending Saturday       bwew = Biweekly, Ending Wednesday       bwem = Biweekly, Ending Monday",
                         "name": "frequency",
                         "optional": true,
-                        "type": "Literal[None, 'a', 'q', 'm', 'w', 'd', 'wef', 'weth', 'wew', 'wetu', 'wem', 'wesu', 'wesa', 'bwew', 'bwem']"
+                        "type": "Literal['a', 'q', 'm', 'w', 'd', 'wef', 'weth', 'wew', 'wetu', 'wem', 'wesu', 'wesa', 'bwew', 'bwem']"
                     },
                     {
                         "default": "eop",
                         "description": "A key that indicates the aggregation method used for frequency aggregation.     This parameter has no affect if the frequency parameter is not set.       avg = Average       sum = Sum       eop = End of Period",
                         "name": "aggregation_method",
                         "optional": true,
-                        "type": "Literal[None, 'avg', 'sum', 'eop']"
+                        "type": "Literal['avg', 'sum', 'eop']"
                     },
                     {
                         "default": null,
                         "description": "Transformation type       None = No transformation       chg = Change       ch1 = Change from Year Ago       pch = Percent Change       pc1 = Percent Change from Year Ago       pca = Compounded Annual Rate of Change       cch = Continuously Compounded Rate of Change       cca = Continuously Compounded Annual Rate of Change       log = Natural Log",
                         "name": "transform",
                         "optional": true,
-                        "type": "Literal[None, 'chg', 'ch1', 'pch', 'pc1', 'pca', 'cch', 'cca', 'log']"
+                        "type": "Literal['chg', 'ch1', 'pch', 'pc1', 'pca', 'cch', 'cca', 'log']"
                     }
                 ],
                 "intrinio": [
                     {
                         "default": false,
                         "description": "Returns all pages of data from the API call at once.",
                         "name": "all_pages",
@@ -3593,28 +3593,35 @@
                 ]
             },
             "deprecated": {
                 "flag": null,
                 "message": null
             },
             "description": "Get economic indicators by country and indicator.",
-            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.economy.indicators(provider='econdb', symbol='PCOCO')\n# Enter the country as the full name, or iso code. Use `available_indicators()` to get a list of supported indicators from EconDB.\nobb.economy.indicators(symbol='CPI', country='united_states,jp', provider='econdb')\n```\n\n",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.economy.indicators(provider='econdb', symbol='PCOCO')\n# Enter the country as the full name, or iso code. Use `available_indicators()` to get a list of supported indicators from EconDB.\nobb.economy.indicators(symbol='CPI', country='united_states,jp', provider='econdb')\n# Use the `main` symbol to get the group of main indicators for a country.\nobb.economy.indicators(provider='econdb', symbol='main', country='eu')\n```\n\n",
             "model": "EconomicIndicators",
             "parameters": {
                 "econdb": [
                     {
                         "default": null,
-                        "description": "The transformation to apply to the data, default is None.     tpop: Change from previous period     toya: Change from one year ago     tusd: Values as US dollars     tpgp: Values as a percent of GDP    Only 'tpop' and 'toya' are applicable to all indicators.   Applying transformations across multiple indicators/countries   may produce unexpected results.   This is because not all indicators are compatible with all transformations,   and the original units and scale differ between entities.   `tusd` should only be used where values are currencies.",
+                        "description": "The transformation to apply to the data, default is None.   tpop: Change from previous period   toya: Change from one year ago   tusd: Values as US dollars   tpgp: Values as a percent of GDP   Only 'tpop' and 'toya' are applicable to all indicators. Applying transformations across multiple indicators/countries may produce unexpected results.   This is because not all indicators are compatible with all transformations, and the original units and scale differ between entities.   `tusd` should only be used where values are currencies.",
                         "name": "transform",
                         "optional": true,
                         "type": "Literal['toya', 'tpop', 'tusd', 'tpgp']"
                     },
                     {
+                        "default": "quarter",
+                        "description": "The frequency of the data, default is 'quarter'. Only valid when 'symbol' is 'main'.",
+                        "name": "frequency",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'month']"
+                    },
+                    {
                         "default": true,
-                        "description": "If True, the request will be cached for one day.Using cache is recommended to avoid needlessly requesting the same data.",
+                        "description": "If True, the request will be cached for one day. Using cache is recommended to avoid needlessly requesting the same data.",
                         "name": "use_cache",
                         "optional": true,
                         "type": "bool"
                     }
                 ],
                 "standard": [
                     {
@@ -10256,22 +10263,22 @@
                         "type": "bool"
                     },
                     {
                         "default": null,
                         "description": "Order of the financial statement.",
                         "name": "order",
                         "optional": true,
-                        "type": "Literal[None, 'asc', 'desc']"
+                        "type": "Literal['asc', 'desc']"
                     },
                     {
                         "default": null,
                         "description": "Sort of the financial statement.",
                         "name": "sort",
                         "optional": true,
-                        "type": "Literal[None, 'filing_date', 'period_of_report_date']"
+                        "type": "Literal['filing_date', 'period_of_report_date']"
                     }
                 ],
                 "standard": [
                     {
                         "default": "",
                         "description": "Symbol to get data for.",
                         "name": "symbol",
@@ -10973,15 +10980,15 @@
                         "type": "date"
                     },
                     {
                         "default": null,
                         "description": "The SEC Act number.",
                         "name": "act",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The SEC Item numbers.",
                         "name": "items",
                         "optional": true,
                         "type": "Union[str, float]"
@@ -11001,50 +11008,50 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The accession number.",
                         "name": "accession_number",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The file number.",
                         "name": "file_number",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The film number.",
                         "name": "film_number",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "Whether the filing is an inline XBRL filing.",
                         "name": "is_inline_xbrl",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "Whether the filing is an XBRL filing.",
                         "name": "is_xbrl",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The size of the filing.",
                         "name": "size",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The URL to the complete filing submission.",
                         "name": "complete_submission_url",
                         "optional": true,
                         "type": "str"
@@ -11143,15 +11150,15 @@
                 ],
                 "sec": [
                     {
                         "default": null,
                         "description": "Lookup filings by Central Index Key (CIK) instead of by symbol.",
                         "name": "cik",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": true,
                         "description": "Whether or not to use cache. If True, cache will store for one day.",
                         "name": "use_cache",
                         "optional": true,
                         "type": "bool"
@@ -21818,29 +21825,29 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The rate tenor unit for receivable portion of the swap.",
                         "name": "rate_tenor_unit_rec",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The reset date for receivable portion of the swap.",
                         "name": "reset_date_rec",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The reset date unit for receivable portion of the swap.",
                         "name": "reset_date_unit_rec",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The type of rate for payment portion of the swap.",
                         "name": "rate_type_pmnt",
                         "optional": true,
                         "type": "str"
@@ -21881,29 +21888,29 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The rate tenor unit for payment portion of the swap.",
                         "name": "rate_tenor_unit_pmnt",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The reset date for payment portion of the swap.",
                         "name": "reset_date_pmnt",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "The reset date unit for payment portion of the swap.",
                         "name": "reset_date_unit_pmnt",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     },
                     {
                         "default": null,
                         "description": "The type of repo.",
                         "name": "repo_type",
                         "optional": true,
                         "type": "str"
@@ -26723,19 +26730,96 @@
                         "name": "source",
                         "optional": false,
                         "type": "str"
                     }
                 ],
                 "intrinio": [
                     {
+                        "default": null,
+                        "description": "The source of the news article.",
+                        "name": "source",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The summary of the news article.",
+                        "name": "summary",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The topics related to the news article.",
+                        "name": "topics",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The word count of the news article.",
+                        "name": "word_count",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
+                        "description": "How strongly correlated the news article is to the business",
+                        "name": "business_relevance",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The sentiment of the news article - i.e, negative, positive.",
+                        "name": "sentiment",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The confidence score of the sentiment rating.",
+                        "name": "sentiment_confidence",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The language of the news article.",
+                        "name": "language",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "Whether the news article is spam.",
+                        "name": "spam",
+                        "optional": true,
+                        "type": "bool"
+                    },
+                    {
+                        "default": null,
+                        "description": "The copyright notice of the news article.",
+                        "name": "copyright",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "",
                         "description": "Article ID.",
                         "name": "id",
                         "optional": false,
                         "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The Intrinio Security object. Contains the security details related to the news article.",
+                        "name": "security",
+                        "optional": true,
+                        "type": "IntrinioSecurity"
                     }
                 ],
                 "polygon": [
                     {
                         "default": null,
                         "description": "Source of the article.",
                         "name": "source",
@@ -26954,15 +27038,79 @@
                         "default": 0,
                         "description": "Page number of the results. Use in combination with limit.",
                         "name": "page",
                         "optional": true,
                         "type": "int"
                     }
                 ],
-                "intrinio": [],
+                "intrinio": [
+                    {
+                        "default": null,
+                        "description": "The source of the news article.",
+                        "name": "source",
+                        "optional": true,
+                        "type": "Literal['yahoo', 'moody', 'moody_us_news', 'moody_us_press_releases']"
+                    },
+                    {
+                        "default": null,
+                        "description": "Return news only from this source.",
+                        "name": "sentiment",
+                        "optional": true,
+                        "type": "Literal['positive', 'neutral', 'negative']"
+                    },
+                    {
+                        "default": null,
+                        "description": "Filter by language. Unsupported for yahoo source.",
+                        "name": "language",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "Filter by topic. Unsupported for yahoo source.",
+                        "name": "topic",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a word count greater than this value. Unsupported for yahoo source.",
+                        "name": "word_count_greater_than",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a word count less than this value. Unsupported for yahoo source.",
+                        "name": "word_count_less_than",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
+                        "description": "Filter whether it is marked as spam or not. Unsupported for yahoo source.",
+                        "name": "is_spam",
+                        "optional": true,
+                        "type": "bool"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a business relevance score more than this value. Unsupported for yahoo source.",
+                        "name": "business_relevance_greater_than",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a business relevance score less than this value. Unsupported for yahoo source.",
+                        "name": "business_relevance_less_than",
+                        "optional": true,
+                        "type": "float"
+                    }
+                ],
                 "polygon": [
                     {
                         "default": "desc",
                         "description": "Sort order of the articles.",
                         "name": "order",
                         "optional": true,
                         "type": "Literal['asc', 'desc']"
@@ -27113,26 +27261,103 @@
                         "name": "site",
                         "optional": false,
                         "type": "str"
                     }
                 ],
                 "intrinio": [
                     {
+                        "default": null,
+                        "description": "The source of the news article.",
+                        "name": "source",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The summary of the news article.",
+                        "name": "summary",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The topics related to the news article.",
+                        "name": "topics",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The word count of the news article.",
+                        "name": "word_count",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
+                        "description": "How strongly correlated the news article is to the business",
+                        "name": "business_relevance",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The sentiment of the news article - i.e, negative, positive.",
+                        "name": "sentiment",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "The confidence score of the sentiment rating.",
+                        "name": "sentiment_confidence",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "The language of the news article.",
+                        "name": "language",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "Whether the news article is spam.",
+                        "name": "spam",
+                        "optional": true,
+                        "type": "bool"
+                    },
+                    {
+                        "default": null,
+                        "description": "The copyright notice of the news article.",
+                        "name": "copyright",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "",
                         "description": "Article ID.",
                         "name": "id",
                         "optional": false,
                         "type": "str"
                     },
                     {
-                        "default": "",
-                        "description": "Company details related to the news article.",
+                        "default": null,
+                        "description": "The Intrinio Company object. Contains details company reference data.",
                         "name": "company",
-                        "optional": false,
-                        "type": "Dict[str, Any]"
+                        "optional": true,
+                        "type": "IntrinioCompany"
+                    },
+                    {
+                        "default": null,
+                        "description": "The Intrinio Security object. Contains the security details related to the news article.",
+                        "name": "security",
+                        "optional": true,
+                        "type": "IntrinioSecurity"
                     }
                 ],
                 "standard": [
                     {
                         "default": "",
                         "description": "The date of the data. The published date of the article.",
                         "name": "date",
@@ -27297,15 +27522,79 @@
                         "description": "Content types of the news to retrieve.",
                         "name": "content_types",
                         "optional": true,
                         "type": "str"
                     }
                 ],
                 "fmp": [],
-                "intrinio": [],
+                "intrinio": [
+                    {
+                        "default": null,
+                        "description": "The source of the news article.",
+                        "name": "source",
+                        "optional": true,
+                        "type": "Literal['yahoo', 'moody', 'moody_us_news', 'moody_us_press_releases']"
+                    },
+                    {
+                        "default": null,
+                        "description": "Return news only from this source.",
+                        "name": "sentiment",
+                        "optional": true,
+                        "type": "Literal['positive', 'neutral', 'negative']"
+                    },
+                    {
+                        "default": null,
+                        "description": "Filter by language. Unsupported for yahoo source.",
+                        "name": "language",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "Filter by topic. Unsupported for yahoo source.",
+                        "name": "topic",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a word count greater than this value. Unsupported for yahoo source.",
+                        "name": "word_count_greater_than",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a word count less than this value. Unsupported for yahoo source.",
+                        "name": "word_count_less_than",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
+                        "description": "Filter whether it is marked as spam or not. Unsupported for yahoo source.",
+                        "name": "is_spam",
+                        "optional": true,
+                        "type": "bool"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a business relevance score more than this value. Unsupported for yahoo source.",
+                        "name": "business_relevance_greater_than",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "default": null,
+                        "description": "News stories will have a business relevance score less than this value. Unsupported for yahoo source.",
+                        "name": "business_relevance_less_than",
+                        "optional": true,
+                        "type": "float"
+                    }
+                ],
                 "standard": [
                     {
                         "default": 2500,
                         "description": "The number of data entries to return. The number of articles to return.",
                         "name": "limit",
                         "optional": true,
                         "type": "int"
@@ -27467,15 +27756,15 @@
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "Central Index Key (CIK)",
                         "name": "cik",
                         "optional": true,
-                        "type": "Union[str, int]"
+                        "type": "Union[int, str]"
                     }
                 ],
                 "standard": []
             },
             "deprecated": {
                 "flag": null,
                 "message": null
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/__extensions__.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/crypto.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/crypto_price.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/currency.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/currency.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/currency_price.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/currency_price.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/derivatives.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/derivatives_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,17 +205,17 @@
             Start date of the data, in YYYY-MM-DD format. If no symbol is supplied, requests are only allowed for a single date. Use the start_date for the target date. Intrinio appears to have data beginning Feb/2022, but is unclear when it actually began. (provider: intrinio)
         end_date : Optional[datetime.date]
             End date of the data, in YYYY-MM-DD format. If a symbol is not supplied, do not include an end date. (provider: intrinio)
         trade_type : Optional[Literal['block', 'sweep', 'large']]
             The type of unusual activity to query for. (provider: intrinio)
         sentiment : Optional[Literal['bullish', 'bearish', 'neutral']]
             The sentiment type to query for. (provider: intrinio)
-        min_value : Optional[Union[float, int]]
+        min_value : Optional[Union[int, float]]
             The inclusive minimum total value for the unusual activity. (provider: intrinio)
-        max_value : Optional[Union[float, int]]
+        max_value : Optional[Union[int, float]]
             The inclusive maximum total value for the unusual activity. (provider: intrinio)
         limit : int
             The number of data entries to return. A typical day for all symbols will yield 50-80K records. The API will paginate at 1000 records. The high default limit (100K) is to be able to reliably capture the most days. The high absolute limit (1.25M) is to allow for outlier days. Queries at the absolute limit will take a long time, and might be unreliable. Apply filters to improve performance. (provider: intrinio)
         source : Literal['delayed', 'realtime']
             The source of the data. Either realtime or delayed. (provider: intrinio)
 
         Returns
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/economy.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/economy.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
             Is release?  If True, other search filter variables are ignored. If no query text or release_id is supplied, this defaults to True. (provider: fred)
         release_id : Optional[Union[int, str]]
             A specific release ID to target. (provider: fred)
         limit : Optional[int]
             The number of data entries to return. (1-1000) (provider: fred)
         offset : Optional[Annotated[int, Ge(ge=0)]]
             Offset the results in conjunction with limit. (provider: fred)
-        filter_variable : Literal[None, 'frequency', 'units', 'seasonal_adjustment']
+        filter_variable : Optional[Literal['frequency', 'units', 'seasonal_adjustment']]
             Filter by an attribute. (provider: fred)
         filter_value : Optional[str]
             String value to filter the variable by.  Used in conjunction with filter_variable. (provider: fred)
         tag_names : Optional[str]
             A semicolon delimited list of tag names that series match all of.  Example: 'japan;imports' (provider: fred)
         exclude_tag_names : Optional[str]
             A semicolon delimited list of tag names that series match none of.  Example: 'imports;services'. Requires that variable tag_names also be set to limit the number of matching series. (provider: fred)
@@ -927,15 +927,15 @@
             End date of the data, in YYYY-MM-DD format.
         limit : Optional[int]
             The number of data entries to return.
         provider : Optional[Literal['fred', 'intrinio']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fred' if there is
             no default.
-        frequency : Literal[None, 'a', 'q', 'm', 'w', 'd', 'wef', 'weth', 'wew', 'wetu', 'wem', 'wesu', 'wesa', 'bwew', 'bwem']
+        frequency : Optional[Literal['a', 'q', 'm', 'w', 'd', 'wef', 'weth', 'wew', 'wetu', 'wem', 'wesu', 'wesa', 'bwew', 'bwem']]
 
                 Frequency aggregation to convert high frequency data to lower frequency.
                     None = No change
                     a = Annual
                     q = Quarterly
                     m = Monthly
                     w = Weekly
@@ -946,23 +946,23 @@
                     wetu = Weekly, Ending Tuesday
                     wem = Weekly, Ending Monday
                     wesu = Weekly, Ending Sunday
                     wesa = Weekly, Ending Saturday
                     bwew = Biweekly, Ending Wednesday
                     bwem = Biweekly, Ending Monday
                  (provider: fred)
-        aggregation_method : Literal[None, 'avg', 'sum', 'eop']
+        aggregation_method : Optional[Literal['avg', 'sum', 'eop']]
 
                 A key that indicates the aggregation method used for frequency aggregation.
                 This parameter has no affect if the frequency parameter is not set.
                     avg = Average
                     sum = Sum
                     eop = End of Period
                  (provider: fred)
-        transform : Literal[None, 'chg', 'ch1', 'pch', 'pc1', 'pca', 'cch', 'cca', 'log']
+        transform : Optional[Literal['chg', 'ch1', 'pch', 'pc1', 'pca', 'cch', 'cca', 'log']]
 
                 Transformation type
                     None = No transformation
                     chg = Change
                     ch1 = Change from Year Ago
                     pch = Percent Change
                     pc1 = Percent Change from Year Ago
@@ -1079,27 +1079,29 @@
             Start date of the data, in YYYY-MM-DD format.
         end_date : Union[datetime.date, None, str]
             End date of the data, in YYYY-MM-DD format.
         provider : Optional[Literal['econdb']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'econdb' if there is
             no default.
-        transform : Literal['toya', 'tpop', 'tusd', 'tpgp']
+        transform : Optional[Literal['toya', 'tpop', 'tusd', 'tpgp']]
             The transformation to apply to the data, default is None.
 
-                tpop: Change from previous period
-                toya: Change from one year ago
-                tusd: Values as US dollars
-                tpgp: Values as a percent of GDP
-
-             Only 'tpop' and 'toya' are applicable to all indicators.     Applying transformations across multiple indicators/countries     may produce unexpected results.
-             This is because not all indicators are compatible with all transformations,     and the original units and scale differ between entities.
-             `tusd` should only be used where values are currencies. (provider: econdb)
+            tpop: Change from previous period
+            toya: Change from one year ago
+            tusd: Values as US dollars
+            tpgp: Values as a percent of GDP
+
+            Only 'tpop' and 'toya' are applicable to all indicators. Applying transformations across multiple indicators/countries may produce unexpected results.
+            This is because not all indicators are compatible with all transformations, and the original units and scale differ between entities.
+            `tusd` should only be used where values are currencies. (provider: econdb)
+        frequency : Literal['annual', 'quarter', 'month']
+            The frequency of the data, default is 'quarter'. Only valid when 'symbol' is 'main'. (provider: econdb)
         use_cache : bool
-            If True, the request will be cached for one day.Using cache is recommended to avoid needlessly requesting the same data. (provider: econdb)
+            If True, the request will be cached for one day. Using cache is recommended to avoid needlessly requesting the same data. (provider: econdb)
 
         Returns
         -------
         OBBject
             results : List[EconomicIndicators]
                 Serializable results.
             provider : Optional[Literal['econdb']]
@@ -1126,14 +1128,16 @@
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.economy.indicators(provider='econdb', symbol='PCOCO')
         >>> # Enter the country as the full name, or iso code. Use `available_indicators()` to get a list of supported indicators from EconDB.
         >>> obb.economy.indicators(symbol='CPI', country='united_states,jp', provider='econdb')
+        >>> # Use the `main` symbol to get the group of main indicators for a country.
+        >>> obb.economy.indicators(provider='econdb', symbol='main', country='eu')
         """  # noqa: E501
 
         return self._run(
             "/economy/indicators",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_compare.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_fundamental.py`

 * *Files 1% similar despite different names*

```diff
@@ -615,17 +615,17 @@
             Period of report date less than or equal to the given date. (provider: polygon)
         period_of_report_date_gt : Optional[datetime.date]
             Period of report date greater than the given date. (provider: polygon)
         period_of_report_date_gte : Optional[datetime.date]
             Period of report date greater than or equal to the given date. (provider: polygon)
         include_sources : bool
             Whether to include the sources of the financial statement. (provider: polygon)
-        order : Literal[None, 'asc', 'desc']
+        order : Optional[Literal['asc', 'desc']]
             Order of the financial statement. (provider: polygon)
-        sort : Literal[None, 'filing_date', 'period_of_report_date']
+        sort : Optional[Literal['filing_date', 'period_of_report_date']]
             Sort of the financial statement. (provider: polygon)
 
         Returns
         -------
         OBBject
             results : List[CashFlowStatement]
                 Serializable results.
@@ -1193,15 +1193,15 @@
             no default.
         start_date : Optional[datetime.date]
             Start date of the data, in YYYY-MM-DD format. (provider: intrinio)
         end_date : Optional[datetime.date]
             End date of the data, in YYYY-MM-DD format. (provider: intrinio)
         thea_enabled : Optional[bool]
             Return filings that have been read by Intrinio's Thea NLP. (provider: intrinio)
-        cik : Optional[Union[str, int]]
+        cik : Optional[Union[int, str]]
             Lookup filings by Central Index Key (CIK) instead of by symbol. (provider: sec)
         use_cache : bool
             Whether or not to use cache.  If True, cache will store for one day. (provider: sec)
 
         Returns
         -------
         OBBject
@@ -1242,33 +1242,33 @@
             URL for the XBRL filing for the report. (provider: intrinio)
         industry_group : Optional[str]
             Industry group of the company. (provider: intrinio)
         industry_category : Optional[str]
             Industry category of the company. (provider: intrinio)
         report_date : Optional[date]
             The date of the filing. (provider: sec)
-        act : Optional[Union[str, int]]
+        act : Optional[Union[int, str]]
             The SEC Act number. (provider: sec)
         items : Optional[Union[str, float]]
             The SEC Item numbers. (provider: sec)
         primary_doc_description : Optional[str]
             The description of the primary document. (provider: sec)
         primary_doc : Optional[str]
             The filename of the primary document. (provider: sec)
-        accession_number : Optional[Union[str, int]]
+        accession_number : Optional[Union[int, str]]
             The accession number. (provider: sec)
-        file_number : Optional[Union[str, int]]
+        file_number : Optional[Union[int, str]]
             The file number. (provider: sec)
-        film_number : Optional[Union[str, int]]
+        film_number : Optional[Union[int, str]]
             The film number. (provider: sec)
-        is_inline_xbrl : Optional[Union[str, int]]
+        is_inline_xbrl : Optional[Union[int, str]]
             Whether the filing is an inline XBRL filing. (provider: sec)
-        is_xbrl : Optional[Union[str, int]]
+        is_xbrl : Optional[Union[int, str]]
             Whether the filing is an XBRL filing. (provider: sec)
-        size : Optional[Union[str, int]]
+        size : Optional[Union[int, str]]
             The size of the filing. (provider: sec)
         complete_submission_url : Optional[str]
             The URL to the complete filing submission. (provider: sec)
         filing_detail_url : Optional[str]
             The URL to the filing details. (provider: sec)
 
         Examples
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             Deemed execution date of the trade. (provider: intrinio)
         exercise_date : Optional[date]
             Exercise date of the trade. (provider: intrinio)
         expiration_date : Optional[date]
             Expiration date of the derivative. (provider: intrinio)
         underlying_security_title : Optional[str]
             Name of the underlying non-derivative security related to this derivative transaction. (provider: intrinio)
-        underlying_shares : Optional[Union[float, int]]
+        underlying_shares : Optional[Union[int, float]]
             Number of underlying shares related to this derivative transaction. (provider: intrinio)
         nature_of_ownership : Optional[str]
             Nature of ownership of the insider trading. (provider: intrinio)
         director : Optional[bool]
             Whether the owner is a director. (provider: intrinio)
         officer : Optional[bool]
             Whether the owner is an officer. (provider: intrinio)
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_price.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             The open price.
         high : float
             The high price.
         low : float
             The low price.
         close : float
             The close price.
-        volume : Optional[Union[float, int]]
+        volume : Optional[Union[int, float]]
             The trading volume.
         vwap : Optional[float]
             Volume Weighted Average Price over the period.
         adj_close : Optional[float]
             The adjusted close price. (provider: fmp, intrinio, tiingo)
         unadjusted_volume : Optional[float]
             Unadjusted volume of the symbol. (provider: fmp)
@@ -504,17 +504,17 @@
             The open price.
         high : Optional[float]
             The high price.
         low : Optional[float]
             The low price.
         close : Optional[float]
             The close price.
-        volume : Optional[Union[float, int]]
+        volume : Optional[Union[int, float]]
             The trading volume.
-        exchange_volume : Optional[Union[float, int]]
+        exchange_volume : Optional[Union[int, float]]
             Volume of shares exchanged during the trading day on the specific exchange.
         prev_close : Optional[float]
             The previous close price.
         change : Optional[float]
             Change in price from previous close.
         change_percent : Optional[float]
             Change in price as a normalized percentage.
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/etf.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/etf.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             The symbol of the equity requested.
         etf_symbol : str
             The symbol of the ETF with exposure to the requested equity.
         shares : Optional[float]
             The number of shares held in the ETF.
         weight : Optional[float]
             The weight of the equity in the ETF, as a normalized percent.
-        market_value : Optional[Union[float, int]]
+        market_value : Optional[Union[int, float]]
             The market value of the equity position in the ETF.
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.etf.equity_exposure(symbol='MSFT', provider='fmp')
         >>> # This function accepts multiple tickers.
@@ -275,15 +275,15 @@
             The open price.
         high : float
             The high price.
         low : float
             The low price.
         close : float
             The close price.
-        volume : Optional[Union[float, int]]
+        volume : Optional[Union[int, float]]
             The trading volume.
         vwap : Optional[float]
             Volume Weighted Average Price over the period.
         adj_close : Optional[float]
             The adjusted close price. (provider: fmp, intrinio, tiingo)
         unadjusted_volume : Optional[float]
             Unadjusted volume of the symbol. (provider: fmp)
@@ -534,37 +534,37 @@
             The upfront amount received of the swap. (provider: sec)
         floating_rate_index_rec : Optional[str]
             The floating rate index for receivable portion of the swap. (provider: sec)
         floating_rate_spread_rec : Optional[float]
             The floating rate spread for reveivable portion of the swap. (provider: sec)
         rate_tenor_rec : Optional[str]
             The rate tenor for receivable portion of the swap. (provider: sec)
-        rate_tenor_unit_rec : Optional[Union[str, int]]
+        rate_tenor_unit_rec : Optional[Union[int, str]]
             The rate tenor unit for receivable portion of the swap. (provider: sec)
         reset_date_rec : Optional[str]
             The reset date for receivable portion of the swap. (provider: sec)
-        reset_date_unit_rec : Optional[Union[str, int]]
+        reset_date_unit_rec : Optional[Union[int, str]]
             The reset date unit for receivable portion of the swap. (provider: sec)
         rate_type_pmnt : Optional[str]
             The type of rate for payment portion of the swap. (provider: sec)
         payment_currency : Optional[str]
             The payment currency of the swap. (provider: sec)
         upfront_payment : Optional[float]
             The upfront amount received of the swap. (provider: sec)
         floating_rate_index_pmnt : Optional[str]
             The floating rate index for payment portion of the swap. (provider: sec)
         floating_rate_spread_pmnt : Optional[float]
             The floating rate spread for payment portion of the swap. (provider: sec)
         rate_tenor_pmnt : Optional[str]
             The rate tenor for payment portion of the swap. (provider: sec)
-        rate_tenor_unit_pmnt : Optional[Union[str, int]]
+        rate_tenor_unit_pmnt : Optional[Union[int, str]]
             The rate tenor unit for payment portion of the swap. (provider: sec)
         reset_date_pmnt : Optional[str]
             The reset date for payment portion of the swap. (provider: sec)
-        reset_date_unit_pmnt : Optional[Union[str, int]]
+        reset_date_unit_pmnt : Optional[Union[int, str]]
             The reset date unit for payment portion of the swap. (provider: sec)
         repo_type : Optional[str]
             The type of repo. (provider: sec)
         is_cleared : Optional[str]
             If the repo is cleared. (provider: sec)
         is_tri_party : Optional[str]
             If the repo is tri party. (provider: sec)
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_corporate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/index.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/index.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/openbb/package/news.py` & `openbb_nightly-4.1.7.dev202405080008/openbb/package/news.py`

 * *Files 27% similar despite different names*

```diff
@@ -92,18 +92,35 @@
             Topics of the news to retrieve. (provider: benzinga)
         authors : Optional[str]
             Authors of the news to retrieve. (provider: benzinga)
         content_types : Optional[str]
             Content types of the news to retrieve. (provider: benzinga)
         page : Optional[int]
             Page number of the results. Use in combination with limit. (provider: fmp)
+        source : Optional[Union[Literal['yahoo', 'moody', 'moody_us_news', 'moody_us_press_releases'], str]]
+            The source of the news article. (provider: intrinio);
+            A comma-separated list of the domains requested. (provider: tiingo)
+        sentiment : Optional[Literal['positive', 'neutral', 'negative']]
+            Return news only from this source. (provider: intrinio)
+        language : Optional[str]
+            Filter by language. Unsupported for yahoo source. (provider: intrinio)
+        topic : Optional[str]
+            Filter by topic. Unsupported for yahoo source. (provider: intrinio)
+        word_count_greater_than : Optional[int]
+            News stories will have a word count greater than this value. Unsupported for yahoo source. (provider: intrinio)
+        word_count_less_than : Optional[int]
+            News stories will have a word count less than this value. Unsupported for yahoo source. (provider: intrinio)
+        is_spam : Optional[bool]
+            Filter whether it is marked as spam or not. Unsupported for yahoo source. (provider: intrinio)
+        business_relevance_greater_than : Optional[float]
+            News stories will have a business relevance score more than this value. Unsupported for yahoo source. (provider: intrinio)
+        business_relevance_less_than : Optional[float]
+            News stories will have a business relevance score less than this value. Unsupported for yahoo source. (provider: intrinio)
         offset : Optional[int]
             Page offset, used in conjunction with limit. (provider: tiingo)
-        source : Optional[str]
-            A comma-separated list of the domains requested. (provider: tiingo)
 
         Returns
         -------
         OBBject
             results : List[CompanyNews]
                 Serializable results.
             provider : Optional[Literal['benzinga', 'fmp', 'intrinio', 'polygon', 'tiingo', 'yfinance']]
@@ -141,17 +158,38 @@
             Stocks associated with the news. (provider: benzinga)
         tags : Optional[str]
             Tags associated with the news. (provider: benzinga, polygon, tiingo)
         updated : Optional[datetime]
             Updated date of the news. (provider: benzinga)
         source : Optional[str]
             Name of the news source. (provider: fmp);
+            The source of the news article. (provider: intrinio);
             Source of the article. (provider: polygon);
             News source. (provider: tiingo);
             Source of the news article (provider: yfinance)
+        summary : Optional[str]
+            The summary of the news article. (provider: intrinio)
+        topics : Optional[str]
+            The topics related to the news article. (provider: intrinio)
+        word_count : Optional[int]
+            The word count of the news article. (provider: intrinio)
+        business_relevance : Optional[float]
+                How strongly correlated the news article is to the business (provider: intrinio)
+        sentiment : Optional[str]
+            The sentiment of the news article - i.e, negative, positive. (provider: intrinio)
+        sentiment_confidence : Optional[float]
+            The confidence score of the sentiment rating. (provider: intrinio)
+        language : Optional[str]
+            The language of the news article. (provider: intrinio)
+        spam : Optional[bool]
+            Whether the news article is spam. (provider: intrinio)
+        copyright : Optional[str]
+            The copyright notice of the news article. (provider: intrinio)
+        security : Optional[IntrinioSecurity]
+            The Intrinio Security object. Contains the security details related to the news article. (provider: intrinio)
         amp_url : Optional[str]
             AMP URL. (provider: polygon)
         publisher : Optional[PolygonPublisher]
             Publisher of the article. (provider: polygon)
         article_id : Optional[int]
             Unique ID of the news article. (provider: tiingo)
         crawl_date : Optional[datetime]
@@ -271,18 +309,35 @@
             Channels of the news to retrieve. (provider: benzinga)
         topics : Optional[str]
             Topics of the news to retrieve. (provider: benzinga)
         authors : Optional[str]
             Authors of the news to retrieve. (provider: benzinga)
         content_types : Optional[str]
             Content types of the news to retrieve. (provider: benzinga)
+        source : Optional[Union[Literal['yahoo', 'moody', 'moody_us_news', 'moody_us_press_releases'], str]]
+            The source of the news article. (provider: intrinio);
+            A comma-separated list of the domains requested. (provider: tiingo)
+        sentiment : Optional[Literal['positive', 'neutral', 'negative']]
+            Return news only from this source. (provider: intrinio)
+        language : Optional[str]
+            Filter by language. Unsupported for yahoo source. (provider: intrinio)
+        topic : Optional[str]
+            Filter by topic. Unsupported for yahoo source. (provider: intrinio)
+        word_count_greater_than : Optional[int]
+            News stories will have a word count greater than this value. Unsupported for yahoo source. (provider: intrinio)
+        word_count_less_than : Optional[int]
+            News stories will have a word count less than this value. Unsupported for yahoo source. (provider: intrinio)
+        is_spam : Optional[bool]
+            Filter whether it is marked as spam or not. Unsupported for yahoo source. (provider: intrinio)
+        business_relevance_greater_than : Optional[float]
+            News stories will have a business relevance score more than this value. Unsupported for yahoo source. (provider: intrinio)
+        business_relevance_less_than : Optional[float]
+            News stories will have a business relevance score less than this value. Unsupported for yahoo source. (provider: intrinio)
         offset : Optional[int]
             Page offset, used in conjunction with limit. (provider: tiingo)
-        source : Optional[str]
-            A comma-separated list of the domains requested. (provider: tiingo)
 
         Returns
         -------
         OBBject
             results : List[WorldNews]
                 Serializable results.
             provider : Optional[Literal['benzinga', 'fmp', 'intrinio', 'tiingo']]
@@ -318,16 +373,38 @@
             Stocks associated with the news. (provider: benzinga)
         tags : Optional[str]
             Tags associated with the news. (provider: benzinga, tiingo)
         updated : Optional[datetime]
             Updated date of the news. (provider: benzinga)
         site : Optional[str]
             News source. (provider: fmp, tiingo)
-        company : Optional[Dict[str, Any]]
-            Company details related to the news article. (provider: intrinio)
+        source : Optional[str]
+            The source of the news article. (provider: intrinio)
+        summary : Optional[str]
+            The summary of the news article. (provider: intrinio)
+        topics : Optional[str]
+            The topics related to the news article. (provider: intrinio)
+        word_count : Optional[int]
+            The word count of the news article. (provider: intrinio)
+        business_relevance : Optional[float]
+                How strongly correlated the news article is to the business (provider: intrinio)
+        sentiment : Optional[str]
+            The sentiment of the news article - i.e, negative, positive. (provider: intrinio)
+        sentiment_confidence : Optional[float]
+            The confidence score of the sentiment rating. (provider: intrinio)
+        language : Optional[str]
+            The language of the news article. (provider: intrinio)
+        spam : Optional[bool]
+            Whether the news article is spam. (provider: intrinio)
+        copyright : Optional[str]
+            The copyright notice of the news article. (provider: intrinio)
+        company : Optional[IntrinioCompany]
+            The Intrinio Company object. Contains details company reference data. (provider: intrinio)
+        security : Optional[IntrinioSecurity]
+            The Intrinio Security object. Contains the security details related to the news article. (provider: intrinio)
         symbols : Optional[str]
             Ticker tagged in the fetched news. (provider: tiingo)
         article_id : Optional[int]
             Unique ID of the news article. (provider: tiingo)
         crawl_date : Optional[datetime]
             Date the news article was crawled. (provider: tiingo)
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class CboeIndexSnapshotsQueryParams(IndexSnapshotsQueryParams):
     """CBOE Index Snapshots Query.
 
     Source: https://www.cboe.com/
     """
 
-    region: Literal[None, "us", "eu"] = Field(
+    region: Optional[Literal["us", "eu"]] = Field(
         default="us",
     )
 
     @field_validator("region", mode="after", check_fields=False)
     @classmethod
     def validate_region(cls, v: str):
         """Validate region."""
@@ -85,59 +85,61 @@
     def transform_query(params: Dict[str, Any]) -> CboeIndexSnapshotsQueryParams:
         """Transform the query."""
         return CboeIndexSnapshotsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeIndexSnapshotsQueryParams,
-        credentials: Optional[Dict[str, str]],
+        credentials: Optional[Dict[str, str]],  # pylint: disable=unused-argument
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Cboe endpoint"""
 
         if query.region == "us":
             url = "https://cdn.cboe.com/api/global/delayed_quotes/quotes/all_us_indices.json"
         if query.region == "eu":
             url = "https://cdn.cboe.com/api/global/european_indices/index_quotes/all-indices.json"
 
         data = await amake_request(url, **kwargs)
         return data.get("data")
 
     @staticmethod
     def transform_data(
-        query: CboeIndexSnapshotsQueryParams, data: dict, **kwargs: Any
+        query: CboeIndexSnapshotsQueryParams,  # pylint: disable=unused-argument
+        data: dict,
+        **kwargs: Any,  # pylint: disable=unused-argument
     ) -> List[CboeIndexSnapshotsData]:
         """Transform the data to the standard format"""
         if not data:
             raise EmptyDataError()
-        data = DataFrame(data)
+        df = DataFrame(data)
         percent_cols = [
             "price_change_percent",
             "iv30",
             "iv30_change",
             "iv30_change_percent",
         ]
         for col in percent_cols:
-            if col in data.columns:
-                data[col] = round(data[col] / 100, 6)
-        data = (
-            data.replace(0, None)
+            if col in df.columns:
+                df[col] = round(df[col] / 100, 6)
+        df = (
+            df.replace(0, None)
             .replace("", None)
             .dropna(how="all", axis=1)
             .fillna("N/A")
             .replace("N/A", None)
         )
         drop_cols = [
             "exchange_id",
             "seqno",
             "index",
             "security_type",
             "ask_size",
             "bid_size",
         ]
         for col in drop_cols:
-            if col in data.columns:
-                data = data.drop(columns=col)
+            if col in df.columns:
+                df = df.drop(columns=col)
         return [
             CboeIndexSnapshotsData.model_validate(d)
-            for d in data.to_dict(orient="records")
+            for d in df.to_dict(orient="records")
         ]
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, List, Optional
 
 from openbb_cboe.utils.helpers import (
     TICKER_EXCEPTIONS,
     get_company_directory,
     get_index_directory,
 )
+from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.options_chains import (
     OptionsChainsData,
     OptionsChainsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
@@ -58,45 +59,80 @@
         return CboeOptionsChainsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeOptionsChainsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
-    ) -> List[Dict]:
-        """Return the raw data from the Cboe endpoint"""
-
-        symbol = query.symbol.replace("^", "").split(",")[0]
+    ) -> Dict:
+        """Return the raw data from the Cboe endpoint."""
+        symbol = query.symbol.replace("^", "").split(",")[0].upper()
         INDEXES = await get_index_directory(use_cache=query.use_cache)
         SYMBOLS = await get_company_directory(use_cache=query.use_cache)
         INDEXES = INDEXES.set_index("index_symbol")
 
         if symbol not in SYMBOLS.index:
             raise RuntimeError(f"{symbol} was not found in the Cboe options directory.")
 
         quotes_url = (
             f"https://cdn.cboe.com/api/global/delayed_quotes/options/_{symbol}.json"
             if symbol in TICKER_EXCEPTIONS or symbol in INDEXES.index
             else f"https://cdn.cboe.com/api/global/delayed_quotes/options/{symbol}.json"
         )
-
-        return await amake_request(quotes_url)
+        results = await amake_request(quotes_url)
+        return results  # type: ignore
 
     @staticmethod
     def transform_data(
         query: CboeOptionsChainsQueryParams,
-        data: List[Dict],
+        data: Dict,
         **kwargs: Any,
-    ) -> List[CboeOptionsChainsData]:
-        """Transform the data to the standard format"""
-
+    ) -> AnnotatedResult[List[CboeOptionsChainsData]]:
+        """Transform the data to the standard format."""
         if not data:
             raise EmptyDataError()
+        results_metadata = {}
+        options = data.get("data", {}).pop("options", [])
+        change_percent = data["data"].get("percent_change", None)
+        iv30_percent = data["data"].get("iv30_change_percent", None)
+        if change_percent:
+            change_percent = change_percent / 100
+        if iv30_percent:
+            iv30_percent = iv30_percent / 100
+        last_timestamp = data["data"].get("last_trade_time", None)
+        if last_timestamp:
+            last_timestamp = to_datetime(
+                last_timestamp, format="%Y-%m-%dT%H:%M:%S"
+            ).strftime("%Y-%m-%d %H:%M:%S")
+        results_metadata.update(
+            {
+                "symbol": data["data"].get("symbol"),
+                "security_type": data["data"].get("security_type", None),
+                "bid": data["data"].get("bid", None),
+                "bid_size": data["data"].get("bid_size", None),
+                "ask": data["data"].get("ask", None),
+                "ask_size": data["data"].get("ask_size", None),
+                "open": data["data"].get("open", None),
+                "high": data["data"].get("high", None),
+                "low": data["data"].get("low", None),
+                "close": data["data"].get("close", None),
+                "volume": data["data"].get("volume", None),
+                "current_price": data["data"].get("current_price", None),
+                "prev_close": data["data"].get("prev_day_close", None),
+                "change": data["data"].get("price_change", None),
+                "change_percent": change_percent,
+                "iv30": data["data"].get("iv30", None),
+                "iv30_change": data["data"].get("iv30_change", None),
+                "iv30_change_percent": iv30_percent,
+                "last_tick": data["data"].get("tick", None),
+                "last_trade_timestamp": last_timestamp,
+            }
+        )
 
-        options_df = DataFrame.from_records(data["data"]["options"])
+        options_df = DataFrame.from_records(options)
 
         options_df = options_df.rename(
             columns={
                 "option": "contract_symbol",
                 "iv": "implied_volatility",
                 "theo": "theoretical_price",
                 "percent_change": "change_percent",
@@ -148,11 +184,14 @@
         quotes["open_interest"] = quotes["open_interest"].astype("int64")
         quotes["volume"] = quotes["volume"].astype("int64")
         quotes["bid_size"] = quotes["bid_size"].astype("int64")
         quotes["ask_size"] = quotes["ask_size"].astype("int64")
         quotes["prev_close"] = round(quotes["prev_close"], 2)
         quotes["change_percent"] = round(quotes["change_percent"] / 100, 4)
 
-        return [
-            CboeOptionsChainsData.model_validate(d)
-            for d in quotes.reset_index().to_dict("records")
-        ]
+        return AnnotatedResult(
+            result=[
+                CboeOptionsChainsData.model_validate(d)
+                for d in quotes.reset_index().to_dict("records")
+            ],
+            metadata=results_metadata,
+        )
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.7.dev202405080008/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/available_indicators.py` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/country_profile.py` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/models/economic_indicators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 """EconDB Economic Indicators."""
 
 # pylint: disable=unused-argument
 
 from datetime import datetime, timedelta
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Literal, Optional, Union
 from warnings import warn
 
 from openbb_core.provider.abstract.annotated_result import AnnotatedResult
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.economic_indicators import (
     EconomicIndicatorsData,
     EconomicIndicatorsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_econdb.utils import helpers
+from openbb_econdb.utils.main_indicators import get_main_indicators
 from pandas import DataFrame, concat
 from pydantic import Field, field_validator
 
 INDICATORS = list(helpers.INDICATORS_DESCRIPTIONS)
 
 
 class EconDbEconomicIndicatorsQueryParams(EconomicIndicatorsQueryParams):
     """EconDB Economic Indicators Query."""
 
     __json_schema_extra__ = {
         "symbol": ["multiple_items_allowed"],
         "country": ["multiple_items_allowed"],
     }
 
-    transform: Literal["toya", "tpop", "tusd", "tpgp"] = Field(
+    transform: Union[None, Literal["toya", "tpop", "tusd", "tpgp"]] = Field(
         default=None,
         description="The transformation to apply to the data, default is None."
         + "\n"
-        + "\n        tpop: Change from previous period"
-        + "\n        toya: Change from one year ago"
-        + "\n        tusd: Values as US dollars"
-        + "\n        tpgp: Values as a percent of GDP"
+        + "\n    tpop: Change from previous period"
+        + "\n    toya: Change from one year ago"
+        + "\n    tusd: Values as US dollars"
+        + "\n    tpgp: Values as a percent of GDP"
         + "\n"
         + "\n"
-        + "     Only 'tpop' and 'toya' are applicable to all indicators."
-        + "     Applying transformations across multiple indicators/countries"
-        + "     may produce unexpected results."
-        + "\n     This is because not all indicators are compatible with all transformations,"
-        + "     and the original units and scale differ between entities."
-        + "\n     `tusd` should only be used where values are currencies.",
+        + "    Only 'tpop' and 'toya' are applicable to all indicators."
+        + " Applying transformations across multiple indicators/countries"
+        + " may produce unexpected results."
+        + "\n    This is because not all indicators are compatible with all transformations,"
+        + " and the original units and scale differ between entities."
+        + "\n    `tusd` should only be used where values are currencies.",
+    )
+    frequency: Literal["annual", "quarter", "month"] = Field(
+        default="quarter",
+        description="The frequency of the data, default is 'quarter'."
+        + " Only valid when 'symbol' is 'main'.",
     )
     use_cache: bool = Field(
         default=True,
         description="If True, the request will be cached for one day."
-        + "Using cache is recommended to avoid needlessly requesting the same data.",
+        + " Using cache is recommended to avoid needlessly requesting the same data.",
     )
 
     @field_validator("country", mode="before", check_fields=False)
     @classmethod
     def validate_countries(cls, v):
         """Validate each country and convert to a two-letter ISO code."""
         if v:
@@ -85,20 +91,28 @@
             return ",".join(country)
         return None
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def validate_symbols(cls, v):
         """Validate each symbol to check if it is a valid indicator."""
+        if not v:
+            v = "main"
         symbols = v if isinstance(v, list) else v.split(",")
         new_symbols: List[str] = []
         for symbol in symbols:
             if "_" in symbol:
                 new_symbols.append(symbol)
                 continue
+            if symbol.upper() == "MAIN":
+                if len(symbols) > 1:
+                    raise ValueError(
+                        "The 'main' indicator cannot be combined with other indicators."
+                    )
+                return symbol
             if not any(
                 (
                     symbol.upper().startswith(indicator)
                     if len(symbol) >= len(indicator)
                     else symbol.upper() == indicator
                 )
                 for indicator in INDICATORS
@@ -131,23 +145,42 @@
         new_params = params.copy()
         if new_params.get("start_date") is None:
             new_params["start_date"] = (
                 datetime.today() - timedelta(weeks=52 * 11)
             ).date()
         if new_params.get("end_date") is None:
             new_params["end_date"] = datetime.today().date()
+        countries = new_params.get("country")
+        if (
+            countries is not None
+            and len(countries.split(",")) > 1
+            and new_params.get("symbol", "").upper() == "MAIN"
+        ):
+            raise ValueError(
+                "The 'main' indicator cannot be combined with multiple countries."
+            )
         return EconDbEconomicIndicatorsQueryParams(**new_params)
 
     @staticmethod
     async def aextract_data(  # pylint: disable=R0914.R0912,R0915
         query: EconDbEconomicIndicatorsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the data."""
+        if query.symbol.upper() == "MAIN":
+            country = query.country.upper() if query.country else "US"
+            return await get_main_indicators(
+                country,
+                query.start_date.strftime("%Y-%m-%d"),  # type: ignore
+                query.end_date.strftime("%Y-%m-%d"),  # type: ignore
+                query.frequency,
+                query.transform,
+                query.use_cache,
+            )
         token = credentials.get("econdb_api_key", "")  # type: ignore
         # Attempt to create a temporary token if one is not supplied.
         if not token:
             token = await helpers.create_token(use_cache=query.use_cache)
             credentials.update({"econdb_api_key": token})  # type: ignore
         base_url = "https://www.econdb.com/api/series/?ticker="
         data: List[Dict] = []
@@ -295,14 +328,22 @@
     @staticmethod
     def transform_data(  # pylint: disable=R0914,R0915
         query: EconDbEconomicIndicatorsQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> AnnotatedResult[List[EconDbEconomicIndicatorsData]]:
         """Transform the data."""
+        if query.symbol.upper() == "MAIN":
+            return AnnotatedResult(
+                result=[
+                    EconDbEconomicIndicatorsData.model_validate(r)
+                    for r in data[0].get("records", [])
+                ],
+                metadata={query.country: data[0].get("metadata", [])},
+            )
         output = DataFrame()
         metadata = {}
         for d in data:
             if "data" in d and not d["data"].get("values"):
                 warn(
                     f"Symbol Error: No data found for '{d.get('ticker', '')}'."
                     + " The country has data, but not for the requested date range."
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/indicator_countries.json` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/indicator_countries.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/indicators_descriptions.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/multipliers.json` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/multipliers.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/scales.json` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/scales.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/econdb/openbb_econdb/utils/units.json` & `openbb_nightly-4.1.7.dev202405080008/providers/econdb/openbb_econdb/utils/units.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405080008/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         default=None,
         description=QUERY_DESCRIPTIONS.get("limit", "") + " (1-1000)",
     )
     offset: Optional[NonNegativeInt] = Field(
         default=0,
         description="Offset the results in conjunction with limit.",
     )
-    filter_variable: Literal[None, "frequency", "units", "seasonal_adjustment"] = Field(
-        default=None, description="Filter by an attribute."
+    filter_variable: Optional[Literal["frequency", "units", "seasonal_adjustment"]] = (
+        Field(default=None, description="Filter by an attribute.")
     )
     filter_value: Optional[str] = Field(
         default=None,
         description="String value to filter the variable by.  Used in conjunction with filter_variable.",
     )
     tag_names: Optional[str] = Field(
         default=None,
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,30 +26,31 @@
         "symbol": "series_id",
         "start_date": "observation_start",
         "end_date": "observation_end",
         "transform": "units",
     }
     __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
 
-    frequency: Literal[
-        None,
-        "a",
-        "q",
-        "m",
-        "w",
-        "d",
-        "wef",
-        "weth",
-        "wew",
-        "wetu",
-        "wem",
-        "wesu",
-        "wesa",
-        "bwew",
-        "bwem",
+    frequency: Optional[
+        Literal[
+            "a",
+            "q",
+            "m",
+            "w",
+            "d",
+            "wef",
+            "weth",
+            "wew",
+            "wetu",
+            "wem",
+            "wesu",
+            "wesa",
+            "bwew",
+            "bwem",
+        ]
     ] = Field(
         default=None,
         description="""
         Frequency aggregation to convert high frequency data to lower frequency.
             None = No change
             a = Annual
             q = Quarterly
@@ -63,40 +64,40 @@
             wem = Weekly, Ending Monday
             wesu = Weekly, Ending Sunday
             wesa = Weekly, Ending Saturday
             bwew = Biweekly, Ending Wednesday
             bwem = Biweekly, Ending Monday
         """,
     )
-    aggregation_method: Literal[None, "avg", "sum", "eop"] = Field(
+    aggregation_method: Optional[Literal["avg", "sum", "eop"]] = Field(
         default="eop",
         description="""
         A key that indicates the aggregation method used for frequency aggregation.
         This parameter has no affect if the frequency parameter is not set.
             avg = Average
             sum = Sum
             eop = End of Period
         """,
     )
-    transform: Literal[None, "chg", "ch1", "pch", "pc1", "pca", "cch", "cca", "log"] = (
-        Field(
-            default=None,
-            description="""
+    transform: Optional[
+        Literal["chg", "ch1", "pch", "pc1", "pca", "cch", "cca", "log"]
+    ] = Field(
+        default=None,
+        description="""
         Transformation type
             None = No transformation
             chg = Change
             ch1 = Change from Year Ago
             pch = Percent Change
             pc1 = Percent Change from Year Ago
             pca = Compounded Annual Rate of Change
             cch = Continuously Compounded Rate of Change
             cca = Continuously Compounded Annual Rate of Change
             log = Natural Log
         """,
-        )
     )
     limit: int = Field(description=QUERY_DESCRIPTIONS.get("limit", ""), default=100000)
 
 
 class FredSeriesData(SeriesData):
     """FRED Series Data."""
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.7.dev202405080008/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """US Government Treasury Prices."""
 
 # pylint: disable=unused-argument
 import asyncio
-from datetime import datetime, timedelta
+from datetime import date, timedelta
 from io import StringIO
 from typing import Any, Dict, List, Literal, Optional
 
 import requests
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.treasury_prices import (
     TreasuryPricesData,
@@ -18,15 +18,15 @@
 from pydantic import Field
 
 
 class GovernmentUSTreasuryPricesQueryParams(TreasuryPricesQueryParams):
     """US Government Treasury Prices Query."""
 
     cusip: Optional[str] = Field(description="Filter by CUSIP.", default=None)
-    security_type: Literal[None, "bill", "note", "bond", "tips", "frn"] = Field(
+    security_type: Optional[Literal["bill", "note", "bond", "tips", "frn"]] = Field(
         description="Filter by security type.",
         default=None,
     )
 
 
 class GovernmentUSTreasuryPricesData(TreasuryPricesData):
     """US Government Treasury Prices Data."""
@@ -41,26 +41,22 @@
     """US Government Treasury Prices Fetcher."""
 
     @staticmethod
     def transform_query(
         params: Dict[str, Any]
     ) -> GovernmentUSTreasuryPricesQueryParams:
         """Transform query params."""
+        yesterday = date.today() - timedelta(days=1)
+        last_bd = (
+            yesterday - timedelta(yesterday.weekday() - 4)
+            if yesterday.weekday() > 4
+            else yesterday
+        )
         if params.get("date") is None:
-            _date = datetime.now().date()
-        else:
-            _date = (
-                datetime.strptime(params["date"], "%Y-%m-%d").date()
-                if isinstance(params["date"], str)
-                else params["date"]
-            )
-        if _date.weekday() > 4:
-            _date = _date - timedelta(days=_date.weekday() - 4)
-        params["date"] = _date
-
+            params["date"] = last_bd
         return GovernmentUSTreasuryPricesQueryParams(**params)
 
     # pylint: disable=unused-argument
     @staticmethod
     async def aextract_data(
         query: GovernmentUSTreasuryPricesQueryParams,
         credentials: Optional[Dict[str, str]],
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/search_attributes.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.7.dev202405080008/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.7.dev202405080008/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,18 +60,18 @@
         default=None,
         description="Period of report date greater than or equal to the given date.",
     )
     include_sources: bool = Field(
         default=False,
         description="Whether to include the sources of the financial statement.",
     )
-    order: Literal[None, "asc", "desc"] = Field(
+    order: Optional[Literal["asc", "desc"]] = Field(
         default=None, description="Order of the financial statement."
     )
-    sort: Literal[None, "filing_date", "period_of_report_date"] = Field(
+    sort: Optional[Literal["filing_date", "period_of_report_date"]] = Field(
         default=None, description="Sort of the financial statement."
     )
 
 
 class PolygonCashFlowStatementData(CashFlowStatementData):
     """Polygon Cash Flow Statement Data."""
 
@@ -156,17 +156,17 @@
 
         request_url = f"{base_url}?{query_string}&apiKey={api_key}"
 
         return await get_data_many(request_url, "results", **kwargs)
 
     @staticmethod
     def transform_data(
-        query: PolygonCashFlowStatementQueryParams,
+        query: PolygonCashFlowStatementQueryParams,  # pylint: disable=unused-argument
         data: dict,
-        **kwargs: Any,
+        **kwargs: Any,  # pylint: disable=unused-argument
     ) -> List[PolygonCashFlowStatementData]:
         """Return the transformed data."""
         transformed_data = []
 
         for item in data:
             sub_data = {
                 key: value["value"]
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             "currency_symbol",
             "currency_name",
             "base_currency_symbol",
             "base_currency_name",
             "last_updated_utc",
             "delisted_utc",
         ]
-    ] = Field(default="", description="Sort field used for ordering.")
+    ] = Field(default=None, description="Sort field used for ordering.")
     limit: Optional[PositiveInt] = Field(
         default=1000, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
 
 
 class PolygonCurrencyPairsData(CurrencyPairsData):
     """Polygon Currency Available Pairs Data."""
@@ -102,17 +102,16 @@
     """Transform the query, extract and transform the data from the Polygon endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> PolygonCurrencyPairsQueryParams:
         """Transform the query parameters. Ticker is set if symbol is provided."""
         transform_params = params
         now = datetime.now().date().isoformat()
-        transform_params["symbol"] = (
-            f"ticker=C:{params.get('symbol').upper()}" if params.get("symbol") else ""
-        )
+        symbol = params.get("symbol")
+        transform_params["symbol"] = f"ticker=C:{symbol.upper()}" if symbol else ""
         if params.get("date") is None:
             transform_params["date"] = now
 
         return PolygonCurrencyPairsQueryParams(**transform_params)
 
     @staticmethod
     async def aextract_data(
@@ -123,20 +122,21 @@
         """Extract the data from the Polygon API."""
         api_key = credentials.get("polygon_api_key") if credentials else ""
 
         request_url = (
             f"https://api.polygon.io/v3/reference/"
             f"tickers?{query.symbol}&market=fx&date={query.date}&"
             f"search={query.search}&active={query.active}&order={query.order}&"
-            f"limit={query.limit}&sort={query.sort}&apiKey={api_key}"
+            f"limit={query.limit}"
         )
-
+        if query.sort:
+            request_url += f"&sort={query.sort}"
+        request_url = f"{request_url}&apiKey={api_key}"
         data = {"next_url": request_url}
         all_data: List[Dict] = []
-
         while "next_url" in data:
             data = await get_data(request_url, **kwargs)
 
             if isinstance(data, list):
                 raise ValueError("Expected a dict, got a list")
 
             if len(data["results"]) == 0:
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             if cik is False
             else await parse_13f.get_13f_candidates(cik=symbol)
         )
         if query.limit and query.date is None:
             urls = filings.iloc[: query.limit].to_list()
         if query.date is not None:
             date = parse_13f.date_to_quarter_end(query.date.strftime("%Y-%m-%d"))
+            filings.index = filings.index.astype(str)
             urls = [filings.loc[date]]
 
         results = []
 
         async def get_filing(url):
             """Get a single 13F-HR filing and parse it."""
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if r.status_code == 200:
             data = xmltodict.parse(r.content)
             cols = ["title", "link", "summary", "date", "id"]
             feed = pd.DataFrame.from_records(data["rss"]["channel"]["item"])[
                 ["title", "link", "description", "pubDate", "dc:creator"]
             ]
             feed.columns = cols
-            feed["date"] = pd.to_datetime(feed["date"])
+            feed["date"] = pd.to_datetime(feed["date"], format="mixed")
             feed = feed.set_index("date")
             # Remove special characters
             for column in ["title", "summary"]:
                 feed[column] = (
                     feed[column]
                     .replace(r"[^\w\s]|_", "", regex=True)
                     .replace(r"\n", "", regex=True)
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.7.dev202405080008/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202405080008/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.7.dev202405080008/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from pydantic import Field, field_validator
 
 
 class TmxIndexSnapshotsQueryParams(IndexSnapshotsQueryParams):
     """TMX Index Snapshots Query Params."""
 
-    region: Literal[None, "ca", "us"] = Field(default="ca")  # type: ignore
+    region: Optional[Literal["ca", "us"]] = Field(default="ca")  # type: ignore
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request."
         + " Index data is from a single JSON file, updated each day after close."
         + " It is cached for one day. To bypass, set to False.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-"""TMX Treasury Prices Fetcher"""
+"""TMX Treasury Prices Fetcher."""
 
 # pylint: disable=unused-argument
 from datetime import (
     date as dateType,
-    datetime,
     timedelta,
 )
 from typing import Any, Dict, List, Literal, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.treasury_prices import (
     TreasuryPricesData,
@@ -15,16 +14,15 @@
 )
 from openbb_tmx.utils.helpers import get_all_bonds
 from pandas import DataFrame
 from pydantic import Field, field_validator
 
 
 class TmxTreasuryPricesQueryParams(TreasuryPricesQueryParams):
-    """
-    TMX Treasury Prices Query Params.
+    """TMX Treasury Prices Query Params.
 
     Data will be made available by 5:00 EST on T+1
 
     Source: https://bondtradedata.iiroc.ca/#/
     """
 
     govt_type: Literal["federal", "provincial", "municipal"] = Field(
@@ -95,21 +93,22 @@
 ):
     """Tmx Bond Reference Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> TmxTreasuryPricesQueryParams:
         """Transform query params."""
         transformed_params = params.copy()
-        now = datetime.now()
-        if now.date().weekday() > 4:
-            now = now - timedelta(now.date().weekday() - 4)
+        yesterday = dateType.today() - timedelta(days=1)
+        last_bd = (
+            yesterday - timedelta(yesterday.weekday() - 4)
+            if yesterday.weekday() > 4
+            else yesterday
+        )
         if "maturity_date_min" not in transformed_params:
-            transformed_params["maturity_date_min"] = (
-                now - timedelta(days=1)
-            ).strftime("%Y-%m-%d")
+            transformed_params["maturity_date_min"] = last_bd
         return TmxTreasuryPricesQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
         query: TmxTreasuryPricesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.7.dev202405080008/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.7.dev202405080008/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405070009/pyproject.toml` & `openbb_nightly-4.1.7.dev202405080008/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.7.dev202405070009"
+version = "4.1.7.dev202405080008"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
@@ -197,14 +197,15 @@
 aiohttp = "^3.9.0"
 ruff = "^0.1.6"
 requests-cache = "^1.1.0"
 pytest-freezegun = "^0.4.2"
 urllib3 = ">1.26.16"
 defusedxml = "^0.8.0rc2"
 xmltodict = "^0.13.0"
+lxml = "^5.2.1"
 random-user-agent = "^1.0.1"
 yfinance = "^0.2.27"
 aiohttp-client-cache = "^0.10.0"
 aiosqlite = "^0.19.0"
 nasdaq-data-link = "^1.0.4"
 exchange-calendars = "^4.2.8"
 finvizfinance = "0.14.7"
```

### Comparing `openbb_nightly-4.1.7.dev202405070009/PKG-INFO` & `openbb_nightly-4.1.7.dev202405080008/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.7.dev202405070009
+Version: 4.1.7.dev202405080008
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,14 +21,15 @@
 Requires-Dist: exchange-calendars (>=4.2.8,<5.0.0)
 Requires-Dist: fastapi (>=0.104.1,<0.105.0)
 Requires-Dist: finvizfinance (==0.14.7)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
 Requires-Dist: ipykernel (>=6.26.0,<7.0.0)
 Requires-Dist: linearmodels (<=4.25)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: mypy (>=1.6.1,<2.0.0)
 Requires-Dist: nasdaq-data-link (>=1.0.4,<2.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: plotly (>=5.17.0,<6.0.0)
 Requires-Dist: poetry (>=1.7.0,<2.0.0)
```


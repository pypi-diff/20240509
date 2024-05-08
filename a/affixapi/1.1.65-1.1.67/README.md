# Comparing `tmp/affixapi-1.1.65.tar.gz` & `tmp/affixapi-1.1.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.65.tar", last modified: Fri Apr 26 11:36:24 2024, max compression
+gzip compressed data, was "affixapi-1.1.67.tar", last modified: Wed May  8 23:01:54 2024, max compression
```

## Comparing `affixapi-1.1.65.tar` & `affixapi-1.1.67.tar`

### file list

```diff
@@ -1,156 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.085887 affixapi-1.1.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-26 11:36:20.000000 affixapi-1.1.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21927 2024-04-26 11:36:24.085887 affixapi-1.1.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-04-26 11:36:20.000000 affixapi-1.1.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.081887 affixapi-1.1.65/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21927 2024-04-26 11:36:24.000000 affixapi-1.1.65/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-26 11:36:24.000000 affixapi-1.1.65/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:36:24.000000 affixapi-1.1.65/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-26 11:36:24.000000 affixapi-1.1.65/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 11:36:24.000000 affixapi-1.1.65/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.061887 affixapi-1.1.65/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.061887 affixapi-1.1.65/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.061887 affixapi-1.1.65/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.073886 affixapi-1.1.65/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.073886 affixapi-1.1.65/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-26 11:36:20.000000 affixapi-1.1.65/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 11:36:24.085887 affixapi-1.1.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-26 11:36:20.000000 affixapi-1.1.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:36:24.081887 affixapi-1.1.65/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-26 11:36:20.000000 affixapi-1.1.65/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.571288 affixapi-1.1.67/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 23:01:51.000000 affixapi-1.1.67/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-05-08 23:01:54.571288 affixapi-1.1.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-08 23:01:51.000000 affixapi-1.1.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.567288 affixapi-1.1.67/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-05-08 23:01:54.000000 affixapi-1.1.67/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-08 23:01:54.000000 affixapi-1.1.67/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:01:54.000000 affixapi-1.1.67/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 23:01:54.000000 affixapi-1.1.67/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 23:01:54.000000 affixapi-1.1.67/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.543289 affixapi-1.1.67/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.547289 affixapi-1.1.67/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.547289 affixapi-1.1.67/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.559289 affixapi-1.1.67/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18785 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18797 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16765 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.559289 affixapi-1.1.67/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-08 23:01:51.000000 affixapi-1.1.67/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 23:01:54.571288 affixapi-1.1.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-08 23:01:51.000000 affixapi-1.1.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:54.567288 affixapi-1.1.67/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-08 23:01:51.000000 affixapi-1.1.67/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.65/LICENSE` & `affixapi-1.1.67/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/PKG-INFO` & `affixapi-1.1.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.65
+Version: 1.1.67
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -392,14 +392,15 @@
  - [Payruns20230301Response](docs/Payruns20230301Response.md)
  - [PayslipResponse](docs/PayslipResponse.md)
  - [PayslipResponseContributions](docs/PayslipResponseContributions.md)
  - [PayslipResponseDeductions](docs/PayslipResponseDeductions.md)
  - [PayslipResponseEarnings](docs/PayslipResponseEarnings.md)
  - [PayslipResponseTaxes](docs/PayslipResponseTaxes.md)
  - [Payslips20230301Response](docs/Payslips20230301Response.md)
+ - [PolicyTypeResponse](docs/PolicyTypeResponse.md)
  - [ProviderRequest](docs/ProviderRequest.md)
  - [ProviderResponse](docs/ProviderResponse.md)
  - [ProvidersResponse](docs/ProvidersResponse.md)
  - [ScopesRequest](docs/ScopesRequest.md)
  - [ScopesResponse](docs/ScopesResponse.md)
  - [TimeOffBalanceResponse](docs/TimeOffBalanceResponse.md)
  - [TimeOffBalances20230301Response](docs/TimeOffBalances20230301Response.md)
```

### Comparing `affixapi-1.1.65/README.md` & `affixapi-1.1.67/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -378,14 +378,15 @@
  - [Payruns20230301Response](docs/Payruns20230301Response.md)
  - [PayslipResponse](docs/PayslipResponse.md)
  - [PayslipResponseContributions](docs/PayslipResponseContributions.md)
  - [PayslipResponseDeductions](docs/PayslipResponseDeductions.md)
  - [PayslipResponseEarnings](docs/PayslipResponseEarnings.md)
  - [PayslipResponseTaxes](docs/PayslipResponseTaxes.md)
  - [Payslips20230301Response](docs/Payslips20230301Response.md)
+ - [PolicyTypeResponse](docs/PolicyTypeResponse.md)
  - [ProviderRequest](docs/ProviderRequest.md)
  - [ProviderResponse](docs/ProviderResponse.md)
  - [ProvidersResponse](docs/ProvidersResponse.md)
  - [ScopesRequest](docs/ScopesRequest.md)
  - [ScopesResponse](docs/ScopesResponse.md)
  - [TimeOffBalanceResponse](docs/TimeOffBalanceResponse.md)
  - [TimeOffBalances20230301Response](docs/TimeOffBalances20230301Response.md)
```

### Comparing `affixapi-1.1.65/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.67/affixapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.65
+Version: 1.1.67
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -392,14 +392,15 @@
  - [Payruns20230301Response](docs/Payruns20230301Response.md)
  - [PayslipResponse](docs/PayslipResponse.md)
  - [PayslipResponseContributions](docs/PayslipResponseContributions.md)
  - [PayslipResponseDeductions](docs/PayslipResponseDeductions.md)
  - [PayslipResponseEarnings](docs/PayslipResponseEarnings.md)
  - [PayslipResponseTaxes](docs/PayslipResponseTaxes.md)
  - [Payslips20230301Response](docs/Payslips20230301Response.md)
+ - [PolicyTypeResponse](docs/PolicyTypeResponse.md)
  - [ProviderRequest](docs/ProviderRequest.md)
  - [ProviderResponse](docs/ProviderResponse.md)
  - [ProvidersResponse](docs/ProvidersResponse.md)
  - [ScopesRequest](docs/ScopesRequest.md)
  - [ScopesResponse](docs/ScopesResponse.md)
  - [TimeOffBalanceResponse](docs/TimeOffBalanceResponse.md)
  - [TimeOffBalances20230301Response](docs/TimeOffBalances20230301Response.md)
```

### Comparing `affixapi-1.1.65/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.67/affixapi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 openapi_client/model/payruns20230301_response.py
 openapi_client/model/payslip_response.py
 openapi_client/model/payslip_response_contributions.py
 openapi_client/model/payslip_response_deductions.py
 openapi_client/model/payslip_response_earnings.py
 openapi_client/model/payslip_response_taxes.py
 openapi_client/model/payslips20230301_response.py
+openapi_client/model/policy_type_response.py
 openapi_client/model/provider_request.py
 openapi_client/model/provider_response.py
 openapi_client/model/providers_response.py
 openapi_client/model/scopes_request.py
 openapi_client/model/scopes_response.py
 openapi_client/model/time_off_balance_response.py
 openapi_client/model/time_off_balances20230301_response.py
@@ -125,14 +126,15 @@
 test/test_payruns20230301_response.py
 test/test_payslip_response.py
 test/test_payslip_response_contributions.py
 test/test_payslip_response_deductions.py
 test/test_payslip_response_earnings.py
 test/test_payslip_response_taxes.py
 test/test_payslips20230301_response.py
+test/test_policy_type_response.py
 test/test_provider_request.py
 test/test_provider_response.py
 test/test_providers_response.py
 test/test_scopes_request.py
 test/test_scopes_response.py
 test/test_time_off_balance_response.py
 test/test_time_off_balances20230301_response.py
```

### Comparing `affixapi-1.1.65/openapi_client/__init__.py` & `affixapi-1.1.67/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.67/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/api/core_api.py` & `affixapi-1.1.67/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/api/management_api.py` & `affixapi-1.1.67/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.67/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/api_client.py` & `affixapi-1.1.67/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/apis/__init__.py` & `affixapi-1.1.67/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/configuration.py` & `affixapi-1.1.67/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/exceptions.py` & `affixapi-1.1.67/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.67/openapi_client/model/address_no_non_null_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,54 +51,75 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('country',): {
             'None': None,
+            'BZ': "BZ",
             'CA': "CA",
-            'US': "US",
+            'CR': "CR",
+            'GT': "GT",
             'MX': "MX",
+            'PA': "PA",
+            'SV': "SV",
+            'US': "US",
+            'AR': "AR",
+            'BR': "BR",
+            'CL': "CL",
+            'PE': "PE",
             'AT': "AT",
             'AU': "AU",
             'BE': "BE",
             'CH': "CH",
+            'CY': "CY",
             'CZ': "CZ",
             'DE': "DE",
             'DK': "DK",
             'EE': "EE",
             'ES': "ES",
             'FI': "FI",
             'FR': "FR",
             'GB': "GB",
+            'GR': "GR",
             'IE': "IE",
             'IM': "IM",
             'IS': "IS",
             'IT': "IT",
             'LI': "LI",
             'LT': "LT",
             'LU': "LU",
             'LV': "LV",
             'NL': "NL",
             'NO': "NO",
             'PH': "PH",
             'PL': "PL",
             'RO': "RO",
+            'RU': "RU",
             'SE': "SE",
             'SK': "SK",
             'CN': "CN",
             'HK': "HK",
             'ID': "ID",
+            'IL': "IL",
             'IN': "IN",
             'JP': "JP",
             'KR': "KR",
             'MO': "MO",
             'MY': "MY",
+            'PH': "PH",
+            'PS': "PS",
             'SG': "SG",
+            'TH': "TH",
+            'TR': "TR",
             'TW': "TW",
+            'VN': "VN",
+            'ZA': "ZA",
+            'AU': "AU",
+            'NZ': "NZ",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
```

### Comparing `affixapi-1.1.65/openapi_client/model/address_response.py` & `affixapi-1.1.67/openapi_client/model/address_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,54 +52,75 @@
           as additional properties values.
     """
 
     allowed_values = {
         ('country',): {
             'None': None,
             'NULL': "null",
+            'BZ': "BZ",
             'CA': "CA",
-            'US': "US",
+            'CR': "CR",
+            'GT': "GT",
             'MX': "MX",
+            'PA': "PA",
+            'SV': "SV",
+            'US': "US",
+            'AR': "AR",
+            'BR': "BR",
+            'CL': "CL",
+            'PE': "PE",
             'AT': "AT",
             'AU': "AU",
             'BE': "BE",
             'CH': "CH",
+            'CY': "CY",
             'CZ': "CZ",
             'DE': "DE",
             'DK': "DK",
             'EE': "EE",
             'ES': "ES",
             'FI': "FI",
             'FR': "FR",
             'GB': "GB",
+            'GR': "GR",
             'IE': "IE",
             'IM': "IM",
             'IS': "IS",
             'IT': "IT",
             'LI': "LI",
             'LT': "LT",
             'LU': "LU",
             'LV': "LV",
             'NL': "NL",
             'NO': "NO",
             'PH': "PH",
             'PL': "PL",
             'RO': "RO",
+            'RU': "RU",
             'SE': "SE",
             'SK': "SK",
             'CN': "CN",
             'HK': "HK",
             'ID': "ID",
+            'IL': "IL",
             'IN': "IN",
             'JP': "JP",
             'KR': "KR",
             'MO': "MO",
             'MY': "MY",
+            'PH': "PH",
+            'PS': "PS",
             'SG': "SG",
+            'TH': "TH",
+            'TR': "TR",
             'TW': "TW",
+            'VN': "VN",
+            'ZA': "ZA",
+            'AU': "AU",
+            'NZ': "NZ",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
```

### Comparing `affixapi-1.1.65/openapi_client/model/client_request.py` & `affixapi-1.1.67/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/client_response.py` & `affixapi-1.1.67/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.67/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/company_response.py` & `affixapi-1.1.67/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/create_employee_request.py` & `affixapi-1.1.67/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.67/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/create_employee_request_dependents.py` & `affixapi-1.1.67/openapi_client/model/create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/create_employee_request_emergency_contacts.py` & `affixapi-1.1.67/openapi_client/model/create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.67/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.67/openapi_client/model/currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/currency_response.py` & `affixapi-1.1.67/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/disconnect_response.py` & `affixapi-1.1.67/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employee_response.py` & `affixapi-1.1.67/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.67/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.67/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.67/openapi_client/model/employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employment_response.py` & `affixapi-1.1.67/openapi_client/model/employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employment_status_not_null_not_nullable.py` & `affixapi-1.1.67/openapi_client/model/employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employment_status_not_null_request.py` & `affixapi-1.1.67/openapi_client/model/employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/employment_status_response.py` & `affixapi-1.1.67/openapi_client/model/employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.67/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/group_response.py` & `affixapi-1.1.67/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.67/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.67/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.67/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/identity_response.py` & `affixapi-1.1.67/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/inline_response400.py` & `affixapi-1.1.67/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/inline_response401.py` & `affixapi-1.1.67/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/inline_response409.py` & `affixapi-1.1.67/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/introspect_response.py` & `affixapi-1.1.67/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.67/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/location_response.py` & `affixapi-1.1.67/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/message_response.py` & `affixapi-1.1.67/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/mode_request.py` & `affixapi-1.1.67/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/mode_response.py` & `affixapi-1.1.67/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payrun_response.py` & `affixapi-1.1.67/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.67/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payslip_response.py` & `affixapi-1.1.67/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.67/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.67/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.67/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.67/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.67/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/provider_request.py` & `affixapi-1.1.67/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/provider_response.py` & `affixapi-1.1.67/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/providers_response.py` & `affixapi-1.1.67/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/scopes_request.py` & `affixapi-1.1.67/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/scopes_response.py` & `affixapi-1.1.67/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.67/openapi_client/model/timesheet_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class TimeOffBalanceResponse(ModelNormal):
+class TimesheetResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,27 +49,20 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('policy_type',): {
-            'None': None,
-            'NULL': "null",
-            'VACATION': "vacation",
-            'SICK': "sick",
-            'PERSONAL': "personal",
-            'JURY_DUTY': "jury_duty",
-            'VOLUNTEER': "volunteer",
-            'BEREAVEMENT': "bereavement",
-        },
     }
 
     validations = {
+        ('hours_worked',): {
+            'multiple_of': 0.1,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -79,36 +72,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'employee_id': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'remote_id': (str,),  # noqa: E501
-            'balance': (float, none_type,),  # noqa: E501
-            'used': (float, none_type,),  # noqa: E501
-            'policy_name': (str, none_type,),  # noqa: E501
-            'policy_type': (str, none_type,),  # noqa: E501
+            'employee_id': (str,),  # noqa: E501
+            'employee_remote_id': (str,),  # noqa: E501
+            'start_time': (datetime, none_type,),  # noqa: E501
+            'end_time': (datetime, none_type,),  # noqa: E501
+            'hours_worked': (float,),  # noqa: E501
             'remote_created_at': (date, none_type,),  # noqa: E501
             'remote_modified_at': (date, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'employee_id': 'employee_id',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'remote_id': 'remote_id',  # noqa: E501
-        'balance': 'balance',  # noqa: E501
-        'used': 'used',  # noqa: E501
-        'policy_name': 'policy_name',  # noqa: E501
-        'policy_type': 'policy_type',  # noqa: E501
+        'employee_id': 'employee_id',  # noqa: E501
+        'employee_remote_id': 'employee_remote_id',  # noqa: E501
+        'start_time': 'start_time',  # noqa: E501
+        'end_time': 'end_time',  # noqa: E501
+        'hours_worked': 'hours_worked',  # noqa: E501
         'remote_created_at': 'remote_created_at',  # noqa: E501
         'remote_modified_at': 'remote_modified_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
@@ -117,24 +112,25 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, employee_id, remote_id, balance, used, policy_name, policy_type, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
-        """TimeOffBalanceResponse - a model defined in OpenAPI
+    def __init__(self, id, remote_id, employee_id, employee_remote_id, start_time, end_time, hours_worked, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
+        """TimesheetResponse - a model defined in OpenAPI
 
         Args:
-            employee_id (str): The Affix-assigned id of the individual
-            remote_id (str): the remote system-assigned id of the individual
-            balance (float, none_type):
-            used (float, none_type):
-            policy_name (str, none_type): The name of the policy, as assigned by the remote system
-            policy_type (str, none_type):
+            id (str): The Affix-assigned id of the time off entry
+            remote_id (str): the remote system-assigned id of the time off entry
+            employee_id (str): the Affix-assigned id of the individual
+            employee_remote_id (str): the remote system-assigned id of the individual
+            start_time (datetime, none_type):
+            end_time (datetime, none_type):
+            hours_worked (float):
             remote_created_at (date, none_type):
             remote_modified_at (date, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -186,20 +182,21 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.employee_id = employee_id
+        self.id = id
         self.remote_id = remote_id
-        self.balance = balance
-        self.used = used
-        self.policy_name = policy_name
-        self.policy_type = policy_type
+        self.employee_id = employee_id
+        self.employee_remote_id = employee_remote_id
+        self.start_time = start_time
+        self.end_time = end_time
+        self.hours_worked = hours_worked
         self.remote_created_at = remote_created_at
         self.remote_modified_at = remote_modified_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `affixapi-1.1.65/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.67/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.67/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.67/openapi_client/model/time_off_entry_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from openapi_client.model.policy_type_response import PolicyTypeResponse
+    globals()['PolicyTypeResponse'] = PolicyTypeResponse
+
 
 class TimeOffEntryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -84,45 +88,54 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'remote_id': (str,),  # noqa: E501
             'employee_id': (str,),  # noqa: E501
+            'employee_remote_id': (str,),  # noqa: E501
             'start_date': (date, none_type,),  # noqa: E501
             'end_date': (date, none_type,),  # noqa: E501
             'amount': (float,),  # noqa: E501
             'unit': (str,),  # noqa: E501
             'status': (str, none_type,),  # noqa: E501
             'employee_note': (str, none_type,),  # noqa: E501
-            'request_type': (str, none_type,),  # noqa: E501
+            'policy_id': (str, none_type,),  # noqa: E501
+            'policy_remote_id': (str, none_type,),  # noqa: E501
+            'policy_name': (str, none_type,),  # noqa: E501
+            'policy_type': (PolicyTypeResponse,),  # noqa: E501
             'remote_created_at': (date, none_type,),  # noqa: E501
             'remote_modified_at': (date, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'remote_id': 'remote_id',  # noqa: E501
         'employee_id': 'employee_id',  # noqa: E501
+        'employee_remote_id': 'employee_remote_id',  # noqa: E501
         'start_date': 'start_date',  # noqa: E501
         'end_date': 'end_date',  # noqa: E501
         'amount': 'amount',  # noqa: E501
         'unit': 'unit',  # noqa: E501
         'status': 'status',  # noqa: E501
         'employee_note': 'employee_note',  # noqa: E501
-        'request_type': 'request_type',  # noqa: E501
+        'policy_id': 'policy_id',  # noqa: E501
+        'policy_remote_id': 'policy_remote_id',  # noqa: E501
+        'policy_name': 'policy_name',  # noqa: E501
+        'policy_type': 'policy_type',  # noqa: E501
         'remote_created_at': 'remote_created_at',  # noqa: E501
         'remote_modified_at': 'remote_modified_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
@@ -131,28 +144,32 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, employee_id, start_date, end_date, amount, unit, status, employee_note, request_type, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, remote_id, employee_id, employee_remote_id, start_date, end_date, amount, unit, status, employee_note, policy_id, policy_remote_id, policy_name, policy_type, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
         """TimeOffEntryResponse - a model defined in OpenAPI
 
         Args:
             id (str): The Affix-assigned id of the time off entry
             remote_id (str): the remote system-assigned id of the time off entry
             employee_id (str): the Affix-assigned id of the individual
+            employee_remote_id (str): the remote system-assigned id of the individual
             start_date (date, none_type):
             end_date (date, none_type):
             amount (float):
             unit (str):
             status (str, none_type):
             employee_note (str, none_type):
-            request_type (str, none_type):
+            policy_id (str, none_type): The Affix-assigned id of the policy
+            policy_remote_id (str, none_type): The remote system-assigned id of the policy
+            policy_name (str, none_type): The name of the policy, as assigned by the remote system
+            policy_type (PolicyTypeResponse):
             remote_created_at (date, none_type):
             remote_modified_at (date, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -207,21 +224,25 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.remote_id = remote_id
         self.employee_id = employee_id
+        self.employee_remote_id = employee_remote_id
         self.start_date = start_date
         self.end_date = end_date
         self.amount = amount
         self.unit = unit
         self.status = status
         self.employee_note = employee_note
-        self.request_type = request_type
+        self.policy_id = policy_id
+        self.policy_remote_id = policy_remote_id
+        self.policy_name = policy_name
+        self.policy_type = policy_type
         self.remote_created_at = remote_created_at
         self.remote_modified_at = remote_modified_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `affixapi-1.1.65/openapi_client/model/timesheet_response.py` & `affixapi-1.1.67/openapi_client/model/time_off_balance_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from openapi_client.model.policy_type_response import PolicyTypeResponse
+    globals()['PolicyTypeResponse'] = PolicyTypeResponse
 
-class TimesheetResponse(ModelNormal):
+
+class TimeOffBalanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,17 +56,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('hours_worked',): {
-            'multiple_of': 0.1,
-        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -71,37 +72,42 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'remote_id': (str,),  # noqa: E501
             'employee_id': (str,),  # noqa: E501
-            'start_time': (datetime, none_type,),  # noqa: E501
-            'end_time': (datetime, none_type,),  # noqa: E501
-            'hours_worked': (float,),  # noqa: E501
+            'employee_remote_id': (str,),  # noqa: E501
+            'balance': (float, none_type,),  # noqa: E501
+            'used': (float, none_type,),  # noqa: E501
+            'policy_id': (str, none_type,),  # noqa: E501
+            'policy_remote_id': (str, none_type,),  # noqa: E501
+            'policy_name': (str, none_type,),  # noqa: E501
+            'policy_type': (PolicyTypeResponse,),  # noqa: E501
             'remote_created_at': (date, none_type,),  # noqa: E501
             'remote_modified_at': (date, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'remote_id': 'remote_id',  # noqa: E501
         'employee_id': 'employee_id',  # noqa: E501
-        'start_time': 'start_time',  # noqa: E501
-        'end_time': 'end_time',  # noqa: E501
-        'hours_worked': 'hours_worked',  # noqa: E501
+        'employee_remote_id': 'employee_remote_id',  # noqa: E501
+        'balance': 'balance',  # noqa: E501
+        'used': 'used',  # noqa: E501
+        'policy_id': 'policy_id',  # noqa: E501
+        'policy_remote_id': 'policy_remote_id',  # noqa: E501
+        'policy_name': 'policy_name',  # noqa: E501
+        'policy_type': 'policy_type',  # noqa: E501
         'remote_created_at': 'remote_created_at',  # noqa: E501
         'remote_modified_at': 'remote_modified_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
@@ -110,24 +116,26 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, employee_id, start_time, end_time, hours_worked, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
-        """TimesheetResponse - a model defined in OpenAPI
+    def __init__(self, employee_id, employee_remote_id, balance, used, policy_id, policy_remote_id, policy_name, policy_type, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
+        """TimeOffBalanceResponse - a model defined in OpenAPI
 
         Args:
-            id (str): The Affix-assigned id of the time off entry
-            remote_id (str): the remote system-assigned id of the time off entry
-            employee_id (str): the Affix-assigned id of the individual
-            start_time (datetime, none_type):
-            end_time (datetime, none_type):
-            hours_worked (float):
+            employee_id (str): The Affix-assigned id of the individual
+            employee_remote_id (str): the remote system-assigned id of the individual
+            balance (float, none_type):
+            used (float, none_type):
+            policy_id (str, none_type): The Affix-assigned id of the policy
+            policy_remote_id (str, none_type): The remote system-assigned id of the policy
+            policy_name (str, none_type): The name of the policy, as assigned by the remote system
+            policy_type (PolicyTypeResponse):
             remote_created_at (date, none_type):
             remote_modified_at (date, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -179,20 +187,22 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.remote_id = remote_id
         self.employee_id = employee_id
-        self.start_time = start_time
-        self.end_time = end_time
-        self.hours_worked = hours_worked
+        self.employee_remote_id = employee_remote_id
+        self.balance = balance
+        self.used = used
+        self.policy_id = policy_id
+        self.policy_remote_id = policy_remote_id
+        self.policy_name = policy_name
+        self.policy_type = policy_type
         self.remote_created_at = remote_created_at
         self.remote_modified_at = remote_modified_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `affixapi-1.1.65/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.67/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/token_request.py` & `affixapi-1.1.67/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/token_response.py` & `affixapi-1.1.67/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/tokens_response.py` & `affixapi-1.1.67/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.67/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/model_utils.py` & `affixapi-1.1.67/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/openapi_client/models/__init__.py` & `affixapi-1.1.67/openapi_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslip_response import PayslipResponse
 from openapi_client.model.payslip_response_contributions import PayslipResponseContributions
 from openapi_client.model.payslip_response_deductions import PayslipResponseDeductions
 from openapi_client.model.payslip_response_earnings import PayslipResponseEarnings
 from openapi_client.model.payslip_response_taxes import PayslipResponseTaxes
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
+from openapi_client.model.policy_type_response import PolicyTypeResponse
 from openapi_client.model.provider_request import ProviderRequest
 from openapi_client.model.provider_response import ProviderResponse
 from openapi_client.model.providers_response import ProvidersResponse
 from openapi_client.model.scopes_request import ScopesRequest
 from openapi_client.model.scopes_response import ScopesResponse
 from openapi_client.model.time_off_balance_response import TimeOffBalanceResponse
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
```

### Comparing `affixapi-1.1.65/openapi_client/rest.py` & `affixapi-1.1.67/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/setup.py` & `affixapi-1.1.67/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.65"
+VERSION = "1.1.67"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.65/test/test_2023_03_01_api.py` & `affixapi-1.1.67/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_address_no_non_null_request.py` & `affixapi-1.1.67/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_address_response.py` & `affixapi-1.1.67/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_client_request.py` & `affixapi-1.1.67/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_client_response.py` & `affixapi-1.1.67/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_companies20230301_response.py` & `affixapi-1.1.67/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_company_response.py` & `affixapi-1.1.67/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_core_api.py` & `affixapi-1.1.67/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_create_employee_request.py` & `affixapi-1.1.67/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.67/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_create_employee_request_dependents.py` & `affixapi-1.1.67/test/test_create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_create_employee_request_emergency_contacts.py` & `affixapi-1.1.67/test/test_create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_create_employee_request_manager.py` & `affixapi-1.1.67/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_currency_not_null_request.py` & `affixapi-1.1.67/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_currency_response.py` & `affixapi-1.1.67/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_disconnect_response.py` & `affixapi-1.1.67/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employee_response.py` & `affixapi-1.1.67/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employee_response_manager.py` & `affixapi-1.1.67/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employees20230301_response.py` & `affixapi-1.1.67/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.67/test/test_employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employment_response.py` & `affixapi-1.1.67/test/test_employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employment_status_not_null_not_nullable.py` & `affixapi-1.1.67/test/test_employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employment_status_not_null_request.py` & `affixapi-1.1.67/test/test_employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_employment_status_response.py` & `affixapi-1.1.67/test/test_employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_group_no_null_enum_request.py` & `affixapi-1.1.67/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_group_response.py` & `affixapi-1.1.67/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_groups20230301_response.py` & `affixapi-1.1.67/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.67/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_id_and_message_response.py` & `affixapi-1.1.67/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_identity_response.py` & `affixapi-1.1.67/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_inline_response400.py` & `affixapi-1.1.67/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_inline_response401.py` & `affixapi-1.1.67/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_inline_response409.py` & `affixapi-1.1.67/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_introspect_response.py` & `affixapi-1.1.67/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_location_no_non_null_request.py` & `affixapi-1.1.67/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_location_response.py` & `affixapi-1.1.67/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_management_api.py` & `affixapi-1.1.67/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_message_response.py` & `affixapi-1.1.67/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_mode_request.py` & `affixapi-1.1.67/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_mode_response.py` & `affixapi-1.1.67/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payrun_response.py` & `affixapi-1.1.67/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payruns20230301_response.py` & `affixapi-1.1.67/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payslip_response.py` & `affixapi-1.1.67/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payslip_response_contributions.py` & `affixapi-1.1.67/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payslip_response_deductions.py` & `affixapi-1.1.67/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payslip_response_earnings.py` & `affixapi-1.1.67/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payslip_response_taxes.py` & `affixapi-1.1.67/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_payslips20230301_response.py` & `affixapi-1.1.67/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_provider_request.py` & `affixapi-1.1.67/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_provider_response.py` & `affixapi-1.1.67/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_providers_response.py` & `affixapi-1.1.67/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_scopes_request.py` & `affixapi-1.1.67/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_scopes_response.py` & `affixapi-1.1.67/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_time_off_balance_response.py` & `affixapi-1.1.67/test/test_time_off_balance_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
+from openapi_client.model.policy_type_response import PolicyTypeResponse
+globals()['PolicyTypeResponse'] = PolicyTypeResponse
 from openapi_client.model.time_off_balance_response import TimeOffBalanceResponse
 
 
 class TestTimeOffBalanceResponse(unittest.TestCase):
     """TimeOffBalanceResponse unit test stubs"""
 
     def setUp(self):
```

### Comparing `affixapi-1.1.65/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.67/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.67/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_time_off_entry_response.py` & `affixapi-1.1.67/test/test_policy_type_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.time_off_entry_response import TimeOffEntryResponse
+from openapi_client.model.policy_type_response import PolicyTypeResponse
 
 
-class TestTimeOffEntryResponse(unittest.TestCase):
-    """TimeOffEntryResponse unit test stubs"""
+class TestPolicyTypeResponse(unittest.TestCase):
+    """PolicyTypeResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTimeOffEntryResponse(self):
-        """Test TimeOffEntryResponse"""
+    def testPolicyTypeResponse(self):
+        """Test PolicyTypeResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TimeOffEntryResponse()  # noqa: E501
+        # model = PolicyTypeResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.65/test/test_timesheet_response.py` & `affixapi-1.1.67/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_timesheets20230301_response.py` & `affixapi-1.1.67/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_token_request.py` & `affixapi-1.1.67/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_token_response.py` & `affixapi-1.1.67/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_tokens_response.py` & `affixapi-1.1.67/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_work_locations20230301_response.py` & `affixapi-1.1.67/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.65/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.67/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*


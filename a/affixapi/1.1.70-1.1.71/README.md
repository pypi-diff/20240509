# Comparing `tmp/affixapi-1.1.70.tar.gz` & `tmp/affixapi-1.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.70.tar", last modified: Thu May  9 11:46:54 2024, max compression
+gzip compressed data, was "affixapi-1.1.71.tar", last modified: Thu May  9 13:27:38 2024, max compression
```

## Comparing `affixapi-1.1.70.tar` & `affixapi-1.1.71.tar`

### file list

```diff
@@ -1,158 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.607016 affixapi-1.1.70/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 11:46:51.000000 affixapi-1.1.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-05-09 11:46:54.607016 affixapi-1.1.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-05-09 11:46:51.000000 affixapi-1.1.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.607016 affixapi-1.1.70/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-05-09 11:46:54.000000 affixapi-1.1.70/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-09 11:46:54.000000 affixapi-1.1.70/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:46:54.000000 affixapi-1.1.70/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 11:46:54.000000 affixapi-1.1.70/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 11:46:54.000000 affixapi-1.1.70/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.583016 affixapi-1.1.70/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.583016 affixapi-1.1.70/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.583016 affixapi-1.1.70/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.595016 affixapi-1.1.70/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.595016 affixapi-1.1.70/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-09 11:46:51.000000 affixapi-1.1.70/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 11:46:54.607016 affixapi-1.1.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 11:46:51.000000 affixapi-1.1.70/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:46:54.603016 affixapi-1.1.70/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-09 11:46:51.000000 affixapi-1.1.70/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.430075 affixapi-1.1.71/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 13:27:35.000000 affixapi-1.1.71/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-05-09 13:27:38.430075 affixapi-1.1.71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21795 2024-05-09 13:27:35.000000 affixapi-1.1.71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.430075 affixapi-1.1.71/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-05-09 13:27:38.000000 affixapi-1.1.71/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-09 13:27:38.000000 affixapi-1.1.71/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:27:38.000000 affixapi-1.1.71/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 13:27:38.000000 affixapi-1.1.71/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 13:27:38.000000 affixapi-1.1.71/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.406075 affixapi-1.1.71/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.406075 affixapi-1.1.71/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    55027 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55042 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.406075 affixapi-1.1.71/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.418075 affixapi-1.1.71/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17860 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24681 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16515 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/currency_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26102 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16956 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.418075 affixapi-1.1.71/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-09 13:27:35.000000 affixapi-1.1.71/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 13:27:38.430075 affixapi-1.1.71/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 13:27:35.000000 affixapi-1.1.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:27:38.430075 affixapi-1.1.71/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_currency_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-09 13:27:35.000000 affixapi-1.1.71/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.70/LICENSE` & `affixapi-1.1.71/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/PKG-INFO` & `affixapi-1.1.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.70
+Version: 1.1.71
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -353,27 +353,29 @@
 
  - [AddressNoNonNullRequest](docs/AddressNoNonNullRequest.md)
  - [AddressResponse](docs/AddressResponse.md)
  - [ClientRequest](docs/ClientRequest.md)
  - [ClientResponse](docs/ClientResponse.md)
  - [Companies20230301Response](docs/Companies20230301Response.md)
  - [CompanyResponse](docs/CompanyResponse.md)
+ - [CompensationHistoryNoNonNullRequest](docs/CompensationHistoryNoNonNullRequest.md)
+ - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
- - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
+ - [CurrencyRequest](docs/CurrencyRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
- - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
- - [EmploymentResponse](docs/EmploymentResponse.md)
+ - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
+ - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
  - [EmploymentStatusNotNullNotNullable](docs/EmploymentStatusNotNullNotNullable.md)
  - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
  - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
```

### Comparing `affixapi-1.1.70/README.md` & `affixapi-1.1.71/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -339,27 +339,29 @@
 
  - [AddressNoNonNullRequest](docs/AddressNoNonNullRequest.md)
  - [AddressResponse](docs/AddressResponse.md)
  - [ClientRequest](docs/ClientRequest.md)
  - [ClientResponse](docs/ClientResponse.md)
  - [Companies20230301Response](docs/Companies20230301Response.md)
  - [CompanyResponse](docs/CompanyResponse.md)
+ - [CompensationHistoryNoNonNullRequest](docs/CompensationHistoryNoNonNullRequest.md)
+ - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
- - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
+ - [CurrencyRequest](docs/CurrencyRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
- - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
- - [EmploymentResponse](docs/EmploymentResponse.md)
+ - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
+ - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
  - [EmploymentStatusNotNullNotNullable](docs/EmploymentStatusNotNullNotNullable.md)
  - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
  - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
```

### Comparing `affixapi-1.1.70/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.71/affixapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.70
+Version: 1.1.71
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -353,27 +353,29 @@
 
  - [AddressNoNonNullRequest](docs/AddressNoNonNullRequest.md)
  - [AddressResponse](docs/AddressResponse.md)
  - [ClientRequest](docs/ClientRequest.md)
  - [ClientResponse](docs/ClientResponse.md)
  - [Companies20230301Response](docs/Companies20230301Response.md)
  - [CompanyResponse](docs/CompanyResponse.md)
+ - [CompensationHistoryNoNonNullRequest](docs/CompensationHistoryNoNonNullRequest.md)
+ - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
- - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
+ - [CurrencyRequest](docs/CurrencyRequest.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
- - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
- - [EmploymentResponse](docs/EmploymentResponse.md)
+ - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
+ - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
  - [EmploymentStatusNotNullNotNullable](docs/EmploymentStatusNotNullNotNullable.md)
  - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
  - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
```

### Comparing `affixapi-1.1.70/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.71/affixapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,29 @@
 openapi_client/model/__init__.py
 openapi_client/model/address_no_non_null_request.py
 openapi_client/model/address_response.py
 openapi_client/model/client_request.py
 openapi_client/model/client_response.py
 openapi_client/model/companies20230301_response.py
 openapi_client/model/company_response.py
+openapi_client/model/compensation_history_no_non_null_request.py
+openapi_client/model/compensation_history_response.py
 openapi_client/model/create_employee_request.py
 openapi_client/model/create_employee_request_bank_account.py
 openapi_client/model/create_employee_request_dependents.py
 openapi_client/model/create_employee_request_emergency_contacts.py
 openapi_client/model/create_employee_request_manager.py
-openapi_client/model/currency_not_null_request.py
+openapi_client/model/currency_request.py
 openapi_client/model/currency_response.py
 openapi_client/model/disconnect_response.py
 openapi_client/model/employee_response.py
 openapi_client/model/employee_response_manager.py
 openapi_client/model/employees20230301_response.py
-openapi_client/model/employment_no_null_enum_request.py
-openapi_client/model/employment_response.py
+openapi_client/model/employment_history_no_non_null_request.py
+openapi_client/model/employment_history_response.py
 openapi_client/model/employment_status_not_null_not_nullable.py
 openapi_client/model/employment_status_not_null_request.py
 openapi_client/model/employment_status_response.py
 openapi_client/model/group_no_null_enum_request.py
 openapi_client/model/group_response.py
 openapi_client/model/groups20230301_response.py
 openapi_client/model/groups_no_null_enum_request.py
@@ -85,28 +87,30 @@
 test/test_2023_03_01_api.py
 test/test_address_no_non_null_request.py
 test/test_address_response.py
 test/test_client_request.py
 test/test_client_response.py
 test/test_companies20230301_response.py
 test/test_company_response.py
+test/test_compensation_history_no_non_null_request.py
+test/test_compensation_history_response.py
 test/test_core_api.py
 test/test_create_employee_request.py
 test/test_create_employee_request_bank_account.py
 test/test_create_employee_request_dependents.py
 test/test_create_employee_request_emergency_contacts.py
 test/test_create_employee_request_manager.py
-test/test_currency_not_null_request.py
+test/test_currency_request.py
 test/test_currency_response.py
 test/test_disconnect_response.py
 test/test_employee_response.py
 test/test_employee_response_manager.py
 test/test_employees20230301_response.py
-test/test_employment_no_null_enum_request.py
-test/test_employment_response.py
+test/test_employment_history_no_non_null_request.py
+test/test_employment_history_response.py
 test/test_employment_status_not_null_not_nullable.py
 test/test_employment_status_not_null_request.py
 test/test_employment_status_response.py
 test/test_group_no_null_enum_request.py
 test/test_group_response.py
 test/test_groups20230301_response.py
 test/test_groups_no_null_enum_request.py
```

### Comparing `affixapi-1.1.70/openapi_client/__init__.py` & `affixapi-1.1.71/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.71/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/api/core_api.py` & `affixapi-1.1.71/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/api/management_api.py` & `affixapi-1.1.71/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.71/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/api_client.py` & `affixapi-1.1.71/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/apis/__init__.py` & `affixapi-1.1.71/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/configuration.py` & `affixapi-1.1.71/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/exceptions.py` & `affixapi-1.1.71/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.71/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/address_response.py` & `affixapi-1.1.71/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/client_request.py` & `affixapi-1.1.71/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/client_response.py` & `affixapi-1.1.71/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.71/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/company_response.py` & `affixapi-1.1.71/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/create_employee_request.py` & `affixapi-1.1.71/openapi_client/model/create_employee_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,30 @@
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
     from openapi_client.model.address_no_non_null_request import AddressNoNonNullRequest
+    from openapi_client.model.compensation_history_no_non_null_request import CompensationHistoryNoNonNullRequest
     from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
     from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
     from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
     from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
-    from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
+    from openapi_client.model.employment_history_no_non_null_request import EmploymentHistoryNoNonNullRequest
     from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
     from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
     from openapi_client.model.location_no_non_null_request import LocationNoNonNullRequest
     globals()['AddressNoNonNullRequest'] = AddressNoNonNullRequest
+    globals()['CompensationHistoryNoNonNullRequest'] = CompensationHistoryNoNonNullRequest
     globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
     globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
     globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
     globals()['CreateEmployeeRequestManager'] = CreateEmployeeRequestManager
-    globals()['EmploymentNoNullEnumRequest'] = EmploymentNoNullEnumRequest
+    globals()['EmploymentHistoryNoNonNullRequest'] = EmploymentHistoryNoNonNullRequest
     globals()['EmploymentStatusNotNullRequest'] = EmploymentStatusNotNullRequest
     globals()['GroupsNoNullEnumRequest'] = GroupsNoNullEnumRequest
     globals()['LocationNoNonNullRequest'] = LocationNoNonNullRequest
 
 
 class CreateEmployeeRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
@@ -142,15 +144,16 @@
             'start_date': (date, none_type,),  # noqa: E501
             'termination_date': (date, none_type,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'home_location': (AddressNoNonNullRequest,),  # noqa: E501
             'work_location': (LocationNoNonNullRequest,),  # noqa: E501
             'manager': (CreateEmployeeRequestManager,),  # noqa: E501
             'bank_account': (CreateEmployeeRequestBankAccount,),  # noqa: E501
-            'employments': ([EmploymentNoNullEnumRequest], none_type,),  # noqa: E501
+            'employment_history': ([EmploymentHistoryNoNonNullRequest], none_type,),  # noqa: E501
+            'compensation_history': ([CompensationHistoryNoNonNullRequest], none_type,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'groups': (GroupsNoNullEnumRequest,),  # noqa: E501
             'dependents': ([CreateEmployeeRequestDependents], none_type,),  # noqa: E501
             'emergency_contacts': ([CreateEmployeeRequestEmergencyContacts], none_type,),  # noqa: E501
         }
 
     @cached_property
@@ -178,15 +181,16 @@
         'start_date': 'start_date',  # noqa: E501
         'termination_date': 'termination_date',  # noqa: E501
         'avatar': 'avatar',  # noqa: E501
         'home_location': 'home_location',  # noqa: E501
         'work_location': 'work_location',  # noqa: E501
         'manager': 'manager',  # noqa: E501
         'bank_account': 'bank_account',  # noqa: E501
-        'employments': 'employments',  # noqa: E501
+        'employment_history': 'employment_history',  # noqa: E501
+        'compensation_history': 'compensation_history',  # noqa: E501
         'custom_fields': 'custom_fields',  # noqa: E501
         'groups': 'groups',  # noqa: E501
         'dependents': 'dependents',  # noqa: E501
         'emergency_contacts': 'emergency_contacts',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -256,15 +260,16 @@
             start_date (date, none_type): [optional]  # noqa: E501
             termination_date (date, none_type): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             home_location (AddressNoNonNullRequest): [optional]  # noqa: E501
             work_location (LocationNoNonNullRequest): [optional]  # noqa: E501
             manager (CreateEmployeeRequestManager): [optional]  # noqa: E501
             bank_account (CreateEmployeeRequestBankAccount): [optional]  # noqa: E501
-            employments ([EmploymentNoNullEnumRequest], none_type): [optional]  # noqa: E501
+            employment_history ([EmploymentHistoryNoNonNullRequest], none_type): [optional]  # noqa: E501
+            compensation_history ([CompensationHistoryNoNonNullRequest], none_type): [optional]  # noqa: E501
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
             groups (GroupsNoNullEnumRequest): [optional]  # noqa: E501
             dependents ([CreateEmployeeRequestDependents], none_type): [optional]  # noqa: E501
             emergency_contacts ([CreateEmployeeRequestEmergencyContacts], none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
```

### Comparing `affixapi-1.1.70/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.71/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/create_employee_request_dependents.py` & `affixapi-1.1.71/openapi_client/model/create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/create_employee_request_emergency_contacts.py` & `affixapi-1.1.71/openapi_client/model/create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.71/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.71/openapi_client/model/currency_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class CurrencyNotNullRequest(ModelSimple):
+class CurrencyRequest(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -47,14 +47,15 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
             'None': None,
+            'NULL': "null",
             'USD': "usd",
             'GBP': "gbp",
             'EUR': "eur",
         },
     }
 
     validations = {
@@ -94,23 +95,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """CurrencyNotNullRequest - a model defined in OpenAPI
+        """CurrencyRequest - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["usd", "gbp", "eur", ]  # noqa: E501
+            args[0] (str):, must be one of ["null", "usd", "gbp", "eur", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["usd", "gbp", "eur", ]  # noqa: E501
+            value (str):, must be one of ["null", "usd", "gbp", "eur", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.70/openapi_client/model/currency_response.py` & `affixapi-1.1.71/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/disconnect_response.py` & `affixapi-1.1.71/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/employee_response.py` & `affixapi-1.1.71/openapi_client/model/employee_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,28 +25,30 @@
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
     from openapi_client.model.address_response import AddressResponse
+    from openapi_client.model.compensation_history_response import CompensationHistoryResponse
     from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
     from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
     from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
     from openapi_client.model.employee_response_manager import EmployeeResponseManager
-    from openapi_client.model.employment_response import EmploymentResponse
+    from openapi_client.model.employment_history_response import EmploymentHistoryResponse
     from openapi_client.model.employment_status_response import EmploymentStatusResponse
     from openapi_client.model.groups20230301_response import Groups20230301Response
     from openapi_client.model.location_response import LocationResponse
     globals()['AddressResponse'] = AddressResponse
+    globals()['CompensationHistoryResponse'] = CompensationHistoryResponse
     globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
     globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
     globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
     globals()['EmployeeResponseManager'] = EmployeeResponseManager
-    globals()['EmploymentResponse'] = EmploymentResponse
+    globals()['EmploymentHistoryResponse'] = EmploymentHistoryResponse
     globals()['EmploymentStatusResponse'] = EmploymentStatusResponse
     globals()['Groups20230301Response'] = Groups20230301Response
     globals()['LocationResponse'] = LocationResponse
 
 
 class EmployeeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
@@ -150,15 +152,16 @@
             'remote_created_at': (date, none_type,),  # noqa: E501
             'termination_date': (date, none_type,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'home_location': (AddressResponse,),  # noqa: E501
             'work_location': (LocationResponse,),  # noqa: E501
             'manager': (EmployeeResponseManager,),  # noqa: E501
             'bank_account': (CreateEmployeeRequestBankAccount,),  # noqa: E501
-            'employments': ([EmploymentResponse], none_type,),  # noqa: E501
+            'employment_history': ([EmploymentHistoryResponse], none_type,),  # noqa: E501
+            'compensation_history': ([CompensationHistoryResponse], none_type,),  # noqa: E501
             'custom_fields': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
             'groups': (Groups20230301Response,),  # noqa: E501
             'dependents': ([CreateEmployeeRequestDependents], none_type,),  # noqa: E501
             'emergency_contacts': ([CreateEmployeeRequestEmergencyContacts], none_type,),  # noqa: E501
         }
 
     @cached_property
@@ -189,15 +192,16 @@
         'remote_created_at': 'remote_created_at',  # noqa: E501
         'termination_date': 'termination_date',  # noqa: E501
         'avatar': 'avatar',  # noqa: E501
         'home_location': 'home_location',  # noqa: E501
         'work_location': 'work_location',  # noqa: E501
         'manager': 'manager',  # noqa: E501
         'bank_account': 'bank_account',  # noqa: E501
-        'employments': 'employments',  # noqa: E501
+        'employment_history': 'employment_history',  # noqa: E501
+        'compensation_history': 'compensation_history',  # noqa: E501
         'custom_fields': 'custom_fields',  # noqa: E501
         'groups': 'groups',  # noqa: E501
         'dependents': 'dependents',  # noqa: E501
         'emergency_contacts': 'emergency_contacts',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -208,15 +212,15 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, employee_number, first_name, last_name, display_full_name, nationality, job_title, work_email, personal_email, mobile_phone_number, tax_id, gender, ethnicity, marital_status, date_of_birth, employment_status, employment_type, start_date, remote_created_at, termination_date, avatar, home_location, work_location, manager, bank_account, employments, custom_fields, groups, dependents, emergency_contacts, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, remote_id, employee_number, first_name, last_name, display_full_name, nationality, job_title, work_email, personal_email, mobile_phone_number, tax_id, gender, ethnicity, marital_status, date_of_birth, employment_status, employment_type, start_date, remote_created_at, termination_date, avatar, home_location, work_location, manager, bank_account, employment_history, compensation_history, custom_fields, groups, dependents, emergency_contacts, *args, **kwargs):  # noqa: E501
         """EmployeeResponse - a model defined in OpenAPI
 
         Args:
             id (str): The Affix-assigned id of the individual
             remote_id (str): the remote system-assigned id of the individual
             employee_number (str, none_type):
             first_name (str): the first name of the individual
@@ -238,15 +242,16 @@
             remote_created_at (date, none_type):
             termination_date (date, none_type):
             avatar (str, none_type):
             home_location (AddressResponse):
             work_location (LocationResponse):
             manager (EmployeeResponseManager):
             bank_account (CreateEmployeeRequestBankAccount):
-            employments ([EmploymentResponse], none_type):
+            employment_history ([EmploymentHistoryResponse], none_type):
+            compensation_history ([CompensationHistoryResponse], none_type):
             custom_fields ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type):
             groups (Groups20230301Response):
             dependents ([CreateEmployeeRequestDependents], none_type):
             emergency_contacts ([CreateEmployeeRequestEmergencyContacts], none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -326,15 +331,16 @@
         self.remote_created_at = remote_created_at
         self.termination_date = termination_date
         self.avatar = avatar
         self.home_location = home_location
         self.work_location = work_location
         self.manager = manager
         self.bank_account = bank_account
-        self.employments = employments
+        self.employment_history = employment_history
+        self.compensation_history = compensation_history
         self.custom_fields = custom_fields
         self.groups = groups
         self.dependents = dependents
         self.emergency_contacts = emergency_contacts
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
```

### Comparing `affixapi-1.1.70/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.71/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.71/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.71/openapi_client/model/compensation_history_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
-    from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
-    globals()['CurrencyNotNullRequest'] = CurrencyNotNullRequest
+    from openapi_client.model.currency_response import CurrencyResponse
+    globals()['CurrencyResponse'] = CurrencyResponse
 
 
-class EmploymentNoNullEnumRequest(ModelNormal):
+class CompensationHistoryResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,21 +60,23 @@
         ('pay_frequency',): {
             'None': None,
             'WEEKLY': "weekly",
             'BIWEEKLY': "biweekly",
             'SEMIMONTHLY': "semimonthly",
             'MONTHLY': "monthly",
             'OTHER': "other",
+            'NULL': "null",
         },
         ('employment_type',): {
             'None': None,
             'FULL_TIME': "full_time",
             'PART_TIME': "part_time",
             'CONTRACTOR': "contractor",
             'OTHER': "other",
+            'NULL': "null",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -89,30 +91,28 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'job_title': (str, none_type,),  # noqa: E501
             'pay_rate': (float, none_type,),  # noqa: E501
             'pay_period': (str, none_type,),  # noqa: E501
             'pay_frequency': (str, none_type,),  # noqa: E501
             'employment_type': (str, none_type,),  # noqa: E501
-            'currency': (CurrencyNotNullRequest,),  # noqa: E501
+            'currency': (CurrencyResponse,),  # noqa: E501
             'effective_date': (date, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'job_title': 'job_title',  # noqa: E501
         'pay_rate': 'pay_rate',  # noqa: E501
         'pay_period': 'pay_period',  # noqa: E501
         'pay_frequency': 'pay_frequency',  # noqa: E501
         'employment_type': 'employment_type',  # noqa: E501
         'currency': 'currency',  # noqa: E501
         'effective_date': 'effective_date',  # noqa: E501
     }
@@ -125,24 +125,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, job_title, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, *args, **kwargs):  # noqa: E501
-        """EmploymentNoNullEnumRequest - a model defined in OpenAPI
+    def __init__(self, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, *args, **kwargs):  # noqa: E501
+        """CompensationHistoryResponse - a model defined in OpenAPI
 
         Args:
-            job_title (str, none_type):
             pay_rate (float, none_type):
             pay_period (str, none_type):
             pay_frequency (str, none_type):
             employment_type (str, none_type):
-            currency (CurrencyNotNullRequest):
+            currency (CurrencyResponse):
             effective_date (date, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -193,15 +192,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.job_title = job_title
         self.pay_rate = pay_rate
         self.pay_period = pay_period
         self.pay_frequency = pay_frequency
         self.employment_type = employment_type
         self.currency = currency
         self.effective_date = effective_date
         for var_name, var_value in kwargs.items():
```

### Comparing `affixapi-1.1.70/openapi_client/model/employment_response.py` & `affixapi-1.1.71/openapi_client/model/compensation_history_no_non_null_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
-    from openapi_client.model.currency_response import CurrencyResponse
-    globals()['CurrencyResponse'] = CurrencyResponse
+    from openapi_client.model.currency_request import CurrencyRequest
+    globals()['CurrencyRequest'] = CurrencyRequest
 
 
-class EmploymentResponse(ModelNormal):
+class CompensationHistoryNoNonNullRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,29 +54,25 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('pay_frequency',): {
-            'None': None,
             'WEEKLY': "weekly",
             'BIWEEKLY': "biweekly",
             'SEMIMONTHLY': "semimonthly",
             'MONTHLY': "monthly",
             'OTHER': "other",
-            'NULL': "null",
         },
         ('employment_type',): {
-            'None': None,
             'FULL_TIME': "full_time",
             'PART_TIME': "part_time",
             'CONTRACTOR': "contractor",
             'OTHER': "other",
-            'NULL': "null",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -91,30 +87,28 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'job_title': (str, none_type,),  # noqa: E501
-            'pay_rate': (float, none_type,),  # noqa: E501
-            'pay_period': (str, none_type,),  # noqa: E501
-            'pay_frequency': (str, none_type,),  # noqa: E501
-            'employment_type': (str, none_type,),  # noqa: E501
-            'currency': (CurrencyResponse,),  # noqa: E501
-            'effective_date': (date, none_type,),  # noqa: E501
+            'pay_rate': (float,),  # noqa: E501
+            'pay_period': (str,),  # noqa: E501
+            'pay_frequency': (str,),  # noqa: E501
+            'employment_type': (str,),  # noqa: E501
+            'currency': (CurrencyRequest,),  # noqa: E501
+            'effective_date': (date,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'job_title': 'job_title',  # noqa: E501
         'pay_rate': 'pay_rate',  # noqa: E501
         'pay_period': 'pay_period',  # noqa: E501
         'pay_frequency': 'pay_frequency',  # noqa: E501
         'employment_type': 'employment_type',  # noqa: E501
         'currency': 'currency',  # noqa: E501
         'effective_date': 'effective_date',  # noqa: E501
     }
@@ -127,25 +121,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, job_title, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, *args, **kwargs):  # noqa: E501
-        """EmploymentResponse - a model defined in OpenAPI
+    def __init__(self, pay_rate, pay_period, pay_frequency, employment_type, currency, effective_date, *args, **kwargs):  # noqa: E501
+        """CompensationHistoryNoNonNullRequest - a model defined in OpenAPI
 
         Args:
-            job_title (str, none_type):
-            pay_rate (float, none_type):
-            pay_period (str, none_type):
-            pay_frequency (str, none_type):
-            employment_type (str, none_type):
-            currency (CurrencyResponse):
-            effective_date (date, none_type):
+            pay_rate (float):
+            pay_period (str):
+            pay_frequency (str):
+            employment_type (str):
+            currency (CurrencyRequest):
+            effective_date (date):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -195,15 +188,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.job_title = job_title
         self.pay_rate = pay_rate
         self.pay_period = pay_period
         self.pay_frequency = pay_frequency
         self.employment_type = employment_type
         self.currency = currency
         self.effective_date = effective_date
         for var_name, var_value in kwargs.items():
```

### Comparing `affixapi-1.1.70/openapi_client/model/employment_status_not_null_not_nullable.py` & `affixapi-1.1.71/openapi_client/model/employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/employment_status_not_null_request.py` & `affixapi-1.1.71/openapi_client/model/employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/employment_status_response.py` & `affixapi-1.1.71/openapi_client/model/employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.71/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/group_response.py` & `affixapi-1.1.71/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.71/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.71/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.71/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/identity_response.py` & `affixapi-1.1.71/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/inline_response400.py` & `affixapi-1.1.71/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/inline_response401.py` & `affixapi-1.1.71/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/inline_response409.py` & `affixapi-1.1.71/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/introspect_response.py` & `affixapi-1.1.71/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.71/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/location_response.py` & `affixapi-1.1.71/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/message_response.py` & `affixapi-1.1.71/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/mode_request.py` & `affixapi-1.1.71/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/mode_response.py` & `affixapi-1.1.71/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payrun_response.py` & `affixapi-1.1.71/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.71/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payslip_response.py` & `affixapi-1.1.71/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.71/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.71/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.71/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.71/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.71/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/policy_type_response.py` & `affixapi-1.1.71/openapi_client/model/policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/provider_request.py` & `affixapi-1.1.71/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/provider_response.py` & `affixapi-1.1.71/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/providers_response.py` & `affixapi-1.1.71/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/scopes_request.py` & `affixapi-1.1.71/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/scopes_response.py` & `affixapi-1.1.71/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.71/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.71/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.71/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.71/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/timesheet_response.py` & `affixapi-1.1.71/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.71/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/token_request.py` & `affixapi-1.1.71/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/token_response.py` & `affixapi-1.1.71/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/tokens_response.py` & `affixapi-1.1.71/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.71/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/model_utils.py` & `affixapi-1.1.71/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/openapi_client/models/__init__.py` & `affixapi-1.1.71/openapi_client/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 
 from openapi_client.model.address_no_non_null_request import AddressNoNonNullRequest
 from openapi_client.model.address_response import AddressResponse
 from openapi_client.model.client_request import ClientRequest
 from openapi_client.model.client_response import ClientResponse
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.company_response import CompanyResponse
+from openapi_client.model.compensation_history_no_non_null_request import CompensationHistoryNoNonNullRequest
+from openapi_client.model.compensation_history_response import CompensationHistoryResponse
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
 from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
 from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
-from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
+from openapi_client.model.currency_request import CurrencyRequest
 from openapi_client.model.currency_response import CurrencyResponse
 from openapi_client.model.disconnect_response import DisconnectResponse
 from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employees20230301_response import Employees20230301Response
-from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
-from openapi_client.model.employment_response import EmploymentResponse
+from openapi_client.model.employment_history_no_non_null_request import EmploymentHistoryNoNonNullRequest
+from openapi_client.model.employment_history_response import EmploymentHistoryResponse
 from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
 from openapi_client.model.employment_status_response import EmploymentStatusResponse
 from openapi_client.model.group_no_null_enum_request import GroupNoNullEnumRequest
 from openapi_client.model.group_response import GroupResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
```

### Comparing `affixapi-1.1.70/openapi_client/rest.py` & `affixapi-1.1.71/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/setup.py` & `affixapi-1.1.71/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.70"
+VERSION = "1.1.71"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.70/test/test_2023_03_01_api.py` & `affixapi-1.1.71/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_address_no_non_null_request.py` & `affixapi-1.1.71/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_address_response.py` & `affixapi-1.1.71/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_client_request.py` & `affixapi-1.1.71/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_client_response.py` & `affixapi-1.1.71/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_companies20230301_response.py` & `affixapi-1.1.71/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_company_response.py` & `affixapi-1.1.71/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_core_api.py` & `affixapi-1.1.71/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_create_employee_request.py` & `affixapi-1.1.71/test/test_create_employee_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 
 
 import sys
 import unittest
 
 import openapi_client
 from openapi_client.model.address_no_non_null_request import AddressNoNonNullRequest
+from openapi_client.model.compensation_history_no_non_null_request import CompensationHistoryNoNonNullRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
 from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
 from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
-from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
+from openapi_client.model.employment_history_no_non_null_request import EmploymentHistoryNoNonNullRequest
 from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
 from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
 from openapi_client.model.location_no_non_null_request import LocationNoNonNullRequest
 globals()['AddressNoNonNullRequest'] = AddressNoNonNullRequest
+globals()['CompensationHistoryNoNonNullRequest'] = CompensationHistoryNoNonNullRequest
 globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
 globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
 globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
 globals()['CreateEmployeeRequestManager'] = CreateEmployeeRequestManager
-globals()['EmploymentNoNullEnumRequest'] = EmploymentNoNullEnumRequest
+globals()['EmploymentHistoryNoNonNullRequest'] = EmploymentHistoryNoNonNullRequest
 globals()['EmploymentStatusNotNullRequest'] = EmploymentStatusNotNullRequest
 globals()['GroupsNoNullEnumRequest'] = GroupsNoNullEnumRequest
 globals()['LocationNoNonNullRequest'] = LocationNoNonNullRequest
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 
 
 class TestCreateEmployeeRequest(unittest.TestCase):
```

### Comparing `affixapi-1.1.70/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.71/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_create_employee_request_dependents.py` & `affixapi-1.1.71/test/test_create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_create_employee_request_emergency_contacts.py` & `affixapi-1.1.71/test/test_create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_create_employee_request_manager.py` & `affixapi-1.1.71/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_currency_not_null_request.py` & `affixapi-1.1.71/test/test_currency_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
+from openapi_client.model.currency_request import CurrencyRequest
 
 
-class TestCurrencyNotNullRequest(unittest.TestCase):
-    """CurrencyNotNullRequest unit test stubs"""
+class TestCurrencyRequest(unittest.TestCase):
+    """CurrencyRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCurrencyNotNullRequest(self):
-        """Test CurrencyNotNullRequest"""
+    def testCurrencyRequest(self):
+        """Test CurrencyRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = CurrencyNotNullRequest()  # noqa: E501
+        # model = CurrencyRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_currency_response.py` & `affixapi-1.1.71/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_disconnect_response.py` & `affixapi-1.1.71/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_employee_response.py` & `affixapi-1.1.71/test/test_employee_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 
 
 import sys
 import unittest
 
 import openapi_client
 from openapi_client.model.address_response import AddressResponse
+from openapi_client.model.compensation_history_response import CompensationHistoryResponse
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
 from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
 from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
-from openapi_client.model.employment_response import EmploymentResponse
+from openapi_client.model.employment_history_response import EmploymentHistoryResponse
 from openapi_client.model.employment_status_response import EmploymentStatusResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.location_response import LocationResponse
 globals()['AddressResponse'] = AddressResponse
+globals()['CompensationHistoryResponse'] = CompensationHistoryResponse
 globals()['CreateEmployeeRequestBankAccount'] = CreateEmployeeRequestBankAccount
 globals()['CreateEmployeeRequestDependents'] = CreateEmployeeRequestDependents
 globals()['CreateEmployeeRequestEmergencyContacts'] = CreateEmployeeRequestEmergencyContacts
 globals()['EmployeeResponseManager'] = EmployeeResponseManager
-globals()['EmploymentResponse'] = EmploymentResponse
+globals()['EmploymentHistoryResponse'] = EmploymentHistoryResponse
 globals()['EmploymentStatusResponse'] = EmploymentStatusResponse
 globals()['Groups20230301Response'] = Groups20230301Response
 globals()['LocationResponse'] = LocationResponse
 from openapi_client.model.employee_response import EmployeeResponse
 
 
 class TestEmployeeResponse(unittest.TestCase):
```

### Comparing `affixapi-1.1.70/test/test_employee_response_manager.py` & `affixapi-1.1.71/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_employees20230301_response.py` & `affixapi-1.1.71/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.71/test/test_employment_status_not_null_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
-globals()['CurrencyNotNullRequest'] = CurrencyNotNullRequest
-from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
+from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
 
 
-class TestEmploymentNoNullEnumRequest(unittest.TestCase):
-    """EmploymentNoNullEnumRequest unit test stubs"""
+class TestEmploymentStatusNotNullRequest(unittest.TestCase):
+    """EmploymentStatusNotNullRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentNoNullEnumRequest(self):
-        """Test EmploymentNoNullEnumRequest"""
+    def testEmploymentStatusNotNullRequest(self):
+        """Test EmploymentStatusNotNullRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentNoNullEnumRequest()  # noqa: E501
+        # model = EmploymentStatusNotNullRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_employment_response.py` & `affixapi-1.1.71/test/test_compensation_history_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 import sys
 import unittest
 
 import openapi_client
 from openapi_client.model.currency_response import CurrencyResponse
 globals()['CurrencyResponse'] = CurrencyResponse
-from openapi_client.model.employment_response import EmploymentResponse
+from openapi_client.model.compensation_history_response import CompensationHistoryResponse
 
 
-class TestEmploymentResponse(unittest.TestCase):
-    """EmploymentResponse unit test stubs"""
+class TestCompensationHistoryResponse(unittest.TestCase):
+    """CompensationHistoryResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentResponse(self):
-        """Test EmploymentResponse"""
+    def testCompensationHistoryResponse(self):
+        """Test CompensationHistoryResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentResponse()  # noqa: E501
+        # model = CompensationHistoryResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_employment_status_not_null_not_nullable.py` & `affixapi-1.1.71/test/test_employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_employment_status_not_null_request.py` & `affixapi-1.1.71/test/test_employment_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
+from openapi_client.model.employment_status_response import EmploymentStatusResponse
 
 
-class TestEmploymentStatusNotNullRequest(unittest.TestCase):
-    """EmploymentStatusNotNullRequest unit test stubs"""
+class TestEmploymentStatusResponse(unittest.TestCase):
+    """EmploymentStatusResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentStatusNotNullRequest(self):
-        """Test EmploymentStatusNotNullRequest"""
+    def testEmploymentStatusResponse(self):
+        """Test EmploymentStatusResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentStatusNotNullRequest()  # noqa: E501
+        # model = EmploymentStatusResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_employment_status_response.py` & `affixapi-1.1.71/test/test_identity_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.employment_status_response import EmploymentStatusResponse
+from openapi_client.model.identity_response import IdentityResponse
 
 
-class TestEmploymentStatusResponse(unittest.TestCase):
-    """EmploymentStatusResponse unit test stubs"""
+class TestIdentityResponse(unittest.TestCase):
+    """IdentityResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentStatusResponse(self):
-        """Test EmploymentStatusResponse"""
+    def testIdentityResponse(self):
+        """Test IdentityResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentStatusResponse()  # noqa: E501
+        # model = IdentityResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_group_no_null_enum_request.py` & `affixapi-1.1.71/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_group_response.py` & `affixapi-1.1.71/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_groups20230301_response.py` & `affixapi-1.1.71/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.71/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_id_and_message_response.py` & `affixapi-1.1.71/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_identity_response.py` & `affixapi-1.1.71/test/test_providers_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.identity_response import IdentityResponse
+from openapi_client.model.providers_response import ProvidersResponse
 
 
-class TestIdentityResponse(unittest.TestCase):
-    """IdentityResponse unit test stubs"""
+class TestProvidersResponse(unittest.TestCase):
+    """ProvidersResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentityResponse(self):
-        """Test IdentityResponse"""
+    def testProvidersResponse(self):
+        """Test ProvidersResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentityResponse()  # noqa: E501
+        # model = ProvidersResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_inline_response400.py` & `affixapi-1.1.71/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_inline_response401.py` & `affixapi-1.1.71/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_inline_response409.py` & `affixapi-1.1.71/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_introspect_response.py` & `affixapi-1.1.71/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_location_no_non_null_request.py` & `affixapi-1.1.71/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_location_response.py` & `affixapi-1.1.71/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_management_api.py` & `affixapi-1.1.71/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_message_response.py` & `affixapi-1.1.71/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_mode_request.py` & `affixapi-1.1.71/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_mode_response.py` & `affixapi-1.1.71/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payrun_response.py` & `affixapi-1.1.71/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payruns20230301_response.py` & `affixapi-1.1.71/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payslip_response.py` & `affixapi-1.1.71/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payslip_response_contributions.py` & `affixapi-1.1.71/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payslip_response_deductions.py` & `affixapi-1.1.71/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payslip_response_earnings.py` & `affixapi-1.1.71/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payslip_response_taxes.py` & `affixapi-1.1.71/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_payslips20230301_response.py` & `affixapi-1.1.71/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_policy_type_response.py` & `affixapi-1.1.71/test/test_policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_provider_request.py` & `affixapi-1.1.71/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_provider_response.py` & `affixapi-1.1.71/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_providers_response.py` & `affixapi-1.1.71/test/test_tokens_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.providers_response import ProvidersResponse
+from openapi_client.model.tokens_response import TokensResponse
 
 
-class TestProvidersResponse(unittest.TestCase):
-    """ProvidersResponse unit test stubs"""
+class TestTokensResponse(unittest.TestCase):
+    """TokensResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProvidersResponse(self):
-        """Test ProvidersResponse"""
+    def testTokensResponse(self):
+        """Test TokensResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ProvidersResponse()  # noqa: E501
+        # model = TokensResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_scopes_request.py` & `affixapi-1.1.71/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_scopes_response.py` & `affixapi-1.1.71/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_time_off_balance_response.py` & `affixapi-1.1.71/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.71/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.71/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_time_off_entry_response.py` & `affixapi-1.1.71/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_timesheet_response.py` & `affixapi-1.1.71/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_timesheets20230301_response.py` & `affixapi-1.1.71/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_token_request.py` & `affixapi-1.1.71/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_token_response.py` & `affixapi-1.1.71/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_tokens_response.py` & `affixapi-1.1.71/test/test_compensation_history_no_non_null_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.tokens_response import TokensResponse
+from openapi_client.model.currency_request import CurrencyRequest
+globals()['CurrencyRequest'] = CurrencyRequest
+from openapi_client.model.compensation_history_no_non_null_request import CompensationHistoryNoNonNullRequest
 
 
-class TestTokensResponse(unittest.TestCase):
-    """TokensResponse unit test stubs"""
+class TestCompensationHistoryNoNonNullRequest(unittest.TestCase):
+    """CompensationHistoryNoNonNullRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokensResponse(self):
-        """Test TokensResponse"""
+    def testCompensationHistoryNoNonNullRequest(self):
+        """Test CompensationHistoryNoNonNullRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokensResponse()  # noqa: E501
+        # model = CompensationHistoryNoNonNullRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.70/test/test_work_locations20230301_response.py` & `affixapi-1.1.71/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.70/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.71/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*


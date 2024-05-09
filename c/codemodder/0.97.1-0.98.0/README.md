# Comparing `tmp/codemodder-0.97.1.tar.gz` & `tmp/codemodder-0.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codemodder-0.97.1.tar", last modified: Tue Apr 30 19:25:35 2024, max compression
+gzip compressed data, was "codemodder-0.98.0.tar", last modified: Thu May  9 13:49:33 2024, max compression
```

## Comparing `codemodder-0.97.1.tar` & `codemodder-0.98.0.tar`

### file list

```diff
@@ -1,530 +1,535 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.024654 codemodder-0.97.1/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-30 19:25:25.000000 codemodder-0.97.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.944654 codemodder-0.97.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/pixeebot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.948654 codemodder-0.97.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/autoformat-pixeebot-prs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/codemod_pygoat.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/deploy_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/integration_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/sonar_pixee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-30 19:25:25.000000 codemodder-0.97.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-30 19:25:25.000000 codemodder-0.97.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-30 19:25:25.000000 codemodder-0.97.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 19:25:25.000000 codemodder-0.97.1/.semgrepignore
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 19:25:25.000000 codemodder-0.97.1/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-30 19:25:25.000000 codemodder-0.97.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-30 19:25:25.000000 codemodder-0.97.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 19:25:25.000000 codemodder-0.97.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-30 19:25:25.000000 codemodder-0.97.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-30 19:25:25.000000 codemodder-0.97.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-30 19:25:25.000000 codemodder-0.97.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    44701 2024-04-30 19:25:35.024654 codemodder-0.97.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-30 19:25:25.000000 codemodder-0.97.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.948654 codemodder-0.97.1/ci_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 19:25:25.000000 codemodder-0.97.1/ci_tests/test_pygoat_findings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 19:25:25.000000 codemodder-0.97.1/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.948654 codemodder-0.97.1/img/
--rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-04-30 19:25:25.000000 codemodder-0.97.1/img/base-codemod.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-30 19:25:25.000000 codemodder-0.97.1/img/codemodder-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-30 19:25:25.000000 codemodder-0.97.1/img/codemodder-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-30 19:25:25.000000 codemodder-0.97.1/img/codemodder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.956654 codemodder-0.97.1/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.960654 codemodder-0.97.1/integration_tests/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/sonar/test_sonar_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_add_requests_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_process_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_str_concat_in_seq_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_use_defusedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 19:25:25.000000 codemodder-0.97.1/integration_tests/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-30 19:25:25.000000 codemodder-0.97.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 19:25:25.000000 codemodder-0.97.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:25:35.024654 codemodder-0.97.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.940654 codemodder-0.97.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.960654 codemodder-0.97.1/src/codemodder/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemodder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.964654 codemodder-0.97.1/src/codemodder/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/base_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/check_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/codeql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/import_modifier_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/imported_call_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/semgrep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.964654 codemodder-0.97.1/src/codemodder/codemods/test/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/test/integration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/test/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.968654 codemodder-0.97.1/src/codemodder/codemods/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/transformations/clean_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/transformations/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23960 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codemods/utils_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codeql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.968654 codemodder-0.97.1/src/codemodder/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/codemod_dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/dependency_management/setupcfg_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.968654 codemodder-0.97.1/src/codemodder/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.968654 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/package_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/project_analysis/python_repo_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/sarifs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.968654 codemodder-0.97.1/src/codemodder/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/scripts/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/scripts/get_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/semgrep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.972654 codemodder-0.97.1/src/codemodder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/utils/abc_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/utils/clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/utils/format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/utils/linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/codemodder/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.020654 codemodder-0.97.1/src/codemodder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44701 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22556 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 19:25:34.000000 codemodder-0.97.1/src/codemodder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.980654 codemodder-0.97.1/src/core_codemods/
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/add_requests_timeouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.980654 codemodder-0.97.1/src/core_codemods/api/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/api/core_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/combine_startswith_endswith.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.980654 codemodder-0.97.1/src/core_codemods/defectdojo/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/defectdojo/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/defectdojo/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.980654 codemodder-0.97.1/src/core_codemods/defectdojo/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/django_session_cookie_secure_off.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.988654 codemodder-0.97.1/src/core_codemods/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_break-or-continue-out-of-loop.md
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_exception-without-raise.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-float-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-math-isclose.md
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-mutable-params.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_flask-json-response-type.md
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_harden-pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_harden-pyyaml.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_harden-ruamel.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_https-connection.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_lazy-logging.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_limit-readline.md
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-future-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-module-global.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_requests-verify.md
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-tempfile.md
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_sql-parameterization.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_unused-imports.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_url-sandbox.md
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-defusedxml.md
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-generator.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-set-literal.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-walrus-if.md
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_async_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/lxml_safe_parser_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/process_creation_sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.988654 codemodder-0.97.1/src/core_codemods/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/refactor/refactor_new_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/requests_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/secure_cookie_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/secure_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.992654 codemodder-0.97.1/src/core_codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sonar/sonar_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    22996 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/use_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-30 19:25:25.000000 codemodder-0.97.1/src/core_codemods/with_threading_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.996654 codemodder-0.97.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.004654 codemodder-0.97.1/tests/codemods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:34.940654 codemodder-0.97.1/tests/codemods/defectdojo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.008654 codemodder-0.97.1/tests/codemods/defectdojo/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.008654 codemodder-0.97.1/tests/codemods/sonar/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/sonar/test_sonar_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_add_requests_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_async_fix_task_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_base_codemod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_base_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_combine_startswith_endswith.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_django_debug_flag_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_django_model_without_dunder_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_django_session_cookie_secure_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_enable_jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_file_resource_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_dataclass_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_deprecated_abstractproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_deprecated_logging_warn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_empty_sequence_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_hasattr_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_fix_mutable_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_flask_enable_csrf_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_harden_pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_harden_pyyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_harden_ruamel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_https_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_include_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)    23745 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_lazy_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_limit_readline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_lxml_safe_parameter_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_lxml_safe_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_order_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_process_creation_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_remove_debug_breakpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_remove_future_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_remove_module_global.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_remove_unnecessary_f_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_remove_unused_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_replace_flask_send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_request_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_secure_flask_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_secure_flask_session_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_str_concat_in_seq_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_subprocess_shell_false.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_upgrade_sslcontext_minimum_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_upgrade_sslcontext_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_url_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_use_defused_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_use_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_use_set_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_walrus_if.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/codemods/test_with_threading_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.012654 codemodder-0.97.1/tests/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/test_base_dependency_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/test_dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/test_pyproject_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/test_requirements_txt_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/test_setup_py_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/dependency_management/test_setupcfgt_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.012654 codemodder-0.97.1/tests/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.012654 codemodder-0.97.1/tests/project_analysis/file_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/file_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/project_analysis/test_python_repo_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.020654 codemodder-0.97.1/tests/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/break_or_continue_out_of_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/django_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/django_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/django_receiver_on_top.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/exception_without_raise.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/fix_assert_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/fix_float_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/fix_math_isclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/fix_missing_self_or_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/fix_sonar_sql_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/flask_json_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/flask_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/jinja2_autoescape.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/jwt_decode_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/literal_or_new_object_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/make_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/multiple_codemods.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/numpy_nan_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)  2680067 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/pygoat.semgrep.sarif.json
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/remove_assertion_in_pytest_raises.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/secure_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/semgrep.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/sonar_hotspots.json
--rw-r--r--   0 runner    (1001) docker     (127)    90652 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/sonar_issues.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/samples/webgoat_v8.2.0_codeql.sarif
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_ancestorpatterns_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_basetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_code_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_codemod_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_codemodder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_codeql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_codetf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_file_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_format_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_libcst_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_linearize_string_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_nameresolution_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_sarif_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_semgrep.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:35.020654 codemodder-0.97.1/tests/transformations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/transformations/test_clean_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/transformations/test_remove_empty_string_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 19:25:25.000000 codemodder-0.97.1/tests/transformations/test_remove_unused_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:33.001279 codemodder-0.98.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-09 13:49:21.000000 codemodder-0.98.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.897278 codemodder-0.98.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/pixeebot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.897278 codemodder-0.98.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/autoformat-pixeebot-prs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/codemod_pygoat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/deploy_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/integration_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/sonar_pixee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-09 13:49:21.000000 codemodder-0.98.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-09 13:49:21.000000 codemodder-0.98.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-09 13:49:21.000000 codemodder-0.98.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-09 13:49:21.000000 codemodder-0.98.0/.semgrepignore
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 13:49:21.000000 codemodder-0.98.0/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-09 13:49:21.000000 codemodder-0.98.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 13:49:21.000000 codemodder-0.98.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-09 13:49:21.000000 codemodder-0.98.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-09 13:49:21.000000 codemodder-0.98.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 13:49:21.000000 codemodder-0.98.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-09 13:49:21.000000 codemodder-0.98.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    44757 2024-05-09 13:49:33.001279 codemodder-0.98.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-09 13:49:21.000000 codemodder-0.98.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.897278 codemodder-0.98.0/ci_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 13:49:21.000000 codemodder-0.98.0/ci_tests/test_pygoat_findings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 13:49:21.000000 codemodder-0.98.0/codecov.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.897278 codemodder-0.98.0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    41511 2024-05-09 13:49:21.000000 codemodder-0.98.0/img/base-codemod.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-09 13:49:21.000000 codemodder-0.98.0/img/codemodder-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-09 13:49:21.000000 codemodder-0.98.0/img/codemodder-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-09 13:49:21.000000 codemodder-0.98.0/img/codemodder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.913278 codemodder-0.98.0/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.917278 codemodder-0.98.0/integration_tests/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/sonar/test_sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_add_requests_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_combine_isinstance_issubclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_process_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_str_concat_in_seq_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_use_defusedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 13:49:21.000000 codemodder-0.98.0/integration_tests/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-09 13:49:21.000000 codemodder-0.98.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 13:49:21.000000 codemodder-0.98.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:49:33.001279 codemodder-0.98.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.889278 codemodder-0.98.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.917278 codemodder-0.98.0/src/codemodder/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemodder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.921278 codemodder-0.98.0/src/codemodder/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/base_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/check_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/codeql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/import_modifier_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/imported_call_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/semgrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.925278 codemodder-0.98.0/src/codemodder/codemods/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/test/integration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/test/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.925278 codemodder-0.98.0/src/codemodder/codemods/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/transformations/clean_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/transformations/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23960 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codemods/utils_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codeql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.925278 codemodder-0.98.0/src/codemodder/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/codemod_dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/dependency_management/setupcfg_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.925278 codemodder-0.98.0/src/codemodder/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.929278 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/project_analysis/python_repo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/sarifs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.929278 codemodder-0.98.0/src/codemodder/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19831 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/scripts/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/scripts/get_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/semgrep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.929278 codemodder-0.98.0/src/codemodder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/utils/abc_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/utils/clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/utils/format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/utils/linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/codemodder/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.997279 codemodder-0.98.0/src/codemodder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44757 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22825 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:49:32.000000 codemodder-0.98.0/src/codemodder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.941278 codemodder-0.98.0/src/core_codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/add_requests_timeouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.941278 codemodder-0.98.0/src/core_codemods/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/api/core_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/combine_calls_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/combine_isinstance_issubclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/combine_startswith_endswith.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.941278 codemodder-0.98.0/src/core_codemods/defectdojo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/defectdojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/defectdojo/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.941278 codemodder-0.98.0/src/core_codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/django_session_cookie_secure_off.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.957279 codemodder-0.98.0/src/core_codemods/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_break-or-continue-out-of-loop.md
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_combine-isinstance-issubclass.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-debug-flag-on.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_exception-without-raise.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-assert-tuple.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-async-task-instantiation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-float-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-hasattr-call.md
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-math-isclose.md
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-missing-self-or-cls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_harden-ruamel.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_https-connection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_lazy-logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_limit-readline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_literal-or-new-object-identity.md
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_numpy-nan-equality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-debug-breakpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-future-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-module-global.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-unnecessary-f-str.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_requests-verify.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-tempfile.md
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_sql-parameterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_str-concat-in-sequence-literals.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_unused-imports.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_url-sandbox.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-defusedxml.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-set-literal.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-walrus-if.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_async_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/lxml_safe_parser_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/process_creation_sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.957279 codemodder-0.98.0/src/core_codemods/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/refactor/refactor_new_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/requests_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/secure_cookie_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/secure_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.961279 codemodder-0.98.0/src/core_codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sonar/sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22996 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/use_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-09 13:49:21.000000 codemodder-0.98.0/src/core_codemods/with_threading_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.965279 codemodder-0.98.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.977279 codemodder-0.98.0/tests/codemods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.893278 codemodder-0.98.0/tests/codemods/defectdojo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.977279 codemodder-0.98.0/tests/codemods/defectdojo/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.981279 codemodder-0.98.0/tests/codemods/sonar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/sonar/test_sonar_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_add_requests_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_async_fix_task_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_base_codemod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_base_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_combine_isinstance_issubclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_combine_startswith_endswith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_django_debug_flag_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_django_model_without_dunder_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_django_session_cookie_secure_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_enable_jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_file_resource_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_dataclass_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_deprecated_abstractproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_deprecated_logging_warn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_empty_sequence_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_hasattr_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_fix_mutable_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_flask_enable_csrf_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_harden_pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_harden_pyyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_harden_ruamel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_https_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_include_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23745 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_lazy_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_limit_readline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_lxml_safe_parameter_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_lxml_safe_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_order_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_process_creation_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_remove_debug_breakpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_remove_future_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_remove_module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_remove_unnecessary_f_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_remove_unused_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_replace_flask_send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_request_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_secure_flask_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_secure_flask_session_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16046 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_str_concat_in_seq_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_subprocess_shell_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_upgrade_sslcontext_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_url_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_use_defused_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_use_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_use_set_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_walrus_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/codemods/test_with_threading_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.981279 codemodder-0.98.0/tests/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/test_base_dependency_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/test_dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/test_pyproject_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/test_requirements_txt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/test_setup_py_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/dependency_management/test_setupcfgt_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.985279 codemodder-0.98.0/tests/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.985279 codemodder-0.98.0/tests/project_analysis/file_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/file_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/project_analysis/test_python_repo_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.993279 codemodder-0.98.0/tests/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/break_or_continue_out_of_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/django_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/django_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/django_receiver_on_top.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/exception_without_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/fix_assert_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/fix_float_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/fix_math_isclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/fix_missing_self_or_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/fix_sonar_sql_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/flask_json_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/flask_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/jinja2_autoescape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/jwt_decode_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/literal_or_new_object_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/make_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/multiple_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/numpy_nan_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2680067 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/pygoat.semgrep.sarif.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/remove_assertion_in_pytest_raises.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/secure_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/semgrep.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/sonar_hotspots.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90652 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/sonar_issues.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   451117 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/samples/webgoat_v8.2.0_codeql.sarif
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_ancestorpatterns_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_basetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_code_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_codemod_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_codemodder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_codeql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_codetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_file_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_format_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_libcst_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_linearize_string_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_nameresolution_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_sarif_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:32.997279 codemodder-0.98.0/tests/transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/transformations/test_clean_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/transformations/test_remove_empty_string_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-09 13:49:21.000000 codemodder-0.98.0/tests/transformations/test_remove_unused_imports.py
```

### Comparing `codemodder-0.97.1/.github/workflows/autoformat-pixeebot-prs.yaml` & `codemodder-0.98.0/.github/workflows/autoformat-pixeebot-prs.yaml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/codemod_pygoat.yml` & `codemodder-0.98.0/.github/workflows/codemod_pygoat.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/deploy_to_pypi.yml` & `codemodder-0.98.0/.github/workflows/deploy_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/integration_test.yml` & `codemodder-0.98.0/.github/workflows/integration_test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/lint.yml` & `codemodder-0.98.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/pre-commit-autoupdate.yml` & `codemodder-0.98.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/sonar_pixee.yml` & `codemodder-0.98.0/.github/workflows/sonar_pixee.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.github/workflows/test.yml` & `codemodder-0.98.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/.gitignore` & `codemodder-0.98.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
+coverage.json
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 
 # Translations
 *.mo
```

### Comparing `codemodder-0.97.1/.pre-commit-config.yaml` & `codemodder-0.98.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
          "types-jsonschema~=4.21.0",
          "types-mock==5.0.*",
          "types-PyYAML==6.0",
          "types-toml~=0.10",
          "types-requests~=2.13",
     ]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.2
+  rev: v0.4.3
   hooks:
     - id: ruff
       exclude: tests/samples/
     # todo: replace black with this?
     # Run the formatter.
     # - id: ruff-format
 - repo: https://github.com/pycqa/isort
```

### Comparing `codemodder-0.97.1/CHANGELOG.md` & `codemodder-0.98.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/CONTRIBUTING.md` & `codemodder-0.98.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/LICENSE` & `codemodder-0.98.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/Makefile` & `codemodder-0.98.0/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 PYTEST = pytest -v
-COV_FLAGS = --cov-fail-under=93.5 --cov=codemodder --cov=core_codemods
+COV_FLAGS = --cov=codemodder --cov=core_codemods
 XDIST_FLAGS = --numprocesses auto
 
 test:
-	COVERAGE_CORE=sysmon ${PYTEST} ${COV_FLAGS} tests ${XDIST_FLAGS}
+	COVERAGE_CORE=sysmon ${PYTEST} ${COV_FLAGS} tests ${XDIST_FLAGS} && coverage json && coverage-threshold
 
 integration-test:
-	${PYTEST} integration_tests ${XDIST_FLAGS}
+	COVERAGE_CORE=sysmon ${PYTEST} integration_tests --cov=core_codemods ${XDIST_FLAGS}  && coverage json && coverage-threshold --line-coverage-min 80
 
 pygoat-test:
 	${PYTEST} -v ci_tests/test_pygoat_findings.py
 
 lint:
 	ruff check  src tests integration_tests --exclude tests/samples/
```

### Comparing `codemodder-0.97.1/PKG-INFO` & `codemodder-0.98.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.97.1
+Version: 0.98.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,24 +683,25 @@
 Requires-Dist: isort<5.14,>=5.12
 Requires-Dist: libcst<1.4,>=1.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: pydantic~=2.7.0
 Requires-Dist: pylint<3.2,>=3.0
 Requires-Dist: python-json-logger~=2.0.0
 Requires-Dist: PyYAML~=6.0.0
-Requires-Dist: semgrep<1.71,>=1.50
+Requires-Dist: semgrep<1.73,>=1.50
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tomlkit~=0.12.0
 Requires-Dist: wrapt~=1.16.0
 Requires-Dist: chardet~=5.2.0
 Provides-Extra: test
 Requires-Dist: coverage<7.6,>=7.3; extra == "test"
+Requires-Dist: coverage-threshold~=0.4; extra == "test"
 Requires-Dist: Flask<4; extra == "test"
 Requires-Dist: Jinja2~=3.1.2; extra == "test"
-Requires-Dist: jsonschema~=4.21.0; extra == "test"
+Requires-Dist: jsonschema~=4.22.0; extra == "test"
 Requires-Dist: lxml<5.3.0,>=4.9.3; extra == "test"
 Requires-Dist: mock==5.1.*; extra == "test"
 Requires-Dist: pre-commit<4; extra == "test"
 Requires-Dist: Pyjwt~=2.8.0; extra == "test"
 Requires-Dist: pytest<9,>=8.2; extra == "test"
 Requires-Dist: pytest-cov<5.1,>=4.1; extra == "test"
 Requires-Dist: pytest-mock<3.15,>=3.12; extra == "test"
@@ -713,15 +714,15 @@
 Requires-Dist: numpy~=1.26.0; extra == "test"
 Requires-Dist: flask_wtf~=1.2.0; extra == "test"
 Requires-Dist: fickling>=0.1.3,~=0.1.0; extra == "test"
 Provides-Extra: complexity
 Requires-Dist: radon==6.0.*; extra == "complexity"
 Requires-Dist: xenon==0.9.*; extra == "complexity"
 Provides-Extra: openai
-Requires-Dist: openai<1.25,>=1.0; extra == "openai"
+Requires-Dist: openai<1.28,>=1.0; extra == "openai"
 Provides-Extra: all
 Requires-Dist: codemodder[test]; extra == "all"
 Requires-Dist: codemodder[complexity]; extra == "all"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="img/codemodder-dark.png">
   <source media="(prefers-color-scheme: light)" srcset="img/codemodder-light.png">
```

### Comparing `codemodder-0.97.1/README.md` & `codemodder-0.98.0/README.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/ci_tests/test_pygoat_findings.py` & `codemodder-0.98.0/ci_tests/test_pygoat_findings.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/img/base-codemod.jpg` & `codemodder-0.98.0/img/base-codemod.jpg`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/img/codemodder-dark.png` & `codemodder-0.98.0/img/codemodder-dark.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/img/codemodder-light.png` & `codemodder-0.98.0/img/codemodder-light.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/img/codemodder.png` & `codemodder-0.98.0/img/codemodder.png`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_break_or_continue_out_of_loop.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_break_or_continue_out_of_loop.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_django_jmodel_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_django_json_response_type.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_django_receiver_on_top.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_exception_without_raise.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_assert_tuple.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_float_equality.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_math_isclose.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_flask_json_response_type.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_jinja2_autoescape.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_jwt_decode_verify.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_numpy_nan_equality.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_secure_random.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_sql_parameterization.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_tempfile_mktemp.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/sonar/test_sonar_url_sandbox.py` & `codemodder-0.98.0/integration_tests/sonar/test_sonar_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_add_requests_timeout.py` & `codemodder-0.98.0/integration_tests/test_add_requests_timeout.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_break_or_continue_out_of_loop.py` & `codemodder-0.98.0/integration_tests/test_break_or_continue_out_of_loop.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_combine_startswith_endswith.py` & `codemodder-0.98.0/integration_tests/test_combine_startswith_endswith.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_dependency_manager.py` & `codemodder-0.98.0/integration_tests/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_django_debug_flag_on.py` & `codemodder-0.98.0/integration_tests/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_django_json_response_type.py` & `codemodder-0.98.0/integration_tests/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_django_model_without_dunder_str.py` & `codemodder-0.98.0/integration_tests/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_django_receiver_on_top.py` & `codemodder-0.98.0/integration_tests/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_django_session_cookie_secure_off.py` & `codemodder-0.98.0/integration_tests/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_exception_without_raise.py` & `codemodder-0.98.0/integration_tests/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_file_resource_leak.py` & `codemodder-0.98.0/integration_tests/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_assert_tuple.py` & `codemodder-0.98.0/integration_tests/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_dataclass_defaults.py` & `codemodder-0.98.0/integration_tests/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_deprecated_abstractproperty.py` & `codemodder-0.98.0/integration_tests/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_deprecated_logging_warn.py` & `codemodder-0.98.0/integration_tests/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_empty_sequence_comparison.py` & `codemodder-0.98.0/integration_tests/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_float_equality.py` & `codemodder-0.98.0/integration_tests/test_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_hasattr_call.py` & `codemodder-0.98.0/integration_tests/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_math_isclose.py` & `codemodder-0.98.0/integration_tests/test_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_missing_self_or_cls.py` & `codemodder-0.98.0/integration_tests/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_mutable_params.py` & `codemodder-0.98.0/integration_tests/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_fix_task_instantiation.py` & `codemodder-0.98.0/integration_tests/test_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_flask_enable_csrf_protection.py` & `codemodder-0.98.0/integration_tests/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_flask_json_response_type.py` & `codemodder-0.98.0/integration_tests/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_harden_pickle_load.py` & `codemodder-0.98.0/integration_tests/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_harden_pyyaml.py` & `codemodder-0.98.0/integration_tests/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_harden_ruamel.py` & `codemodder-0.98.0/integration_tests/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_https_connection.py` & `codemodder-0.98.0/integration_tests/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_jinja2_autoescape.py` & `codemodder-0.98.0/integration_tests/test_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_jwt_decode_verify.py` & `codemodder-0.98.0/integration_tests/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_lazy_logging.py` & `codemodder-0.98.0/integration_tests/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_limit_readline.py` & `codemodder-0.98.0/integration_tests/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_literal_or_new_object_identity.py` & `codemodder-0.98.0/integration_tests/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_lxml_safe_parser_defaults.py` & `codemodder-0.98.0/integration_tests/test_lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_lxml_safe_parsing.py` & `codemodder-0.98.0/integration_tests/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_multiple_codemods.py` & `codemodder-0.98.0/integration_tests/test_multiple_codemods.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_numpy_nan_equality.py` & `codemodder-0.98.0/integration_tests/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_order_imports.py` & `codemodder-0.98.0/integration_tests/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_process_sandbox.py` & `codemodder-0.98.0/integration_tests/test_process_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_program.py` & `codemodder-0.98.0/integration_tests/test_program.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.98.0/integration_tests/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_remove_debug_breakpoint.py` & `codemodder-0.98.0/integration_tests/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_remove_future_imports.py` & `codemodder-0.98.0/integration_tests/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_remove_module_global.py` & `codemodder-0.98.0/integration_tests/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_remove_unused_imports.py` & `codemodder-0.98.0/integration_tests/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_replace_flask_send_file.py` & `codemodder-0.98.0/integration_tests/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_request_verify.py` & `codemodder-0.98.0/integration_tests/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_secure_flask_cookie.py` & `codemodder-0.98.0/integration_tests/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_secure_flask_session_config.py` & `codemodder-0.98.0/integration_tests/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_secure_random.py` & `codemodder-0.98.0/integration_tests/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_sql_parameterization.py` & `codemodder-0.98.0/integration_tests/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_str_concat_in_seq_literals.py` & `codemodder-0.98.0/integration_tests/test_str_concat_in_seq_literals.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_subprocess_shell_false.py` & `codemodder-0.98.0/integration_tests/test_subprocess_shell_false.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from core_codemods.subprocess_shell_false import SubprocessShellFalse
 
 
 class TestSubprocessShellFalse(BaseIntegrationTest):
     codemod = SubprocessShellFalse
     original_code = """
     import subprocess
-    subprocess.run("echo 'hi'", shell=True)
+    subprocess.run(['ls', '-l'], shell=True)
     """
-    replacement_lines = [(2, "subprocess.run(\"echo 'hi'\", shell=False)\n")]
+    replacement_lines = [(2, "subprocess.run(['ls', '-l'], shell=False)\n")]
 
-    expected_diff = "--- \n+++ \n@@ -1,2 +1,2 @@\n import subprocess\n-subprocess.run(\"echo 'hi'\", shell=True)\n+subprocess.run(\"echo 'hi'\", shell=False)\n"
+    expected_diff = "--- \n+++ \n@@ -1,2 +1,2 @@\n import subprocess\n-subprocess.run(['ls', '-l'], shell=True)\n+subprocess.run(['ls', '-l'], shell=False)\n"
     expected_line_change = "2"
     change_description = SubprocessShellFalse.change_description
     # expected because output code points to fake file
     allowed_exceptions = (FileNotFoundError,)
```

### Comparing `codemodder-0.97.1/integration_tests/test_tempfile_mktemp.py` & `codemodder-0.98.0/integration_tests/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_unnecessary_f_str.py` & `codemodder-0.98.0/integration_tests/test_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.98.0/integration_tests/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_upgrade_sslcontext_tls.py` & `codemodder-0.98.0/integration_tests/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_url_sandbox.py` & `codemodder-0.98.0/integration_tests/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_use_defusedxml.py` & `codemodder-0.98.0/integration_tests/test_use_defusedxml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_use_generator.py` & `codemodder-0.98.0/integration_tests/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_use_set_literal.py` & `codemodder-0.98.0/integration_tests/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_use_walrus_if.py` & `codemodder-0.98.0/integration_tests/test_use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/integration_tests/test_with_threading_lock.py` & `codemodder-0.98.0/integration_tests/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/pyproject.toml` & `codemodder-0.98.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "isort>=5.12,<5.14",
     "libcst>=1.1,<1.4",
     "packaging>=23.2,<25.0",
     "pydantic~=2.7.0",
     "pylint>=3.0,<3.2",
     "python-json-logger~=2.0.0",
     "PyYAML~=6.0.0",
-    "semgrep>=1.50,<1.71",
+    "semgrep>=1.50,<1.73",
     "toml~=0.10.2",
     "tomlkit~=0.12.0",
     "wrapt~=1.16.0",
     "chardet~=5.2.0",
 ]
 keywords = ["codemod", "codemods", "security", "fix", "fixes"]
 classifiers = [
@@ -45,17 +45,18 @@
 codemodder = "codemodder.codemodder:main"
 generate-docs = 'codemodder.scripts.generate_docs:main'
 get-hashes = 'codemodder.scripts.get_hashes:main'
 
 [project.optional-dependencies]
 test = [
     "coverage>=7.3,<7.6",
+    "coverage-threshold~=0.4",
     "Flask<4",
     "Jinja2~=3.1.2",
-    "jsonschema~=4.21.0",
+    "jsonschema~=4.22.0",
     "lxml>=4.9.3,<5.3.0",
     "mock==5.1.*",
     "pre-commit<4",
     "Pyjwt~=2.8.0",
     "pytest>=8.2,<9",
     "pytest-cov>=4.1,<5.1",
     "pytest-mock>=3.12,<3.15",
@@ -70,15 +71,15 @@
     "fickling~=0.1.0,>=0.1.3",
 ]
 complexity = [
     "radon==6.0.*",
     "xenon==0.9.*",
 ]
 openai = [
-    "openai>=1.0,<1.25",
+    "openai>=1.0,<1.28",
 ]
 all = [
     "codemodder[test]",
     "codemodder[complexity]",
 ]
 
 [project.entry-points.codemods]
@@ -106,7 +107,13 @@
 [tool.black]
 extend-exclude = '''
 /(
   tests/samples |
   src/codemodder/_version.py
 )/
 '''
+
+[coverage-threshold]
+line_coverage_min = 93.5
+[coverage-threshold.modules."src/core_codemods/"]
+# Detect if a codemod is missing unit or integration tests
+file_line_coverage_min = 50
```

### Comparing `codemodder-0.97.1/src/codemodder/cli.py` & `codemodder-0.98.0/src/codemodder/cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/code_directory.py` & `codemodder-0.98.0/src/codemodder/code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemodder.py` & `codemodder-0.98.0/src/codemodder/codemodder.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/api.py` & `codemodder-0.98.0/src/codemodder/codemods/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/base_codemod.py` & `codemodder-0.98.0/src/codemodder/codemods/base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/base_transformer.py` & `codemodder-0.98.0/src/codemodder/codemods/base_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/base_visitor.py` & `codemodder-0.98.0/src/codemodder/codemods/base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/check_annotations.py` & `codemodder-0.98.0/src/codemodder/codemods/check_annotations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/codeql.py` & `codemodder-0.98.0/src/codemodder/codemods/codeql.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/import_modifier_codemod.py` & `codemodder-0.98.0/src/codemodder/codemods/import_modifier_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/imported_call_modifier.py` & `codemodder-0.98.0/src/codemodder/codemods/imported_call_modifier.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/libcst_transformer.py` & `codemodder-0.98.0/src/codemodder/codemods/libcst_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/semgrep.py` & `codemodder-0.98.0/src/codemodder/codemods/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/test/integration_utils.py` & `codemodder-0.98.0/src/codemodder/codemods/test/integration_utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/test/utils.py` & `codemodder-0.98.0/src/codemodder/codemods/test/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/test/validations.py` & `codemodder-0.98.0/src/codemodder/codemods/test/validations.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/transformations/clean_imports.py` & `codemodder-0.98.0/src/codemodder/codemods/transformations/clean_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py` & `codemodder-0.98.0/src/codemodder/codemods/transformations/remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/transformations/remove_unused_imports.py` & `codemodder-0.98.0/src/codemodder/codemods/transformations/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/utils.py` & `codemodder-0.98.0/src/codemodder/codemods/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codemods/utils_mixin.py` & `codemodder-0.98.0/src/codemodder/codemods/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/codeql.py` & `codemodder-0.98.0/src/codemodder/codeql.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 
 
 class CodeQLLocation(Location):
     @classmethod
     def from_sarif(cls, sarif_location) -> Self:
         artifact_location = sarif_location["physicalLocation"]["artifactLocation"]
         file = Path(artifact_location["uri"])
-        start = LineInfo(
-            line=sarif_location["physicalLocation"]["region"]["startLine"],
-            column=sarif_location["physicalLocation"]["region"].get("startColumn"),
-        )
+
+        try:
+            region = sarif_location["physicalLocation"]["region"]
+        except KeyError:
+            # A location without a region indicates a result for the entire file.
+            # Use sentinel values of 0 index for start/end
+            zero = LineInfo(0)
+            return cls(file=file, start=zero, end=zero)
+
+        start = LineInfo(line=region["startLine"], column=region.get("startColumn"))
         end = LineInfo(
-            line=sarif_location["physicalLocation"]["region"].get(
-                "endLine", start.line
-            ),
-            column=sarif_location["physicalLocation"]["region"].get(
-                "endColumn", start.column
-            ),
+            line=region.get("endLine", start.line),
+            column=region.get("endColumn", start.column),
         )
         return cls(file=file, start=start, end=end)
 
 
 class CodeQLResult(Result):
     @classmethod
     def from_sarif(
         cls, sarif_result, sarif_run, rule_extensions, truncate_rule_id: bool = False
     ) -> Self:
         extension_index = sarif_result["rule"]["toolComponent"]["index"]
         tool_index = sarif_result["rule"]["index"]
-
         rule_data = rule_extensions[extension_index]["rules"][tool_index]
 
         locations: list[Location] = []
         for location in sarif_result["locations"]:
             try:
                 codeql_location = CodeQLLocation.from_sarif(location)
             except KeyError:
-                # TODO: handle this case more gracefully
                 continue
 
             locations.append(codeql_location)
         return cls(rule_id=rule_data["id"], locations=locations)
 
 
 class CodeQLResultSet(ResultSet):
```

### Comparing `codemodder-0.97.1/src/codemodder/codetf.py` & `codemodder-0.98.0/src/codemodder/codetf.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     diffSide: DiffSide = DiffSide.RIGHT
     properties: Optional[dict] = None
     packageActions: Optional[list[PackageAction]] = None
     finding: Optional[Finding] = None
 
 
 class AIMetadata(BaseModel):
-    provider: str
-    model: str
-    tokens: int
+    provider: Optional[str] = None
+    model: Optional[str] = None
+    tokens: Optional[int] = None
 
 
 class ChangeSet(BaseModel):
     """A set of changes made to a file at `path`"""
 
     path: str
     diff: str
```

### Comparing `codemodder-0.97.1/src/codemodder/context.py` & `codemodder-0.98.0/src/codemodder/context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency.py` & `codemodder-0.98.0/src/codemodder/dependency.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency_management/base_dependency_writer.py` & `codemodder-0.98.0/src/codemodder/dependency_management/base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency_management/dependency_manager.py` & `codemodder-0.98.0/src/codemodder/dependency_management/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency_management/pyproject_writer.py` & `codemodder-0.98.0/src/codemodder/dependency_management/pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency_management/requirements_txt_writer.py` & `codemodder-0.98.0/src/codemodder/dependency_management/requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency_management/setup_py_writer.py` & `codemodder-0.98.0/src/codemodder/dependency_management/setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/dependency_management/setupcfg_writer.py` & `codemodder-0.98.0/src/codemodder/dependency_management/setupcfg_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/diff.py` & `codemodder-0.98.0/src/codemodder/diff.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/file_context.py` & `codemodder-0.98.0/src/codemodder/file_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/logging.py` & `codemodder-0.98.0/src/codemodder/logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/base_parser.py` & `codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/package_store.py` & `codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/package_store.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py` & `codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py` & `codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py` & `codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py` & `codemodder-0.98.0/src/codemodder/project_analysis/file_parsers/setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/project_analysis/python_repo_manager.py` & `codemodder-0.98.0/src/codemodder/project_analysis/python_repo_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/registry.py` & `codemodder-0.98.0/src/codemodder/registry.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/result.py` & `codemodder-0.98.0/src/codemodder/result.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/sarifs.py` & `codemodder-0.98.0/src/codemodder/sarifs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/scripts/generate_docs.py` & `codemodder-0.98.0/src/codemodder/scripts/generate_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         guidance_explained="Django's `SESSION_COOKIE_SECURE` flag may be overridden somewhere else or the runtime settings file may be set with the `DJANGO_SETTINGS_MODULE` environment variable. This means that the flag may intentionally be left off or missing. Also some applications may still want to support pure http. This is often the case for legacy apps.",
     ),
     "enable-jinja2-autoescape": DocMetadata(
         importance="High",
         guidance_explained="This codemod protects your applications against XSS attacks. However, it's possible you would like to set the `autoescape` parameter to a custom callable.",
     ),
     "fix-mutable-params": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="We believe that this codemod fixes an unsafe practice and that the changes themselves are safe and reliable.",
     ),
     "harden-pyyaml": DocMetadata(
         importance="Medium",
         guidance_explained="This codemod replaces any unsafe loaders with the `SafeLoader`, which is already the recommended replacement suggested in `yaml` documentation. We believe this replacement is safe and should not result in any issues.",
     ),
     "harden-ruamel": DocMetadata(
@@ -144,19 +144,19 @@
         guidance_explained="Our change fixes explicitly insecure session configuration for a Flask application. However, there may be valid cases to use these insecure configurations, such as for testing or backward compatibility.",
     ),
     "fix-file-resource-leak": DocMetadata(
         importance="High",
         guidance_explained="We believe this change is safe and will only close file resources that are not referenced outside of the with statement block.",
     ),
     "django-receiver-on-top": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="We believe this change leads to the intended behavior the application and is thus safe.",
     ),
     "numpy-nan-equality": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="We believe any use of `==` to compare with `numpy.nan` is unintended given that it is always `False`. Thus we consider this change safe.",
     ),
     "django-json-response-type": DocMetadata(
         importance="Medium",
         guidance_explained="This change will only restrict the response type and will not alter the response data itself. Thus we deem it safe.",
     ),
     "fix-deprecated-abstractproperty": DocMetadata(
@@ -188,21 +188,25 @@
         guidance_explained="We believe this change is safe and will not cause any issues.",
     ),
     "remove-module-global": DocMetadata(
         importance="Low",
         guidance_explained="Since the `global` keyword is intended for use in non-module scopes, using it at the module scope is unnecessary.",
     ),
     "remove-debug-breakpoint": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="Breakpoints are generally used only for debugging and can easily be forgotten before deploying code.",
     ),
     "combine-startswith-endswith": DocMetadata(
         importance="Low",
         guidance_explained="Simplifying expressions involving `startswith` or `endswith` calls is safe.",
     ),
+    "combine-isinstance-issubclass": DocMetadata(
+        importance="Low",
+        guidance_explained="Simplifying expressions involving `isinstance` or `issubclass` calls is safe.",
+    ),
     "fix-deprecated-logging-warn": DocMetadata(
         importance="Low",
         guidance_explained="This change fixes deprecated uses and is safe.",
     ),
     "flask-enable-csrf-protection": DocMetadata(
         importance="High",
         guidance_explained="Flask views may require proper handling of CSRF to function as expected and thus this change may break some views.",
@@ -216,23 +220,23 @@
         guidance_explained="Values compared to empty sequences should be verified in case they are falsy values that are not a sequence.",
     ),
     "remove-assertion-in-pytest-raises": DocMetadata(
         importance="Low",
         guidance_explained="We believe this change is safe and will not cause any issues.",
     ),
     "fix-assert-tuple": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="An `assert` statement on a non-empty tuple is likely unintended and should be rewritten. However, the new change may result in assertion failures that should be reviewed.",
     ),
     "lazy-logging": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="We believe this change is safe and will not cause any issues.",
     ),
     "str-concat-in-sequence-literals": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="While string concatenation inside a sequence iterable is likely a mistake, there are instances when you may choose to use them..",
     ),
     "fix-async-task-instantiation": DocMetadata(
         importance="Low",
         guidance_explained="Manual instantiation of `asyncio.Task` is discouraged. We believe this change is safe and will not cause any issues.",
     ),
     "django-model-without-dunder-str": DocMetadata(
@@ -244,27 +248,27 @@
         guidance_explained="We believe this change is safe because using `callable` is a more reliable way to check if an object is a callable.",
     ),
     "harden-pickle-load": DocMetadata(
         importance="High",
         guidance_explained="This change may impact performance in some cases, but it is recommended when handling untrusted data.",
     ),
     "fix-dataclass-defaults": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="This change is safe and will prevent runtime `ValueError`.",
     ),
     "fix-missing-self-or-cls": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="This change is safe and will prevent errors when calling on these instance or class methods..",
     ),
     "fix-float-equality": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="This change makes your code more accurate but in some cases it may be necessary to adjust the `abs_tol` and `rel_tol` parameter values for your particular calculations.",
     ),
     "fix-math-isclose": DocMetadata(
-        importance="Medium",
+        importance="Low",
         guidance_explained="This change makes your code more accurate but in some cases it may be necessary to adjust the `abs_tol` parameter value for your particular calculations.",
     ),
     "break-or-continue-out-of-loop": DocMetadata(
         importance="Low",
         guidance_explained="While this change will make the code consistent, it is likely that the `break` or `continue` statement is a symptom of an error in program logic.",
     ),
 }
```

### Comparing `codemodder-0.97.1/src/codemodder/scripts/get_hashes.py` & `codemodder-0.98.0/src/codemodder/scripts/get_hashes.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/semgrep.py` & `codemodder-0.98.0/src/codemodder/semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/utils/clean_code.py` & `codemodder-0.98.0/src/codemodder/utils/clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/utils/format_string_parser.py` & `codemodder-0.98.0/src/codemodder/utils/format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/utils/linearize_string_expression.py` & `codemodder-0.98.0/src/codemodder/utils/linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/utils/timer.py` & `codemodder-0.98.0/src/codemodder/utils/timer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder/utils/utils.py` & `codemodder-0.98.0/src/codemodder/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/codemodder.egg-info/PKG-INFO` & `codemodder-0.98.0/src/codemodder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemodder
-Version: 0.97.1
+Version: 0.98.0
 Summary: A pluggable framework for building codemods in Python
 Author-email: Pixee <python@pixee.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,24 +683,25 @@
 Requires-Dist: isort<5.14,>=5.12
 Requires-Dist: libcst<1.4,>=1.1
 Requires-Dist: packaging<25.0,>=23.2
 Requires-Dist: pydantic~=2.7.0
 Requires-Dist: pylint<3.2,>=3.0
 Requires-Dist: python-json-logger~=2.0.0
 Requires-Dist: PyYAML~=6.0.0
-Requires-Dist: semgrep<1.71,>=1.50
+Requires-Dist: semgrep<1.73,>=1.50
 Requires-Dist: toml~=0.10.2
 Requires-Dist: tomlkit~=0.12.0
 Requires-Dist: wrapt~=1.16.0
 Requires-Dist: chardet~=5.2.0
 Provides-Extra: test
 Requires-Dist: coverage<7.6,>=7.3; extra == "test"
+Requires-Dist: coverage-threshold~=0.4; extra == "test"
 Requires-Dist: Flask<4; extra == "test"
 Requires-Dist: Jinja2~=3.1.2; extra == "test"
-Requires-Dist: jsonschema~=4.21.0; extra == "test"
+Requires-Dist: jsonschema~=4.22.0; extra == "test"
 Requires-Dist: lxml<5.3.0,>=4.9.3; extra == "test"
 Requires-Dist: mock==5.1.*; extra == "test"
 Requires-Dist: pre-commit<4; extra == "test"
 Requires-Dist: Pyjwt~=2.8.0; extra == "test"
 Requires-Dist: pytest<9,>=8.2; extra == "test"
 Requires-Dist: pytest-cov<5.1,>=4.1; extra == "test"
 Requires-Dist: pytest-mock<3.15,>=3.12; extra == "test"
@@ -713,15 +714,15 @@
 Requires-Dist: numpy~=1.26.0; extra == "test"
 Requires-Dist: flask_wtf~=1.2.0; extra == "test"
 Requires-Dist: fickling>=0.1.3,~=0.1.0; extra == "test"
 Provides-Extra: complexity
 Requires-Dist: radon==6.0.*; extra == "complexity"
 Requires-Dist: xenon==0.9.*; extra == "complexity"
 Provides-Extra: openai
-Requires-Dist: openai<1.25,>=1.0; extra == "openai"
+Requires-Dist: openai<1.28,>=1.0; extra == "openai"
 Provides-Extra: all
 Requires-Dist: codemodder[test]; extra == "all"
 Requires-Dist: codemodder[complexity]; extra == "all"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="img/codemodder-dark.png">
   <source media="(prefers-color-scheme: light)" srcset="img/codemodder-light.png">
```

### Comparing `codemodder-0.97.1/src/codemodder.egg-info/SOURCES.txt` & `codemodder-0.98.0/src/codemodder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 img/codemodder-light.png
 img/codemodder.png
 integration_tests/README.md
 integration_tests/__init__.py
 integration_tests/conftest.py
 integration_tests/test_add_requests_timeout.py
 integration_tests/test_break_or_continue_out_of_loop.py
+integration_tests/test_combine_isinstance_issubclass.py
 integration_tests/test_combine_startswith_endswith.py
 integration_tests/test_dependency_manager.py
 integration_tests/test_django_debug_flag_on.py
 integration_tests/test_django_json_response_type.py
 integration_tests/test_django_model_without_dunder_str.py
 integration_tests/test_django_receiver_on_top.py
 integration_tests/test_django_session_cookie_secure_off.py
@@ -185,14 +186,16 @@
 src/codemodder/utils/format_string_parser.py
 src/codemodder/utils/linearize_string_expression.py
 src/codemodder/utils/timer.py
 src/codemodder/utils/utils.py
 src/core_codemods/__init__.py
 src/core_codemods/add_requests_timeouts.py
 src/core_codemods/break_or_continue_out_of_loop.py
+src/core_codemods/combine_calls_base.py
+src/core_codemods/combine_isinstance_issubclass.py
 src/core_codemods/combine_startswith_endswith.py
 src/core_codemods/django_debug_flag_on.py
 src/core_codemods/django_json_response_type.py
 src/core_codemods/django_model_without_dunder_str.py
 src/core_codemods/django_receiver_on_top.py
 src/core_codemods/django_session_cookie_secure_off.py
 src/core_codemods/enable_jinja2_autoescape.py
@@ -256,14 +259,15 @@
 src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py
 src/core_codemods/docs/__init__.py
 src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md
 src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md
 src/core_codemods/docs/pixee_python_add-requests-timeouts.md
 src/core_codemods/docs/pixee_python_bad-lock-with-statement.md
 src/core_codemods/docs/pixee_python_break-or-continue-out-of-loop.md
+src/core_codemods/docs/pixee_python_combine-isinstance-issubclass.md
 src/core_codemods/docs/pixee_python_combine-startswith-endswith.md
 src/core_codemods/docs/pixee_python_django-debug-flag-on.md
 src/core_codemods/docs/pixee_python_django-json-response-type.md
 src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md
 src/core_codemods/docs/pixee_python_django-receiver-on-top.md
 src/core_codemods/docs/pixee_python_django-session-cookie-secure-off.md
 src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md
@@ -364,14 +368,15 @@
 tests/codemods/__init__.py
 tests/codemods/conftest.py
 tests/codemods/test_add_requests_timeouts.py
 tests/codemods/test_async_fix_task_instantiation.py
 tests/codemods/test_base_codemod.py
 tests/codemods/test_base_visitor.py
 tests/codemods/test_break_or_continue_out_of_loop.py
+tests/codemods/test_combine_isinstance_issubclass.py
 tests/codemods/test_combine_startswith_endswith.py
 tests/codemods/test_django_debug_flag_on.py
 tests/codemods/test_django_json_response_type.py
 tests/codemods/test_django_model_without_dunder_str.py
 tests/codemods/test_django_receiver_on_top.py
 tests/codemods/test_django_session_cookie_secure_off.py
 tests/codemods/test_enable_jinja2_autoescape.py
```

### Comparing `codemodder-0.97.1/src/codemodder.egg-info/requires.txt` & `codemodder-0.98.0/src/codemodder.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 isort<5.14,>=5.12
 libcst<1.4,>=1.1
 packaging<25.0,>=23.2
 pydantic~=2.7.0
 pylint<3.2,>=3.0
 python-json-logger~=2.0.0
 PyYAML~=6.0.0
-semgrep<1.71,>=1.50
+semgrep<1.73,>=1.50
 toml~=0.10.2
 tomlkit~=0.12.0
 wrapt~=1.16.0
 chardet~=5.2.0
 
 [all]
 codemodder[test]
 codemodder[complexity]
 
 [complexity]
 radon==6.0.*
 xenon==0.9.*
 
 [openai]
-openai<1.25,>=1.0
+openai<1.28,>=1.0
 
 [test]
 coverage<7.6,>=7.3
+coverage-threshold~=0.4
 Flask<4
 Jinja2~=3.1.2
-jsonschema~=4.21.0
+jsonschema~=4.22.0
 lxml<5.3.0,>=4.9.3
 mock==5.1.*
 pre-commit<4
 Pyjwt~=2.8.0
 pytest<9,>=8.2
 pytest-cov<5.1,>=4.1
 pytest-mock<3.15,>=3.12
```

### Comparing `codemodder-0.97.1/src/core_codemods/__init__.py` & `codemodder-0.98.0/src/core_codemods/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from codemodder.registry import CodemodCollection
 
 from .add_requests_timeouts import AddRequestsTimeouts
 from .break_or_continue_out_of_loop import BreakOrContinueOutOfLoop
+from .combine_isinstance_issubclass import CombineIsinstanceIssubclass
 from .combine_startswith_endswith import CombineStartswithEndswith
 from .defectdojo.semgrep.avoid_insecure_deserialization import (
     AvoidInsecureDeserialization,
 )
 from .defectdojo.semgrep.django_secure_set_cookie import DjangoSecureSetCookie
 from .django_debug_flag_on import DjangoDebugFlagOn
 from .django_json_response_type import DjangoJsonResponseType
@@ -131,14 +132,15 @@
         DjangoJsonResponseType,
         FlaskJsonResponseType,
         ExceptionWithoutRaise,
         LiteralOrNewObjectIdentity,
         RemoveModuleGlobal,
         RemoveDebugBreakpoint,
         CombineStartswithEndswith,
+        CombineIsinstanceIssubclass,
         FixDeprecatedLoggingWarn,
         FlaskEnableCSRFProtection,
         ReplaceFlaskSendFile,
         FixEmptySequenceComparison,
         RemoveAssertionInPytestRaises,
         FixAssertTuple,
         FixFloatEquality,
```

### Comparing `codemodder-0.97.1/src/core_codemods/add_requests_timeouts.py` & `codemodder-0.98.0/src/core_codemods/add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/api/core_codemod.py` & `codemodder-0.98.0/src/core_codemods/api/core_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/break_or_continue_out_of_loop.py` & `codemodder-0.98.0/src/core_codemods/break_or_continue_out_of_loop.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/defectdojo/api.py` & `codemodder-0.98.0/src/core_codemods/defectdojo/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/defectdojo/results.py` & `codemodder-0.98.0/src/core_codemods/defectdojo/results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py` & `codemodder-0.98.0/src/core_codemods/defectdojo/semgrep/avoid_insecure_deserialization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py` & `codemodder-0.98.0/src/core_codemods/defectdojo/semgrep/django_secure_set_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/django_debug_flag_on.py` & `codemodder-0.98.0/src/core_codemods/django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/django_json_response_type.py` & `codemodder-0.98.0/src/core_codemods/django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/django_model_without_dunder_str.py` & `codemodder-0.98.0/src/core_codemods/django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/django_receiver_on_top.py` & `codemodder-0.98.0/src/core_codemods/django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/django_session_cookie_secure_off.py` & `codemodder-0.98.0/src/core_codemods/django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md` & `codemodder-0.98.0/src/core_codemods/docs/defectdojo_python_avoid-insecure-deserialization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md` & `codemodder-0.98.0/src/core_codemods/docs/defectdojo_python_django-secure-set-cookie.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-This codemod sets the most secure parameters when Django applications call `set_cookie` on a response object. Without these parameters, your Django
-application cookies may be vulnerable to being intercepted and used to gain access to sensitive data.
+This codemod sets the most secure parameters when Django applications call `set_cookie` on a response object. Without these parameters, your Django application cookies may be vulnerable to being intercepted and used to gain access to sensitive data.
 
 The changes from this codemod look like this:
 
 ```diff
  from django.shortcuts import render
  def index(request):
    resp = render(request, 'index.html')
```

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_add-requests-timeouts.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_add-requests-timeouts.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_bad-lock-with-statement.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_combine-startswith-endswith.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-json-response-type.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-model-without-dunder-str.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_django-receiver-on-top.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_django-receiver-on-top.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_enable-jinja2-autoescape.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-dataclass-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-deprecated-abstractproperty.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-deprecated-logging-warn.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-empty-sequence-comparison.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-file-resource-leak.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-float-equality.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-float-equality.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-math-isclose.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-math-isclose.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_fix-mutable-params.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_fix-mutable-params.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_flask-enable-csrf-protection.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_flask-json-response-type.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_flask-json-response-type.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_harden-pickle-load.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_harden-pickle-load.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_harden-pyyaml.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_harden-pyyaml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_harden-ruamel.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_harden-ruamel.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_jwt-decode-verify.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_jwt-decode-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_lazy-logging.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_lazy-logging.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_limit-readline.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_limit-readline.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-assertion-in-pytest-raises.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_remove-future-imports.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_remove-future-imports.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_replace-flask-send-file.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_replace-flask-send-file.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_requests-verify.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_requests-verify.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_safe-lxml-parser-defaults.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_safe-lxml-parsing.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_sandbox-process-creation.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_sandbox-process-creation.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-flask-cookie.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-flask-cookie.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-flask-session-configuration.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_secure-random.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_secure-random.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_sql-parameterization.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_sql-parameterization.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_subprocess-shell-false.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_subprocess-shell-false.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-minimum-version.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_upgrade-sslcontext-tls.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_url-sandbox.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_url-sandbox.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-defusedxml.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-defusedxml.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-generator.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-generator.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/docs/pixee_python_use-walrus-if.md` & `codemodder-0.98.0/src/core_codemods/docs/pixee_python_use-walrus-if.md`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/enable_jinja2_autoescape.py` & `codemodder-0.98.0/src/core_codemods/enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/exception_without_raise.py` & `codemodder-0.98.0/src/core_codemods/exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/file_resource_leak.py` & `codemodder-0.98.0/src/core_codemods/file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_assert_tuple.py` & `codemodder-0.98.0/src/core_codemods/fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_async_task_instantiation.py` & `codemodder-0.98.0/src/core_codemods/fix_async_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_dataclass_defaults.py` & `codemodder-0.98.0/src/core_codemods/fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_deprecated_abstractproperty.py` & `codemodder-0.98.0/src/core_codemods/fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_deprecated_logging_warn.py` & `codemodder-0.98.0/src/core_codemods/fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_empty_sequence_comparison.py` & `codemodder-0.98.0/src/core_codemods/fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_float_equality.py` & `codemodder-0.98.0/src/core_codemods/fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_hasattr_call.py` & `codemodder-0.98.0/src/core_codemods/fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_math_isclose.py` & `codemodder-0.98.0/src/core_codemods/fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_missing_self_or_cls.py` & `codemodder-0.98.0/src/core_codemods/fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/fix_mutable_params.py` & `codemodder-0.98.0/src/core_codemods/fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/flask_enable_csrf_protection.py` & `codemodder-0.98.0/src/core_codemods/flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/flask_json_response_type.py` & `codemodder-0.98.0/src/core_codemods/flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/harden_pickle_load.py` & `codemodder-0.98.0/src/core_codemods/harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/harden_pyyaml.py` & `codemodder-0.98.0/src/core_codemods/harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/harden_ruamel.py` & `codemodder-0.98.0/src/core_codemods/harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/https_connection.py` & `codemodder-0.98.0/src/core_codemods/https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/jwt_decode_verify.py` & `codemodder-0.98.0/src/core_codemods/jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/lazy_logging.py` & `codemodder-0.98.0/src/core_codemods/lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/limit_readline.py` & `codemodder-0.98.0/src/core_codemods/limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/literal_or_new_object_identity.py` & `codemodder-0.98.0/src/core_codemods/literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/lxml_safe_parser_defaults.py` & `codemodder-0.98.0/src/core_codemods/lxml_safe_parser_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/lxml_safe_parsing.py` & `codemodder-0.98.0/src/core_codemods/lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/numpy_nan_equality.py` & `codemodder-0.98.0/src/core_codemods/numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/order_imports.py` & `codemodder-0.98.0/src/core_codemods/order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/process_creation_sandbox.py` & `codemodder-0.98.0/src/core_codemods/process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/refactor/refactor_new_api.py` & `codemodder-0.98.0/src/core_codemods/refactor/refactor_new_api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/remove_assertion_in_pytest_raises.py` & `codemodder-0.98.0/src/core_codemods/remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/remove_debug_breakpoint.py` & `codemodder-0.98.0/src/core_codemods/remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/remove_future_imports.py` & `codemodder-0.98.0/src/core_codemods/remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/remove_module_global.py` & `codemodder-0.98.0/src/core_codemods/remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/remove_unnecessary_f_str.py` & `codemodder-0.98.0/src/core_codemods/remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/remove_unused_imports.py` & `codemodder-0.98.0/src/core_codemods/remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/replace_flask_send_file.py` & `codemodder-0.98.0/src/core_codemods/replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/requests_verify.py` & `codemodder-0.98.0/src/core_codemods/requests_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/secure_cookie_mixin.py` & `codemodder-0.98.0/src/core_codemods/secure_cookie_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/secure_flask_cookie.py` & `codemodder-0.98.0/src/core_codemods/secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/secure_flask_session_config.py` & `codemodder-0.98.0/src/core_codemods/secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/secure_random.py` & `codemodder-0.98.0/src/core_codemods/secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/sonar/api.py` & `codemodder-0.98.0/src/core_codemods/sonar/api.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/sonar/results.py` & `codemodder-0.98.0/src/core_codemods/sonar/results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/sonar/sonar_fix_math_isclose.py` & `codemodder-0.98.0/src/core_codemods/sonar/sonar_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/sonar/sonar_jwt_decode_verify.py` & `codemodder-0.98.0/src/core_codemods/sonar/sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/sql_parameterization.py` & `codemodder-0.98.0/src/core_codemods/sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/str_concat_in_seq_literal.py` & `codemodder-0.98.0/src/core_codemods/str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/tempfile_mktemp.py` & `codemodder-0.98.0/src/core_codemods/tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/upgrade_sslcontext_minimum_version.py` & `codemodder-0.98.0/src/core_codemods/upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/upgrade_sslcontext_tls.py` & `codemodder-0.98.0/src/core_codemods/upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/url_sandbox.py` & `codemodder-0.98.0/src/core_codemods/url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/use_defused_xml.py` & `codemodder-0.98.0/src/core_codemods/use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/use_generator.py` & `codemodder-0.98.0/src/core_codemods/use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/use_set_literal.py` & `codemodder-0.98.0/src/core_codemods/use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/use_walrus_if.py` & `codemodder-0.98.0/src/core_codemods/use_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/src/core_codemods/with_threading_lock.py` & `codemodder-0.98.0/src/core_codemods/with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py` & `codemodder-0.98.0/tests/codemods/defectdojo/semgrep/test_avoid_insecure_deserialization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py` & `codemodder-0.98.0/tests/codemods/defectdojo/semgrep/test_django_secure_set_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_break_or_continue_out_of_loop.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_break_or_continue_out_of_loop.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_django_json_response_type.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_django_receiver_on_top.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_exception_without_raise.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_assert_tuple.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_float_equality.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_math_isclose.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_flask_json_response_type.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_jwt_decode_verify.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_numpy_nan_equality.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_secure_random.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_sql_parameterization.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_tempfile_mktemp.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/sonar/test_sonar_url_sandbox.py` & `codemodder-0.98.0/tests/codemods/sonar/test_sonar_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_add_requests_timeouts.py` & `codemodder-0.98.0/tests/codemods/test_add_requests_timeouts.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_async_fix_task_instantiation.py` & `codemodder-0.98.0/tests/codemods/test_async_fix_task_instantiation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_base_codemod.py` & `codemodder-0.98.0/tests/codemods/test_base_codemod.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_base_visitor.py` & `codemodder-0.98.0/tests/codemods/test_base_visitor.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_break_or_continue_out_of_loop.py` & `codemodder-0.98.0/tests/codemods/test_break_or_continue_out_of_loop.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_django_debug_flag_on.py` & `codemodder-0.98.0/tests/codemods/test_django_debug_flag_on.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_django_json_response_type.py` & `codemodder-0.98.0/tests/codemods/test_django_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_django_model_without_dunder_str.py` & `codemodder-0.98.0/tests/codemods/test_django_model_without_dunder_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_django_receiver_on_top.py` & `codemodder-0.98.0/tests/codemods/test_django_receiver_on_top.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_django_session_cookie_secure_off.py` & `codemodder-0.98.0/tests/codemods/test_django_session_cookie_secure_off.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_enable_jinja2_autoescape.py` & `codemodder-0.98.0/tests/codemods/test_enable_jinja2_autoescape.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_exception_without_raise.py` & `codemodder-0.98.0/tests/codemods/test_exception_without_raise.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_file_resource_leak.py` & `codemodder-0.98.0/tests/codemods/test_file_resource_leak.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_assert_tuple.py` & `codemodder-0.98.0/tests/codemods/test_fix_assert_tuple.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_dataclass_defaults.py` & `codemodder-0.98.0/tests/codemods/test_fix_dataclass_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_deprecated_abstractproperty.py` & `codemodder-0.98.0/tests/codemods/test_fix_deprecated_abstractproperty.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_deprecated_logging_warn.py` & `codemodder-0.98.0/tests/codemods/test_fix_deprecated_logging_warn.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_empty_sequence_comparison.py` & `codemodder-0.98.0/tests/codemods/test_fix_empty_sequence_comparison.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_float_equality.py` & `codemodder-0.98.0/tests/codemods/test_fix_float_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_hasattr_call.py` & `codemodder-0.98.0/tests/codemods/test_fix_hasattr_call.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_math_isclose.py` & `codemodder-0.98.0/tests/codemods/test_fix_math_isclose.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_missing_self_or_cls.py` & `codemodder-0.98.0/tests/codemods/test_fix_missing_self_or_cls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_fix_mutable_params.py` & `codemodder-0.98.0/tests/codemods/test_fix_mutable_params.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_flask_enable_csrf_protection.py` & `codemodder-0.98.0/tests/codemods/test_flask_enable_csrf_protection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_flask_json_response_type.py` & `codemodder-0.98.0/tests/codemods/test_flask_json_response_type.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_harden_pickle_load.py` & `codemodder-0.98.0/tests/codemods/test_harden_pickle_load.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_harden_pyyaml.py` & `codemodder-0.98.0/tests/codemods/test_harden_pyyaml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_harden_ruamel.py` & `codemodder-0.98.0/tests/codemods/test_harden_ruamel.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_https_connection.py` & `codemodder-0.98.0/tests/codemods/test_https_connection.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_include_exclude.py` & `codemodder-0.98.0/tests/codemods/test_include_exclude.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_jwt_decode_verify.py` & `codemodder-0.98.0/tests/codemods/test_jwt_decode_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_lazy_logging.py` & `codemodder-0.98.0/tests/codemods/test_lazy_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_limit_readline.py` & `codemodder-0.98.0/tests/codemods/test_limit_readline.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_literal_or_new_object_identity.py` & `codemodder-0.98.0/tests/codemods/test_literal_or_new_object_identity.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_lxml_safe_parameter_defaults.py` & `codemodder-0.98.0/tests/codemods/test_lxml_safe_parameter_defaults.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_lxml_safe_parsing.py` & `codemodder-0.98.0/tests/codemods/test_lxml_safe_parsing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_numpy_nan_equality.py` & `codemodder-0.98.0/tests/codemods/test_numpy_nan_equality.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_order_imports.py` & `codemodder-0.98.0/tests/codemods/test_order_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_process_creation_sandbox.py` & `codemodder-0.98.0/tests/codemods/test_process_creation_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_remove_assertion_in_pytest_raises.py` & `codemodder-0.98.0/tests/codemods/test_remove_assertion_in_pytest_raises.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_remove_debug_breakpoint.py` & `codemodder-0.98.0/tests/codemods/test_remove_debug_breakpoint.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_remove_future_imports.py` & `codemodder-0.98.0/tests/codemods/test_remove_future_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_remove_module_global.py` & `codemodder-0.98.0/tests/codemods/test_remove_module_global.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_remove_unnecessary_f_str.py` & `codemodder-0.98.0/tests/codemods/test_remove_unnecessary_f_str.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_remove_unused_imports.py` & `codemodder-0.98.0/tests/codemods/test_remove_unused_imports.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_replace_flask_send_file.py` & `codemodder-0.98.0/tests/codemods/test_replace_flask_send_file.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_request_verify.py` & `codemodder-0.98.0/tests/codemods/test_request_verify.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_secure_flask_cookie.py` & `codemodder-0.98.0/tests/codemods/test_secure_flask_cookie.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_secure_flask_session_config.py` & `codemodder-0.98.0/tests/codemods/test_secure_flask_session_config.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_secure_random.py` & `codemodder-0.98.0/tests/codemods/test_secure_random.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_sql_parameterization.py` & `codemodder-0.98.0/tests/codemods/test_sql_parameterization.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_str_concat_in_seq_literal.py` & `codemodder-0.98.0/tests/codemods/test_str_concat_in_seq_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_subprocess_shell_false.py` & `codemodder-0.98.0/tests/codemods/test_subprocess_shell_false.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 
     @each_func
     def test_import(self, tmpdir, func):
         input_code = f"""
         import subprocess
         subprocess.{func}(args, shell=True)
         """
-        expexted_output = f"""
+        expected = f"""
         import subprocess
         subprocess.{func}(args, shell=False)
         """
-        self.run_and_assert(tmpdir, input_code, expexted_output)
+        self.run_and_assert(tmpdir, input_code, expected)
 
     @each_func
     def test_from_import(self, tmpdir, func):
         input_code = f"""
         from subprocess import {func}
         {func}(args, shell=True)
         """
-        expexted_output = f"""
+        expected = f"""
         from subprocess import {func}
         {func}(args, shell=False)
         """
-        self.run_and_assert(tmpdir, input_code, expexted_output)
+        self.run_and_assert(tmpdir, input_code, expected)
 
     @each_func
     def test_no_shell(self, tmpdir, func):
         input_code = f"""
         import subprocess
         subprocess.{func}(args, timeout=1)
         """
@@ -85,7 +85,23 @@
         subprocess.run(args, shell=True) # noqa: S604
         """
         expected = """
         import subprocess
         subprocess.run(args, shell=False) # noqa: S604
         """
         self.run_and_assert(tmpdir, input_code, expected)
+
+    def test_no_change_if_first_arg_is_string(self, tmpdir):
+        input_code = """
+        import subprocess
+        subprocess.run("ls -l", shell=True)
+        subprocess.run("ls" "-l", shell=True)
+        ls_args = "-l -a"
+        subprocess.run(f"ls {ls_args}", shell=True)
+        
+        subprocess.run('ls -l', shell=True)
+        subprocess.run('ls' '-l', shell=True)
+        ls_args = '-l -a'
+        subprocess.run(f'ls {ls_args}', shell=True)
+        """
+
+        self.run_and_assert(tmpdir, input_code, input_code, num_changes=0)
```

### Comparing `codemodder-0.97.1/tests/codemods/test_tempfile_mktemp.py` & `codemodder-0.98.0/tests/codemods/test_tempfile_mktemp.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_upgrade_sslcontext_minimum_version.py` & `codemodder-0.98.0/tests/codemods/test_upgrade_sslcontext_minimum_version.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_upgrade_sslcontext_tls.py` & `codemodder-0.98.0/tests/codemods/test_upgrade_sslcontext_tls.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_url_sandbox.py` & `codemodder-0.98.0/tests/codemods/test_url_sandbox.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_use_defused_xml.py` & `codemodder-0.98.0/tests/codemods/test_use_defused_xml.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_use_generator.py` & `codemodder-0.98.0/tests/codemods/test_use_generator.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_use_set_literal.py` & `codemodder-0.98.0/tests/codemods/test_use_set_literal.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_walrus_if.py` & `codemodder-0.98.0/tests/codemods/test_walrus_if.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/codemods/test_with_threading_lock.py` & `codemodder-0.98.0/tests/codemods/test_with_threading_lock.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/conftest.py` & `codemodder-0.98.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/dependency_management/test_base_dependency_writer.py` & `codemodder-0.98.0/tests/dependency_management/test_base_dependency_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/dependency_management/test_dependency_manager.py` & `codemodder-0.98.0/tests/dependency_management/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/dependency_management/test_pyproject_writer.py` & `codemodder-0.98.0/tests/dependency_management/test_pyproject_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/dependency_management/test_requirements_txt_writer.py` & `codemodder-0.98.0/tests/dependency_management/test_requirements_txt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/dependency_management/test_setup_py_writer.py` & `codemodder-0.98.0/tests/dependency_management/test_setup_py_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/dependency_management/test_setupcfgt_writer.py` & `codemodder-0.98.0/tests/dependency_management/test_setupcfgt_writer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py` & `codemodder-0.98.0/tests/project_analysis/file_parsers/test_pyproject_toml_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py` & `codemodder-0.98.0/tests/project_analysis/file_parsers/test_requirements_txt_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py` & `codemodder-0.98.0/tests/project_analysis/file_parsers/test_setup_cfg_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/project_analysis/file_parsers/test_setup_py_file_parser.py` & `codemodder-0.98.0/tests/project_analysis/file_parsers/test_setup_py_file_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/samples/pygoat.semgrep.sarif.json` & `codemodder-0.98.0/tests/samples/pygoat.semgrep.sarif.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/samples/semgrep.sarif` & `codemodder-0.98.0/tests/samples/semgrep.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/samples/sonar_hotspots.json` & `codemodder-0.98.0/tests/samples/sonar_hotspots.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/samples/sonar_issues.json` & `codemodder-0.98.0/tests/samples/sonar_issues.json`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/samples/webgoat_v8.2.0_codeql.sarif` & `codemodder-0.98.0/tests/samples/webgoat_v8.2.0_codeql.sarif`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_ancestorpatterns_mixin.py` & `codemodder-0.98.0/tests/test_ancestorpatterns_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_basetype.py` & `codemodder-0.98.0/tests/test_basetype.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_cli.py` & `codemodder-0.98.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_code_directory.py` & `codemodder-0.98.0/tests/test_code_directory.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_codemod_docs.py` & `codemodder-0.98.0/tests/test_codemod_docs.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_codemodder.py` & `codemodder-0.98.0/tests/test_codemodder.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_codetf.py` & `codemodder-0.98.0/tests/test_codetf.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_context.py` & `codemodder-0.98.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_format_string_parser.py` & `codemodder-0.98.0/tests/test_format_string_parser.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_libcst_transformer.py` & `codemodder-0.98.0/tests/test_libcst_transformer.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_linearize_string_expression.py` & `codemodder-0.98.0/tests/test_linearize_string_expression.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_logging.py` & `codemodder-0.98.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_nameresolution_mixin.py` & `codemodder-0.98.0/tests/test_nameresolution_mixin.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_registry.py` & `codemodder-0.98.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_results.py` & `codemodder-0.98.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_sarif_processing.py` & `codemodder-0.98.0/tests/test_sarif_processing.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/test_semgrep.py` & `codemodder-0.98.0/tests/test_semgrep.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/transformations/test_clean_code.py` & `codemodder-0.98.0/tests/transformations/test_clean_code.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/transformations/test_remove_empty_string_concatenation.py` & `codemodder-0.98.0/tests/transformations/test_remove_empty_string_concatenation.py`

 * *Files identical despite different names*

### Comparing `codemodder-0.97.1/tests/transformations/test_remove_unused_imports.py` & `codemodder-0.98.0/tests/transformations/test_remove_unused_imports.py`

 * *Files identical despite different names*


# Comparing `tmp/snowflake_cli_labs-2.2.0rc0.tar.gz` & `tmp/snowflake_cli_labs-2.3.0rc0.tar.gz`

## Comparing `snowflake_cli_labs-2.2.0rc0.tar` & `snowflake_cli_labs-2.3.0rc0.tar`

### file list

```diff
@@ -1,562 +1,581 @@
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0    16098 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/RELEASE-NOTES.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/SECURITY.md
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/performance_history_analysis.py
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/docs/images/coverage_5.png
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/snyk/dependency-sync.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/snyk/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/cli_global_context.py
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/config.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/constants.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/exceptions.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/feature_flags.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_path.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_utils.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/sql_execution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/alias.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/decorators.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/experimental_behaviour.py
--rw-r--r--   0        0        0    17770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/flags.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/project_initialisation.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/snow_typer.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/__init__.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/abc.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/console.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/enum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/formats.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/__init__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/plugin_config.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/__init__.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition_manager.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/errors.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/argument.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/cursor.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/error_handling.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/naming_utils.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/path_utils.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/rendering.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/__main__.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/cli_app.py
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/loggers.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/main_typer.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/printing.py
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/snow_connector.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/__init__.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/exception_logging.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/commands_structure.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/__init__.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/generator.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/__init__.py
--rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/commands.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/plugin_spec.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/__init__.py
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/commands.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/manager.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/__init__.py
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/init.py
--rw-r--r--   0        0        0    16830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py
--rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/__init__.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py
--rw-r--r--   0        0        0    13227 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/__init__.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/commands.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/common.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/plugin_spec.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/__init__.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/commands.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/render/plugin_spec.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/__init__.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/commands.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/common.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/manager.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/models.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/plugin_spec.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/venv.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/__init__.py
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
--rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/utils.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/common.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/__init__.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/__init__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/__init__.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/commands.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/manager.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/__init__.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/commands.py
--rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/diff.py
--rw-r--r--   0        0        0    11112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/manager.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/__init__.py
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/commands.py
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/manager.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/plugin_spec.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/environment.yml.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/.gitignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/common.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/functions.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/.gitignore
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/environment.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/snowflake.yml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/common/hello.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__init__.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/empty_config.toml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_cli.py
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_command_registration.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_common_decorators.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_common_global_context.py
--rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_config.py
--rw-r--r--   0        0        0    24815 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_connection.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_experimental_behaviour.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_help_messages.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_loaded_modules.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_logs.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_main.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_performance.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_project_initialisation.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_render.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_snow_connector.py
--rw-r--r--   0        0        0    10093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_sql.py
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_utils.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_zipper.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_connection.ambr
--rw-r--r--   0        0        0   529299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_help_messages.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/test_feature_flags.py
--rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/test_secure_path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__init__.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_flags.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_snow_typer.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_flags.ambr
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/__init__.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_cli_console_output.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_console_abc.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/console/test_intermediate_output.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/api/utils/test_naming_utils.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/app/test_telemetry.py
--rw-r--r--   0        0        0    17131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/git/test_git_commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/patch_utils.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_artifacts.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_commands.py
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_init.py
--rw-r--r--   0        0        0    23734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_manager.py
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_package_scripts.py
--rw-r--r--   0        0        0    43760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_run_processor.py
--rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_teardown_processor.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_utils.py
--rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_create_processor.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_drop_processor.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/utils.py
--rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_init.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_common.py
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_object.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/test_stage.py
--rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/object/__snapshots__/test_object.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_format_silent_enforcement.py
--rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_printing.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/output/test_silent_output.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_broken_plugin.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_failing_plugin.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/plugin/test_override_by_external_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/fixtures.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_config.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_definition_manager.py
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/test_util.py
--rw-r--r--   0        0        0    19709 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/project/__snapshots__/test_config.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/mocks.py
--rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_anaconda.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_build.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_common.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_function.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_models.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_package.py
--rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_procedure.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_common.py
--rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_image_repository.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_jobs.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_registry.py
--rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/test_services.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_registry.ambr
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/__init__.py
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/test_diff.py
--rw-r--r--   0        0        0    29844 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/test_stage.py
--rw-r--r--   0        0        0     7770 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/stage/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_commands.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/anaconda_channel_data.json
--rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/test_data.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/test_streamlit_requirements.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/broken_plugin_config.toml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/disabled_override_plugin_config.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/failing_plugin_config.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/configs/override_plugin_config.toml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure/core/file.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
--rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
--rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
--rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2/file.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/zendesk/file.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/empty_project/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/environment.yml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit/pages/my_page.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/main.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/environment.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/snowflake.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/package/002-shared.sql
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/snowflake.local.yml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/snowflake.yml
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/manifest.yml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/setup.sql
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/package/001-shared.sql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/package/002-shared.sql
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/minimal/snowflake.yml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/setup.sql
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/main.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/no_definition_version/snowflake.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/requirements.txt
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.zip
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/requirements.txt
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/snowflake.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/requirements.txt
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/snowflake.yml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.zip
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/environment.yml
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/snowflake.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/streamlit_full_definition/utils/utils.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/underspecified/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/unknown_fields/snowflake.yml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/another_file_with_list.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/another_file_with_single_item.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/with_list_in_source_file.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/test_data/streamlit/with_single_item.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/conversion.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/files_and_dirs.py
--rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/fixtures.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests/testing_utils/result_assertions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/conftest.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_error_handling.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_installation.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/test_snowpark_examples.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/__snapshots__/test_installation.ambr
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/config/config.toml
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_e2e/config/malformatted_config.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__init__.py
--rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/conftest.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/snowflake_connector.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_config.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_connection.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_external_plugins.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_git.py
--rw-r--r--   0        0        0    19879 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_nativeapp.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_object.py
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_package.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_session_token.py
--rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark_external_access.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_sql.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_stage.py
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_streamlit.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_temporary_connection.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_utils.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_function.ambr
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_git.ambr
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_package.ambr
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_sql.ambr
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_stage.ambr
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/config_with_enabled_all_external_plugins.toml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/config/connection_configs.toml
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/scripts/integration_account_setup.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/__init__.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_compute_pool.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_image_repository.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_jobs.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_registry.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_services.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/Dockerfile
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/bootstrap_containers_setup.sh
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/echo_service.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/spec/spec.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/spec/spec_upgrade.yml
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/sql_multi_queries.sql
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/requirements.txt
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/.gitignore
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_version_check/app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script3.sql
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_execute/script_template.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/environment.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/snowflake.yml
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/streamlit_app.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/pages/my_page.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/streamlit/utils/utils.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/naming_utils.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/snowpark_utils.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/sql_utils.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/working_directory_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_file_assertions.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/LICENSE
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/README.md
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0    16123 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/RELEASE-NOTES.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/SECURITY.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/conftest.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/performance_history_analysis.py
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/docs/images/coverage_5.png
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/scripts/main.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/snyk/dependency-sync.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/snyk/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/cli_global_context.py
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/config.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/constants.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/exceptions.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/feature_flags.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/secure_path.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/secure_utils.py
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/sql_execution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/alias.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/decorators.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/experimental_behaviour.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/flags.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/project_initialisation.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/snow_typer.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/console/__init__.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/console/abc.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/console/console.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/console/enum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/output/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/output/formats.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/output/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/plugins/__init__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/plugins/plugin_config.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/plugins/command/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/plugins/command/plugin_hook_specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/__init__.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/definition.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/definition_manager.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/errors.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/__init__.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/path_mapping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/snowpark/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/snowpark/argument.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/streamlit/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/cursor.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/error_handling.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/naming_utils.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/path_utils.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/rendering.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/types.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/__main__.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/cli_app.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/constants.py
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/loggers.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/main_typer.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/printing.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/snow_connector.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/api_impl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/api_impl/plugin/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/exception_logging.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/commands_structure.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/docs/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/docs/generator.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/docs/templates/overview.rst.jinja2
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/connection/__init__.py
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/connection/commands.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/connection/plugin_spec.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/connection/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/git/__init__.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/git/commands.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/git/manager.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/git/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/__init__.py
+-rw-r--r--   0        0        0    10568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py
+-rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/feature_flags.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/init.py
+-rw-r--r--   0        0        0    20336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/plugin_spec.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py
+-rw-r--r--   0        0        0    12493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/__init__.py
+-rw-r--r--   0        0        0     7628 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/codegen/sandbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/version/__init__.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py
+-rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/notebook/__init__.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/notebook/commands.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/notebook/manager.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/notebook/plugin_spec.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/__init__.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/commands.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/common.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/plugin_spec.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/__init__.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/commands.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/common.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/manager.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/models.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/plugin_spec.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/__init__.py
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/utils.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/common.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_registry/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_repository/__init__.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/jobs/__init__.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/services/__init__.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/sql/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/sql/commands.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/sql/manager.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/sql/plugin_spec.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/sql/snowsql_templating.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/__init__.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/commands.py
+-rw-r--r--   0        0        0    10645 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/diff.py
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/manager.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/streamlit/__init__.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/streamlit/commands.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/streamlit/manager.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/streamlit/plugin_spec.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/environment.yml.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/.gitignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/app/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/app/common.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/app/functions.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_streamlit/.gitignore
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_streamlit/environment.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_streamlit/snowflake.yml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_streamlit/common/hello.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/broken_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/commands.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/broken_plugin/src/snowflakecli/test_plugins/broken_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/failing_plugin/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/commands.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/failing_plugin/src/snowflakecli/test_plugins/failing_plugin/plugin_spec.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/__init__.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/hello_language.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/plugin_spec.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/override_build_in_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/commands.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/override_build_in_command/src/snowflakecli/test_plugins/override_build_in_command/plugin_spec.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/plugin_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/empty_config.toml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test.toml
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_cli.py
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_command_registration.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_common_decorators.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_common_global_context.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_config.py
+-rw-r--r--   0        0        0    25851 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_connection.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_experimental_behaviour.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_help_messages.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_loaded_modules.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_logs.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_main.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_performance.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_project_initialisation.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_snow_connector.py
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_sql.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_zipper.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/__snapshots__/test_connection.ambr
+-rw-r--r--   0        0        0   554299 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/__snapshots__/test_help_messages.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/__init__.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/test_feature_flags.py
+-rw-r--r--   0        0        0    17128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/test_secure_path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/commands/__init__.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/commands/test_flags.py
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/commands/test_snow_typer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/commands/__snapshots__/test_flags.ambr
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/console/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/console/test_cli_console_output.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/console/test_console_abc.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/console/test_intermediate_output.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/utils/test_naming_utils.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/api/utils/test_rendering.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/app/test_telemetry.py
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/git/test_git_commands.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/git/__snapshots__/test_git_commands.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/patch_utils.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_annotation_processor_config.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_artifacts.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_commands.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_feature_flags.py
+-rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_init.py
+-rw-r--r--   0        0        0    26124 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_manager.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_package_scripts.py
+-rw-r--r--   0        0        0    43940 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_run_processor.py
+-rw-r--r--   0        0        0    35934 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_teardown_processor.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_utils.py
+-rw-r--r--   0        0        0    22474 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_version_create_processor.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_version_drop_processor.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/utils.py
+-rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/__snapshots__/test_init.ambr
+-rw-r--r--   0        0        0    21526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/nativeapp/codegen/test_sandbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/notebook/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/notebook/test_notebook_commands.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/notebook/test_notebook_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/object/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/object/test_common.py
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/object/test_object.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/object/test_stage.py
+-rw-r--r--   0        0        0     9313 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/object/__snapshots__/test_object.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/output/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/output/test_format_silent_enforcement.py
+-rw-r--r--   0        0        0     9704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/output/test_printing.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/output/test_silent_output.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/plugin/test_broken_plugin.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/plugin/test_failing_plugin.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/plugin/test_override_by_external_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/fixtures.py
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/test_config.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/test_definition_manager.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/test_project_schemas.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/test_util.py
+-rw-r--r--   0        0        0    19829 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/project/__snapshots__/test_config.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/mocks.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_anaconda.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_build.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_common.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_function.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_models.py
+-rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_package.py
+-rw-r--r--   0        0        0    14097 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_procedure.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_procedure_coverage.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/test_common.py
+-rw-r--r--   0        0        0    16282 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     9321 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/test_image_repository.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/test_jobs.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/test_registry.py
+-rw-r--r--   0        0        0    22547 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/test_services.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/spcs/__snapshots__/test_registry.ambr
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/stage/__init__.py
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/stage/test_diff.py
+-rw-r--r--   0        0        0    30692 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/stage/test_stage.py
+-rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/stage/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/streamlit/test_commands.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/streamlit/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/anaconda_channel_data.json
+-rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/test_data.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/test_streamlit_requirements.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/configs/broken_plugin_config.toml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/configs/disabled_override_plugin_config.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/configs/failing_plugin_config.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/configs/override_plugin_config.toml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure/core/file.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure/eventhub/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    36617 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE
+-rw-r--r--   0        0        0    66103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA
+-rw-r--r--   0        0        0    17195 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/REQUESTED
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/WHEEL
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2/file.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/zendesk/file.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/empty_project/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit/environment.yml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_defaults/main.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_defaults/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_environment.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_defaults/streamlit_pages/first_page.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_stage/environment.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_stage/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_stage/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/example_streamlit_no_stage/pages/my_page.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/snowflake.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/package/002-shared.sql
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/snowflake.local.yml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/snowflake.yml
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/app/README.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/app/manifest.yml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/app/setup.sql
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/package/001-shared.sql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/package/002-shared.sql
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/minimal/snowflake.yml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/setup.sql
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_1/app/streamlit/main.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/001-shared.sql
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/002-shared.sql
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/setup.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.local.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/snowflake.yml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/README.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/config.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_project_with_pkg_warehouse/app/streamlit/main.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/napp_with_annotation_processor/snowflake.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/no_definition_version/snowflake.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_external_access/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_external_access/requirements.txt
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_external_access/snowflake.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_functions/app.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_functions/app.zip
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_functions/requirements.txt
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_functions/snowflake.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_external_access/requirements.txt
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_external_access/snowflake.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures/app.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures/requirements.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures/snowflake.yml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.zip
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures_coverage/requirements.txt
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures_coverage/snowflake.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/streamlit_full_definition/environment.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/streamlit_full_definition/snowflake.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/streamlit_full_definition/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/streamlit_full_definition/pages/my_page.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/streamlit_full_definition/utils/utils.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/underspecified/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/unknown_fields/snowflake.yml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/streamlit/another_file_with_list.yml
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/streamlit/another_file_with_single_item.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/streamlit/with_list_in_source_file.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/test_data/streamlit/with_single_item.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/testing_utils/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/testing_utils/conversion.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/testing_utils/files_and_dirs.py
+-rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/testing_utils/fixtures.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests/testing_utils/result_assertions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/conftest.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/test_error_handling.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/test_installation.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/test_snowpark_examples.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/__snapshots__/test_installation.ambr
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/config/config.toml
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_e2e/config/malformatted_config.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/__init__.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/conftest.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/snowflake_connector.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_config.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_connection.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_external_plugins.py
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_git.py
+-rw-r--r--   0        0        0    30602 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_nativeapp.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_notebooks.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_object.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_package.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_session_token.py
+-rw-r--r--   0        0        0    28873 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_snowpark.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_snowpark_external_access.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_sql.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_stage.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_streamlit.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_temporary_connection.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_utils.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_function.ambr
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_git.ambr
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_package.ambr
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_sql.ambr
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_stage.ambr
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/config/config_with_enabled_all_external_plugins.toml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/config/config_with_enabled_only_one_external_plugin.toml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/config/connection_configs.toml
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/scripts/integration_account_setup.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/__init__.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_compute_pool.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_image_repository.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_jobs.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_registry.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_services.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/docker/Dockerfile
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/docker/bootstrap_containers_setup.sh
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/docker/echo_service.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/spec/spec.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/spec/spec_upgrade.yml
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/sql_multi_queries.sql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark/requirements.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/requirements.txt
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_external_access/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_external_access/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/requirements.txt
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_vectorized/.gitignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_vectorized/requirements.txt
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_vectorized/snowflake.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_vectorized/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_version_check/.gitignore
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_version_check/requirements.txt
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_version_check/snowflake.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_version_check/app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.other.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/requirements.txt
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/app/app.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_import/.gitignore
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_import/requirements.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_import/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_import/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/.gitignore
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_no_other_deps/app/functions.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/.gitignore
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/requirements.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/snowflake.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_single_requirements_having_transient_deps/app/functions.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_execute/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_execute/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_execute/script3.sql
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_execute/script_template.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/script1.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/script2.sql
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/stage_get_directory_structure/dir/subdir/script3.sql
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/streamlit/environment.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/streamlit/snowflake.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/streamlit/streamlit_app.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/streamlit/pages/my_page.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/streamlit/utils/utils.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/naming_utils.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/snowpark_utils.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/sql_utils.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/working_directory_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/assertions/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/assertions/test_file_assertions.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/LICENSE
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/README.md
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    16880 2020-02-02 00:00:00.000000 snowflake_cli_labs-2.3.0rc0/PKG-INFO
```

### Comparing `snowflake_cli_labs-2.2.0rc0/.pre-commit-config.yaml` & `snowflake_cli_labs-2.3.0rc0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         files: ^src/snowflake/cli/api/.*\.py$
       - id: avoid-snowcli
         language: pygrep
         name: "Prefer snowflake CLI over snowcli"
         entry: "snowcli"
         pass_filenames: true
         files: ^src/.*\.py$
-        exclude: ^src/snowflake/cli/app/telemetry.py$
+        exclude: ^src/snowflake/cli/app/constants.py$
       - id: dependencies-sync
         name: "Copy dependencies from pyproject.toml to requirements.txt"
         language: system
         entry: python snyk/dependency-sync.py
         files: ^pyproject.toml$
       - id: use-local-requirements-model
         language: pygrep
```

### Comparing `snowflake_cli_labs-2.2.0rc0/CONTRIBUTING.md` & `snowflake_cli_labs-2.3.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/RELEASE-NOTES.md` & `snowflake_cli_labs-2.3.0rc0/RELEASE-NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,57 @@
+# Unreleased version
+## Backward incompatibility
+
+## Deprecations
+
+## New additions
+
+## Fixes and improvements
+
+
+# v2.3.0
+
+## Backward incompatibility
+
+## Deprecations
+
+## New additions
+* `snow sql` command supports now client-side templating of queries
+* New `snow sql` functionality:
+  * `-D/--data` allows variable substitutions in a SQL input (client-side query templating)
+* New `snow app deploy` functionality:
+  * Passing files and directories as arguments syncs these only: `snow app deploy some-file some-dir`.
+  * `--recursive` syncs all files and subdirectories recursively.
+  * `--prune` deletes specified files from the stage if they don't exist locally.
+
+## Fixes and improvements
+* More human-friendly errors in case of corrupted `config.toml` file.
+* Fixed a bug in `snow app` that caused files to be re-uploaded unnecessarily.
+* Optimize snowpark dependency search to lower the size of .zip artifacts and
+  the number of anaconda dependencies for snowpark projects.
+* Added support for fully qualified stage names in stage and git execute commands.
+* Fixed a bug where `snow app run` was not upgrading the application when the local state and remote stage are identical (for example immediately after `snow app deploy`).
+* Fixed handling of stage path separators on Windows
+* The `--info` callback returns info about configured feature flags.
+
 # v2.2.0
 
 ## Backward incompatibility
 
 ## Deprecations
 * `snow snowpark package lookup` no longer performs check against PyPi. Using `--pypi-download` or `--yes`
   has no effect and will cause a warning. In this way the command has single responsibility - check if package is
   available in Snowflake Anaconda channel.
 * `snow snowpark package create`:
   * `--pypi-download` or `--yes` flags are deprecated, have no effect and will cause a warning.
     `create` command always checks against PyPi.
   * `--allow-native-libraries` is deprecated in favour of boolean flag `--allow-shared-libraries`.
     Using old flag will cause a warning.
 * `snow snowpark build`:
-  * `--pypi-download` flag is deprecated, have no effect and will cause a warning. Create command always check against PyPi.
+  * `--pypi-download` flag is deprecated, have no effect and will cause a warning. Build command always check against PyPi.
   * `--check-anaconda-for-pypi-depts` is deprecated and using it will cause warning, the functionality is replaced by `--ignore-anaconda`
   * `--package-native-libraries` is deprecated and using it will cause warning, the functionality is replaced by `--allow-shared-libraries`
 * `snow object stage` commands are deprecated and using them will cause a warning.
    Functionality is replaced by `snow stage` commands.
 
 ## New additions
 * Added support for fully qualified name (`database.schema.name`) in `name` parameter in streamlit project definition
@@ -33,15 +68,15 @@
 * `snow snowpark build`:
   * new `--skip-version-check` skips comparing versions of dependencies between requirements and Anaconda.
   * new `--index-url` flag sets up Base URL of the Python Package Index to use for package lookup.
 * Added `--recursive` flag for copy from stage, it will reproduce the directory structure locally.
 * Added support for snowgit. New commands:
   * `snow git setup` - wizard setting up a git repository stage and creating all necessary objects
   * `snow git fetch` - fetches latest changes from the origin repository into Snowflake repository
-  * `snow git list-brahces` - lists all branches in the repository
+  * `snow git list-branches` - lists all branches in the repository
   * `snow git list-tags` - lists all tags in the repository
   * `snow git list-files` - lists all files on provided branch/tag/commit
   * `snow git copy` - copies files from provided branch/tag/commit into stage or local directory
   * `snow git execute` - execute immediate files from repository
 * Added command for execute immediate `snow object stage execute`
 * Fetching available packages list from Snowflake instead of directly from Anaconda with fallback to the old method (for backward compatibility).
   As the new method requires a connection to Snowflake, it adds connection options to the following commands:
@@ -50,22 +85,23 @@
   * `snow snowpark package create`
 
 ## Fixes and improvements
 * Adding `--image-name` option for image name argument in `spcs image-repository list-tags` for consistency with other commands.
 * Fixed errors during `spcs image-registry login` not being formatted correctly.
 * Project definition no longer accept extra fields. Any extra field will cause an error.
 * Changing imports in function/procedure section in `snowflake.yml` will cause the definition update on replace
-* Adding `--pattern` flag to `stage list` command for filtering out results with regex.
+* Adding `--pattern` flag to `stage list-files` command for filtering out results with regex.
 * Fixed snowpark build paths for builds with --project option (fixed empty zip issue).
 * More clear error messages in `snow snowpark build` command
 * Adding support for any source supported by `pip` in `snow snowpark`.
 * Fixed version parsing for packages lookup on Snowflake Anaconda Channel
 * Fix handling database/schema/role identifiers containing dashes
 * Fix schema override bug in `snow connection test`
 * Hidden incorrectly working config permissions warning on Windows
+* Make errors from `snow connection test` more meaningful when role, warehouse or database does not exist.
 
 # v2.1.2
 
 ## Fixes and improvements
 * Add `pip` as Snowflake-cli dependency
 * Optimize `connection test` command
 * Fix venv creation issues in `snowpark package create` and `snowpark build` command
```

### Comparing `snowflake_cli_labs-2.2.0rc0/performance_history_analysis.py` & `snowflake_cli_labs-2.3.0rc0/performance_history_analysis.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_1.png` & `snowflake_cli_labs-2.3.0rc0/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_2.png` & `snowflake_cli_labs-2.3.0rc0/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_3.png` & `snowflake_cli_labs-2.3.0rc0/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_4.png` & `snowflake_cli_labs-2.3.0rc0/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/docs/images/coverage_5.png` & `snowflake_cli_labs-2.3.0rc0/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/__init__.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/cli_global_context.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/cli_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/config.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from snowflake.cli.api.exceptions import (
     ConfigFileTooWidePermissionsError,
     MissingConfiguration,
     UnsupportedConfigSectionTypeError,
 )
 from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.api.secure_utils import file_permissions_are_strict
+from snowflake.cli.api.utils.types import try_cast_to_bool
 from snowflake.connector.compat import IS_WINDOWS
 from snowflake.connector.config_manager import CONFIG_MANAGER
 from snowflake.connector.constants import CONFIG_FILE, CONNECTIONS_FILE
-from snowflake.connector.errors import MissingConfigOptionError
+from snowflake.connector.errors import ConfigSourceError, MissingConfigOptionError
 from tomlkit import TOMLDocument, dump
 from tomlkit.container import Container
 from tomlkit.exceptions import NonExistentKey
 from tomlkit.items import Table
 
 log = logging.getLogger(__name__)
 
@@ -137,15 +138,20 @@
     with warnings.catch_warnings():
         if IS_WINDOWS:
             warnings.filterwarnings(
                 action="ignore",
                 message="Bad owner or permissions.*",
                 module="snowflake.connector.config_manager",
             )
-        CONFIG_MANAGER.read_config()
+        try:
+            CONFIG_MANAGER.read_config()
+        except ConfigSourceError as exception:
+            raise ClickException(
+                f"Configuration file seems to be corrupted. {str(exception.__cause__)}"
+            )
 
 
 def _initialise_logs_section():
     with _config_file() as conf_file_cache:
         if conf_file_cache.get(CLI_SECTION) is None:
             conf_file_cache[CLI_SECTION] = _DEFAULT_CLI_CONFIG
         if conf_file_cache[CLI_SECTION].get(LOGS_SECTION) is None:
@@ -203,15 +209,21 @@
 
 
 def get_default_connection_name() -> str:
     return CONFIG_MANAGER["default_connection_name"]
 
 
 def get_default_connection_dict() -> dict:
-    return get_connection_dict(get_default_connection_name())
+    def_connection_name = get_default_connection_name()
+    if not connection_exists(def_connection_name):
+        raise MissingConfiguration(
+            f"Couldn't find connection for default connection `{def_connection_name}`. "
+            f"Specify connection name or configure default connection."
+        )
+    return get_connection_dict(def_connection_name)
 
 
 def get_config_section(*path) -> dict:
     section = _find_section(*path)
     if isinstance(section, Container):
         return {s: _merge_section_with_env(section[s], *path, s) for s in section}
     if isinstance(section, dict):
@@ -230,29 +242,20 @@
         if default is not Empty:
             return default
         raise
 
 
 def get_config_bool_value(*path, key: str, default: Optional[Any] = Empty) -> bool:
     value = get_config_value(*path, key=key, default=default)
-    # If we get bool then we can return
-    if isinstance(value, bool):
-        return value
-
-    # Now if value is not string then cast it to str. Simplifies logic for 1 and 0
-    if not isinstance(value, str):
-        value = str(value)
-
-    know_booleans_mapping = {"true": True, "false": False, "1": True, "0": False}
-
-    if value.lower() not in know_booleans_mapping:
+    try:
+        return try_cast_to_bool(value)
+    except ValueError:
         raise ClickException(
             f"Expected boolean value for {'.'.join((*path, key))} option."
         )
-    return know_booleans_mapping[value.lower()]
 
 
 def _initialise_config(config_file: Path) -> None:
     config_file = SecurePath(config_file)
     config_file.parent.mkdir(parents=True, exist_ok=True)
     config_file.touch()
     _initialise_logs_section()
@@ -303,7 +306,25 @@
 def _check_default_config_files_permissions() -> None:
     if IS_WINDOWS:
         return
     if CONNECTIONS_FILE.exists() and not file_permissions_are_strict(CONNECTIONS_FILE):
         raise ConfigFileTooWidePermissionsError(CONNECTIONS_FILE)
     if CONFIG_FILE.exists() and not file_permissions_are_strict(CONFIG_FILE):
         raise ConfigFileTooWidePermissionsError(CONFIG_FILE)
+
+
+from typing import Literal
+
+
+def get_feature_flags_section() -> Dict[str, bool | Literal["UNKNOWN"]]:
+    if not config_section_exists(*FEATURE_FLAGS_SECTION_PATH):
+        return {}
+
+    flags = get_config_section(*FEATURE_FLAGS_SECTION_PATH)
+
+    def _bool_or_unknown(value):
+        try:
+            return try_cast_to_bool(value)
+        except ValueError:
+            return "UNKNOWN"
+
+    return {k: _bool_or_unknown(v) for k, v in flags.items()}
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/constants.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/exceptions.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/feature_flags.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/feature_flags.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,7 +30,8 @@
 
 
 @unique
 class FeatureFlag(FeatureFlagMixin):
     ENABLE_STREAMLIT_EMBEDDED_STAGE = BooleanFlag(
         "ENABLE_STREAMLIT_EMBEDDED_STAGE", False
     )
+    ENABLE_NOTEBOOKS = BooleanFlag("ENABLE_NOTEBOOKS", False)
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_path.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/secure_utils.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/secure_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/sql_execution.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/sql_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,21 @@
         *_, last_result = self._execute_queries(query, **kwargs)
         return last_result
 
     def _execute_queries(self, queries: str, **kwargs):
         return list(self._execute_string(dedent(queries), **kwargs))
 
     def use(self, object_type: ObjectType, name: str):
-        return self._execute_query(f"use {object_type.value.sf_name} {name}")
+        try:
+            self._execute_query(f"use {object_type.value.sf_name} {name}")
+        except ProgrammingError:
+            # Rewrite the error to make the message more useful.
+            raise ProgrammingError(
+                f"Could not use {object_type} {name}. Object does not exist, or operation cannot be performed."
+            )
 
     @contextmanager
     def use_role(self, new_role: str):
         """
         Switches to a different role for a while, then switches back.
         This is a no-op if the requested role is already active.
         """
@@ -220,7 +226,15 @@
             )
 
         show_obj_row = find_first_row(
             show_obj_cursor,
             lambda row: row[name_col] == unquote_identifier(unqualified_name),
         )
         return show_obj_row
+
+    def qualified_name_for_url(
+        self, object_name: str, database: str | None = None, schema: str | None = None
+    ):
+        fqn = self.to_fully_qualified_name(
+            object_name, database=database, schema=schema
+        )
+        return ".".join(unquote_identifier(part) for part in fqn.split("."))
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/decorators.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/flags.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import tempfile
+from dataclasses import dataclass
 from enum import Enum
 from inspect import signature
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Tuple
 
 import click
 import typer
@@ -528,7 +529,29 @@
         if ctx.get_parameter_source(param.name) != click.core.ParameterSource.DEFAULT:  # type: ignore[attr-defined]
             cli_console.warning(message=msg)
         # Typer bug: enums passed through callback are turning into None,
         # unless their explicit value is returned ¯\_(ツ)_/¯
         return value.value
 
     return _warning_callback
+
+
+@dataclass
+class Variable:
+    key: str
+    value: str
+
+    def __init__(self, key: str, value: str):
+        self.key = key
+        self.value = value
+
+
+def parse_key_value_variables(variables: List[str]) -> List[Variable]:
+    """Util for parsing key=value input. Useful for commands accepting multiple input options."""
+    result = []
+    for p in variables:
+        if "=" not in p:
+            raise ClickException(f"Invalid variable: '{p}'")
+
+        key, value = p.split("=", 1)
+        result.append(Variable(key.strip(), value.strip()))
+    return result
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/project_initialisation.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/commands/snow_typer.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/commands/snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/abc.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/console/abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/console/console.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/console/console.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/output/types.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/output/types.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/plugins/command/__init__.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/plugins/command/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/definition_manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/errors.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/errors.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/util.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/project_definition.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/updatable_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,18 +10,30 @@
 
     def __init__(self, *args, **kwargs):
         try:
             super().__init__(**kwargs)
         except ValidationError as e:
             raise SchemaValidationError(e)
 
-    def update_from_dict(
-        self, update_values: Dict[str, Any]
-    ):  # this method works wrong for optional fields set to None
-        for field, value in update_values.items():  # do we even need this?
-            if getattr(self, field, None):
-                setattr(self, field, value)
+    def update_from_dict(self, update_values: Dict[str, Any]):
+        """
+        Takes a dictionary with values to override.
+        If the field type is subclass of a UpdatableModel, its update_from_dict() method is called with
+        the value to be set.
+        If not, we use simple setattr to set new value.
+        Values provided are validated against original restrictions, so it's impossible to overwrite string field with
+        integer value etc.
+        """
+        for field, value in update_values.items():
+            if field in self.model_fields.keys():
+                if (
+                    hasattr(getattr(self, field), "update_from_dict")
+                    and field in self.model_fields_set
+                ):
+                    getattr(self, field).update_from_dict(value)
+                else:
+                    setattr(self, field, value)
         return self
 
 
 def IdentifierField(*args, **kwargs):  # noqa
     return Field(max_length=254, pattern=IDENTIFIER_NO_LENGTH, *args, **kwargs)
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Literal, Optional
+from typing import Optional
 
 from pydantic import Field
 from snowflake.cli.api.project.schemas.updatable_model import (
     IdentifierField,
     UpdatableModel,
 )
 
@@ -22,10 +22,7 @@
         title="Name of the application object created when you run the snow app run command",
         default=None,
     )
     debug: Optional[bool] = Field(
         title="Whether to enable debug mode when using a named stage to create an application object",
         default=True,
     )
-
-
-DistributionOptions = Literal["internal", "external", "INTERNAL", "EXTERNAL"]
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/native_app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/native_app/package.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import Field, field_validator
-from snowflake.cli.api.project.schemas.native_app.application import DistributionOptions
 from snowflake.cli.api.project.schemas.updatable_model import (
     IdentifierField,
     UpdatableModel,
 )
 
+DistributionOptions = Literal["internal", "external", "INTERNAL", "EXTERNAL"]
+
 
 class Package(UpdatableModel):
     scripts: Optional[List[str]] = Field(
         title="List of SQL file paths relative to the project root", default=None
     )
     role: Optional[str] = IdentifierField(
         title="Role to use when creating the application package and provider-side objects",
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/snowpark/callable.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     )
     external_access_integrations: Optional[List[str]] = Field(
         title="Names of external access integrations needed for this procedure’s handler code to access external networks",
         default=[],
     )
     secrets: Optional[Dict[str, str]] = Field(
         title="Assigns the names of secrets to variables so that you can use the variables to reference the secrets",
-        default=[],
+        default={},
     )
     imports: Optional[List[str]] = Field(
         title="Stage and path to previously uploaded files you want to import",
         default=[],
     )
 
     @field_validator("runtime")
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/snowpark/snowpark.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/project/schemas/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/cursor.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/naming_utils.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/path_utils.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/api/utils/rendering.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/api/utils/rendering.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
-import json
+import os
 from pathlib import Path
 from textwrap import dedent
-from typing import Optional
+from typing import Dict, Optional
 
 import jinja2
+from jinja2 import Environment, StrictUndefined, loaders
 from snowflake.cli.api.secure_path import UNLIMITED, SecurePath
 
 
 def read_file_content(file_name: str):
     return SecurePath(file_name).read_text(file_size_limit_mb=UNLIMITED)
 
 
@@ -29,93 +30,82 @@
         )
     )
     return template.render(
         code=SecurePath(file_name).read_text(file_size_limit_mb=UNLIMITED)
     )
 
 
-PROCEDURE_TEMPLATE = dedent(
-    """\
-    CREATE OR REPLACE {{ object_type | upper }} {{ name | upper }}(\
-    {% for arg in signature %}
-    {{ arg['name'] | upper }} {{ arg['type'] }}{{ "," if not loop.last -}}
-    {% endfor %}
-    )
-    RETURNS {{ returns }}
-    LANGUAGE {{ language }}
-    {% if runtime_version is defined -%}
-    RUNTIME_VERSION = '{{ runtime_version }}'
-    {% endif -%}
-    {% if packages is defined -%}
-    PACKAGES = ('{{ packages }}')
-    {% endif -%}
-    {% if imports is defined -%}
-    IMPORTS = ({% for import in imports %}'{{ import }}'{{ ", " if not loop.last }}{% endfor %})
-    {% endif -%}
-    {% if handler is defined -%}
-    HANDLER = '{{ handler }}'
-    {% endif -%}
-    {% if code is defined -%}
-    AS
-    $$
-    {{ code }}
-    $$
-    {%- endif -%}
-    ;
-
-    {%- if grants is defined -%}
-    {%- for grant in grants %}
-    GRANT USAGE ON {{ object_type | upper }} {{ name | upper }}({% for arg in signature %}{{ arg['type'] }}{{ ", " if not loop.last }}{% endfor %})
-    TO DATABASE ROLE {{ grant['role'] }};
-    {% endfor -%}
-    {% endif -%}\
-"""
-)
+_CUSTOM_FILTERS = [read_file_content, procedure_from_js_file]
 
 
-@jinja2.pass_environment  # type: ignore
-def render_metadata(env: jinja2.Environment, file_name: str):
-    metadata = json.loads(
-        SecurePath(file_name).absolute().read_text(file_size_limit_mb=UNLIMITED)
-    )
-    template = env.from_string(PROCEDURE_TEMPLATE)
+def _env_bootstrap(env: Environment) -> Environment:
+    for custom_filter in _CUSTOM_FILTERS:
+        env.filters[custom_filter.__name__] = custom_filter
+
+    return env
+
 
-    rendered = []
-    known_objects = {
-        "procedures": "procedure",
-        "udfs": "function",
-        "udtfs": "function",
-    }
-    for object_key, object_type in known_objects.items():
-        for obj in metadata.get(object_key, []):
-            rendered.append(template.render(object_type=object_type, **obj))
-    return "\n".join(rendered)
+def get_snowflake_cli_jinja_env():
+    _random_block = "___very___unique___block___to___disable___logic___blocks___"
+    return _env_bootstrap(
+        Environment(
+            loader=loaders.BaseLoader(),
+            keep_trailing_newline=True,
+            variable_start_string="&{",
+            variable_end_string="}",
+            block_start_string=_random_block,
+            block_end_string=_random_block,
+            undefined=StrictUndefined,
+        )
+    )
 
 
-def generic_render_template(
-    template_path: Path, data: dict, output_file_path: Optional[Path] = None
+def jinja_render_from_file(
+    template_path: Path, data: Dict, output_file_path: Optional[Path] = None
 ):
     """
     Create a file from a jinja template.
 
     Args:
         template_path (Path): Path to the template
         data (dict): A dictionary of jinja variables and their actual values
         output_file_path (Optional[Path]): If provided then rendered template will be written to this file
 
     Returns:
         None
     """
-    env = jinja2.Environment(
-        loader=jinja2.loaders.FileSystemLoader(template_path.parent),
-        keep_trailing_newline=True,
-        undefined=jinja2.StrictUndefined,
+    env = _env_bootstrap(
+        Environment(
+            loader=loaders.FileSystemLoader(template_path.parent),
+            keep_trailing_newline=True,
+            undefined=StrictUndefined,
+        )
     )
-    filters = [render_metadata, read_file_content, procedure_from_js_file]
-    for custom_filter in filters:
-        env.filters[custom_filter.__name__] = custom_filter
     loaded_template = env.get_template(template_path.name)
     rendered_result = loaded_template.render(**data)
     if output_file_path:
         SecurePath(output_file_path).write_text(rendered_result)
     else:
         print(rendered_result)
+
+
+class _AttrGetter:
+    def __init__(self, data_dict):
+        self._data_dict = data_dict
+
+    def __getattr__(self, item):
+        if item not in self._data_dict:
+            raise AttributeError(f"No attribute {item}")
+        return self._data_dict[item]
+
+
+def _add_project_context(data: Dict):
+    context_key = "ctx"
+    if context_key in data:
+        raise ValueError(f"{context_key} in user defined data")
+    context_data = {context_key: {"env": _AttrGetter(os.environ)}}
+    return {**data, **context_data}
+
+
+def snowflake_cli_jinja_render(content: str, data: Dict | None = None) -> str:
+    data = _add_project_context(data or dict())
+    return get_snowflake_cli_jinja_env().from_string(content).render(**data)
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/cli_app.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/cli_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,26 +103,30 @@
 @_do_not_execute_on_completion
 def _version_callback(value: bool):
     if value:
         print_result(MessageResult(f"Snowflake CLI version: {__about__.VERSION}"))
         _exit_with_cleanup()
 
 
+from snowflake.cli.api.config import get_feature_flags_section
+
+
 @_do_not_execute_on_completion
 def _info_callback(value: bool):
     if value:
         result = CollectionResult(
             [
                 {"key": "version", "value": __about__.VERSION},
                 {
                     "key": "default_config_file_path",
                     "value": str(CONFIG_MANAGER.file_path),
                 },
                 {"key": "python_version", "value": sys.version},
                 {"key": "system_info", "value": platform.platform()},
+                {"key": "feature_flags", "value": get_feature_flags_section()},
             ],
         )
         print_result(result, output_format=OutputFormat.JSON)
         _exit_with_cleanup()
 
 
 def app_factory() -> SnowCliMainTyper:
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/loggers.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/loggers.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/main_typer.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/main_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/printing.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/snow_connector.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/snow_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,26 @@
 from snowflake.cli.api.config import get_connection_dict, get_default_connection_dict
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB
 from snowflake.cli.api.exceptions import (
     InvalidConnectionConfiguration,
     SnowflakeConnectionError,
 )
 from snowflake.cli.api.secure_path import SecurePath
+from snowflake.cli.app.constants import (
+    PARAM_APPLICATION_NAME,
+    PARAM_INTERNAL_APPLICATION_NAME,
+)
 from snowflake.cli.app.telemetry import command_info
 from snowflake.connector import SnowflakeConnection
 from snowflake.connector.errors import DatabaseError, ForbiddenError
 
 log = logging.getLogger(__name__)
 
+from snowflake.cli.__about__ import VERSION
+
 ENCRYPTED_PKCS8_PK_HEADER = b"-----BEGIN ENCRYPTED PRIVATE KEY-----"
 UNENCRYPTED_PKCS8_PK_HEADER = b"-----BEGIN PRIVATE KEY-----"
 
 
 def connect_to_snowflake(
     temporary_connection: bool = False,
     mfa_passcode: Optional[str] = None,
@@ -88,14 +94,16 @@
             ] = diag_allowlist_path
 
     # Make sure the connection is not closed if it was shared to the SnowCLI, instead of being created in the SnowCLI
     _avoid_closing_the_connection_if_it_was_shared(
         using_session_token, using_master_token, connection_parameters
     )
 
+    _update_connection_application_name(connection_parameters)
+
     try:
         # Whatever output is generated when creating connection,
         # we don't want it in our output. This is particularly important
         # for cases when external browser and json format are used.
         # Redirecting both stdout and stderr for offline usage.
         with contextlib.redirect_stdout(None), contextlib.redirect_stderr(None):
             return snowflake.connector.connect(
@@ -141,14 +149,24 @@
         else:
             raise ClickException(
                 "Private Key authentication requires authenticator set to SNOWFLAKE_JWT"
             )
     return connection_parameters
 
 
+def _update_connection_application_name(connection_parameters: Dict):
+    """Update version and name of app handling connection."""
+    connection_application_params = {
+        "application_name": PARAM_APPLICATION_NAME,
+        "_internal_application_name": PARAM_INTERNAL_APPLICATION_NAME,
+        "_internal_application_version": VERSION,
+    }
+    connection_parameters.update(connection_application_params)
+
+
 def _load_pem_to_der(private_key_path: str) -> bytes:
     """
     Given a private key file path (in PEM format), decode key data into DER
     format
     """
     from cryptography.hazmat.backends import default_backend
     from cryptography.hazmat.primitives.serialization import (
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/telemetry.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import sys
 from enum import Enum, unique
 from typing import Any, Dict, Union
 
 import click
 from snowflake.cli.__about__ import VERSION
 from snowflake.cli.api.cli_global_context import cli_context
+from snowflake.cli.api.config import get_feature_flags_section
 from snowflake.cli.api.output.formats import OutputFormat
 from snowflake.cli.api.utils.error_handling import ignore_exceptions
+from snowflake.cli.app.constants import PARAM_APPLICATION_NAME
 from snowflake.connector.telemetry import (
     TelemetryData,
     TelemetryField,
 )
 from snowflake.connector.time_util import get_time_millis
 
 
@@ -25,14 +27,16 @@
     VERSION_PYTHON = "version_python"
     VERSION_OS = "version_os"
     # Command execution context
     COMMAND = "command"
     COMMAND_GROUP = "command_group"
     COMMAND_FLAGS = "command_flags"
     COMMAND_OUTPUT_TYPE = "command_output_type"
+    # Configuration
+    CONFIG_FEATURE_FLAGS = "config_feature_flags"
     # Information
     EVENT = "event"
     ERROR_MSG = "error_msg"
     ERROR_TYPE = "error_type"
 
 
 class TelemetryEvent(Enum):
@@ -57,15 +61,16 @@
             "format", OutputFormat.TABLE
         ).value,
     }
 
 
 def command_info() -> str:
     info = _find_command_info()
-    return ("SNOWCLI." + ".".join(info[CLITelemetryField.COMMAND])).upper()
+    command = ".".join(info[CLITelemetryField.COMMAND])
+    return f"{PARAM_APPLICATION_NAME}.{command}".upper()
 
 
 def python_version() -> str:
     py_ver = sys.version_info
     return f"{py_ver.major}.{py_ver.minor}.{py_ver.micro}"
 
 
@@ -74,18 +79,21 @@
         self._ctx = ctx
 
     @staticmethod
     def generate_telemetry_data_dict(
         telemetry_payload: TelemetryDict,
     ) -> Dict[str, Any]:
         data = {
-            CLITelemetryField.SOURCE: "snowcli",
+            CLITelemetryField.SOURCE: PARAM_APPLICATION_NAME,
             CLITelemetryField.VERSION_CLI: VERSION,
             CLITelemetryField.VERSION_OS: platform.platform(),
             CLITelemetryField.VERSION_PYTHON: python_version(),
+            CLITelemetryField.CONFIG_FEATURE_FLAGS: {
+                k: str(v) for k, v in get_feature_flags_section().items()
+            },
             **_find_command_info(),
             **telemetry_payload,
         }
         # To map Enum to string, so we don't have to use .value every time
         return {getattr(k, "value", k): v for k, v in data.items()}  # type: ignore[arg-type]
 
     @property
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/api_impl/plugin/plugin_config_provider_impl.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/builtin_plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from snowflake.cli.plugins.connection import plugin_spec as connection_plugin_spec
 from snowflake.cli.plugins.git import plugin_spec as git_plugin_spec
 from snowflake.cli.plugins.nativeapp import plugin_spec as nativeapp_plugin_spec
+from snowflake.cli.plugins.notebook import plugin_spec as notebook_plugin_spec
 from snowflake.cli.plugins.object import plugin_spec as object_plugin_spec
-from snowflake.cli.plugins.render import plugin_spec as render_plugin_spec
 from snowflake.cli.plugins.snowpark import plugin_spec as snowpark_plugin_spec
 from snowflake.cli.plugins.spcs import plugin_spec as spcs_plugin_spec
 from snowflake.cli.plugins.sql import plugin_spec as sql_plugin_spec
 from snowflake.cli.plugins.stage import plugin_spec as stage_plugin_spec
 from snowflake.cli.plugins.streamlit import plugin_spec as streamlit_plugin_spec
 
 
 # plugin name to plugin spec
 def get_builtin_plugin_name_to_plugin_spec():
     plugin_specs = {
         "connection": connection_plugin_spec,
         "spcs": spcs_plugin_spec,
         "nativeapp": nativeapp_plugin_spec,
         "object": object_plugin_spec,
-        "render": render_plugin_spec,
         "snowpark": snowpark_plugin_spec,
         "stage": stage_plugin_spec,
         "sql": sql_plugin_spec,
         "streamlit": streamlit_plugin_spec,
         "git": git_plugin_spec,
+        "notebook": notebook_plugin_spec,
     }
 
     return plugin_specs
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/command_plugins_loader.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/commands_registration_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/threadsafe.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/commands_registration/typer_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/commands_structure.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/commands_structure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/pycharm_remote_debug.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/generator.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/docs/generator.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/app/dev/docs/templates/usage.rst.jinja2`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/connection/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/connection/util.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/connection/util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/git/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/git/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     requires_connection=True,
 )
 def fetch(
     repository_name: str = RepoNameArgument,
     **options,
 ) -> CommandResult:
     """
-    Fetch changes from origin to snowflake repository.
+    Fetch changes from origin to Snowflake repository.
     """
     return QueryResult(GitManager().fetch(repo_name=repository_name))
 
 
 @app.command(
     "copy",
     requires_connection=True,
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/artifacts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
-from click import ClickException
+from click.exceptions import ClickException
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB
 from snowflake.cli.api.project.schemas.native_app.path_mapping import PathMapping
 from snowflake.cli.api.secure_path import SecurePath
 from yaml import safe_load
 
+# Map from source directories and files in the project directory to their path in the deploy directory. Both paths are absolute.
+ArtifactDeploymentMap = Dict[Path, Path]
+
 
 class DeployRootError(ClickException):
     """
     The deploy root was incorrectly specified.
     """
 
     def __init__(self, msg: str):
@@ -191,19 +194,22 @@
     Resolves a Path to an absolute version of itself, without following
     symlinks like Path.resolve() does.
     """
     return Path(os.path.abspath(path))
 
 
 def build_bundle(
-    project_root: Path, deploy_root: Path, artifacts: List[ArtifactMapping]
-):
+    project_root: Path,
+    deploy_root: Path,
+    artifacts: List[ArtifactMapping],
+) -> ArtifactDeploymentMap:
     """
     Prepares a local folder (deploy_root) with configured app artifacts.
     This folder can then be uploaded to a stage.
+    Returns a map of the copied source files, pointing to where they were copied.
     """
     resolved_root = deploy_root.resolve()
     if resolved_root.exists() and not resolved_root.is_dir():
         raise DeployRootError(
             f"Deploy root {resolved_root} exists, but is not a directory!"
         )
 
@@ -213,37 +219,42 @@
         )
 
     # users may have removed files or entire artifact mappings from their project
     # definition since the last time we bundled; we need to clear the deploy root first
     if resolved_root.exists():
         delete(resolved_root)
 
+    mapped_files: ArtifactDeploymentMap = {}
     for artifact in artifacts:
         dest_path = resolve_without_follow(Path(resolved_root, artifact.dest))
         source_paths = get_source_paths(artifact, project_root)
 
         if specifies_directory(artifact.dest):
             # make sure we are only modifying files / directories inside the deploy root
             if resolved_root != dest_path and resolved_root not in dest_path.parents:
                 raise NotInDeployRootError(artifact.src, dest_path, resolved_root)
 
             # copy all files as children of the given destination path
             for source_path in source_paths:
-                symlink_or_copy(source_path, dest_path / source_path.name)
+                dest_child_path = dest_path / source_path.name
+                symlink_or_copy(source_path, dest_child_path)
+                mapped_files[source_path.resolve()] = dest_child_path
         else:
             # ensure we are copying into the deploy root, not replacing it!
             if resolved_root not in dest_path.parents:
                 raise NotInDeployRootError(artifact.src, dest_path, resolved_root)
 
             if len(source_paths) == 1:
                 # copy a single file as the given destination path
                 symlink_or_copy(source_paths[0], dest_path)
+                mapped_files[source_paths[0].resolve()] = dest_path
             else:
                 # refuse to map multiple source files to one destination (undefined behaviour)
                 raise TooManyFilesError(dest_path)
+    return mapped_files
 
 
 def find_manifest_file(deploy_root: Path) -> Path:
     """
     Find manifest.yml file, if available, in the deploy_root of the Snowflake Native App project.
     """
     resolved_root = deploy_root.resolve()
@@ -279,7 +290,35 @@
     if version_field in manifest_content:
         version_info = manifest_content[version_field]
         version_name = version_info[name_field]
         if patch_field in version_info:
             patch_name = version_info[patch_field]
 
     return version_name, patch_name
+
+
+def source_path_to_deploy_path(
+    source_path: Path, mapped_files: ArtifactDeploymentMap
+) -> Path:
+    """Returns the absolute path where the specified source path was copied to during bundle."""
+
+    source_path = source_path.resolve()
+
+    if source_path in mapped_files:
+        return mapped_files[source_path]
+
+    # Find the first parent directory that exists in mapped_files
+    common_root = source_path
+    while common_root:
+        if common_root in mapped_files:
+            break
+        elif common_root.parent != common_root:
+            common_root = common_root.parent
+        else:
+            raise ClickException(f"Could not find the deploy path of {source_path}")
+
+    # Construct the target deploy path
+    path_to_symlink = mapped_files[common_root]
+    relative_path_to_target = Path(source_path).relative_to(common_root)
+    result = Path(path_to_symlink, relative_path_to_target)
+
+    return result
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
-from typing import Optional
+from pathlib import Path
+from typing import List, Optional
 
 import typer
 from snowflake.cli.api.cli_global_context import cli_context
 from snowflake.cli.api.commands.decorators import (
     with_project_definition,
 )
 from snowflake.cli.api.commands.snow_typer import SnowTyper
@@ -225,21 +226,49 @@
     processor.process(force)
     return MessageResult(f"Teardown is now complete.")
 
 
 @app.command("deploy", requires_connection=True)
 @with_project_definition("native_app")
 def app_deploy(
+    prune: Optional[bool] = typer.Option(
+        default=None,
+        help=f"""Whether to delete specified files from the stage if they don't exist locally. If set, the command deletes files that exist in the stage, but not in the local filesystem.""",
+    ),
+    recursive: Optional[bool] = typer.Option(
+        None,
+        "--recursive",
+        "-r",
+        help=f"""Whether to traverse and deploy files from subdirectories. If set, the command deploys all files and subdirectories; otherwise, only files in the current directory are deployed.""",
+    ),
+    files: Optional[List[Path]] = typer.Argument(
+        default=None,
+        show_default=False,
+        help=f"""Paths, relative to the the project root, of files you want to upload to a stage. The paths must match one of the artifacts src pattern entries in snowflake.yml. If unspecified, the command syncs all local changes to the stage.""",
+    ),
     **options,
 ) -> CommandResult:
     """
     Creates an application package in your Snowflake account and syncs the local changes to the stage without creating or updating the application.
+    Running this command with no arguments at all, as in `snow app deploy`, is a shorthand for `snow app deploy --prune --recursive`.
     """
+    has_files = files is not None and len(files) > 0
+    if prune is None and recursive is None and not has_files:
+        prune = True
+        recursive = True
+    else:
+        if prune is None:
+            prune = False
+        if recursive is None:
+            recursive = False
+
     manager = NativeAppManager(
         project_definition=cli_context.project_definition,
         project_root=cli_context.project_root,
     )
 
-    manager.build_bundle()
-    manager.deploy()
+    mapped_files = manager.build_bundle()
+    manager.deploy(prune, recursive, files, mapped_files)
 
-    return MessageResult(f"Deployed successfully.")
+    return MessageResult(
+        f"Deployed successfully. Application package and stage are up-to-date."
+    )
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/common_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/init.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.api.project.util import (
     is_valid_identifier,
     is_valid_unquoted_identifier,
     to_identifier,
 )
 from snowflake.cli.api.secure_path import SecurePath
-from snowflake.cli.api.utils.rendering import generic_render_template
+from snowflake.cli.api.utils.rendering import jinja_render_from_file
 from yaml import dump, safe_dump, safe_load
 
 log = logging.getLogger(__name__)
 
 OFFICIAL_TEMPLATES_GITHUB_URL = "https://github.com/snowflakedb/native-apps-templates"
 BASIC_TEMPLATE = "basic"
 
@@ -117,15 +117,15 @@
     Returns:
         None
     """
 
     snowflake_yml_jinja = "snowflake.yml.jinja"
 
     try:
-        generic_render_template(
+        jinja_render_from_file(
             template_path=parent_to_snowflake_yml / snowflake_yml_jinja,
             data={
                 # generic_render_template operates on text, not YAML, so escape before rendering
                 "project_name": _to_yaml_string(project_identifier)
             },
             output_file_path=parent_to_snowflake_yml / "snowflake.yml",
         )
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 from abc import ABC, abstractmethod
 from functools import cached_property
 from pathlib import Path
 from textwrap import dedent
 from typing import List, Optional
 
 import jinja2
@@ -19,16 +20,19 @@
     extract_schema,
     to_identifier,
     unquote_identifier,
 )
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.connection.util import make_snowsight_url
 from snowflake.cli.plugins.nativeapp.artifacts import (
+    ArtifactDeploymentMap,
     ArtifactMapping,
     build_bundle,
+    resolve_without_follow,
+    source_path_to_deploy_path,
     translate_artifact,
 )
 from snowflake.cli.plugins.nativeapp.constants import (
     ALLOWED_SPECIAL_COMMENTS,
     COMMENT_COL,
     ERROR_MESSAGE_606,
     ERROR_MESSAGE_2043,
@@ -39,18 +43,22 @@
 )
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationPackageAlreadyExistsError,
     InvalidPackageScriptError,
     MissingPackageScriptError,
     UnexpectedOwnerError,
 )
+from snowflake.cli.plugins.nativeapp.utils import verify_exists, verify_no_directories
 from snowflake.cli.plugins.stage.diff import (
     DiffResult,
-    stage_diff,
+    StagePath,
+    compute_stage_diff,
+    preserve_from_diff,
     sync_local_diff_with_stage,
+    to_stage_path,
 )
 from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import DictCursor
 
 
 def generic_sql_error_handler(
     err: ProgrammingError, role: Optional[str] = None, warehouse: Optional[str] = None
@@ -96,14 +104,33 @@
     actual_owner = row[
         OWNER_COL
     ].upper()  # Because unquote_identifier() always returns uppercase str
     if actual_owner != unquote_identifier(role):
         raise UnexpectedOwnerError(obj_name, role, actual_owner)
 
 
+def _get_stage_paths_to_sync(
+    local_paths_to_sync: List[Path], deploy_root: Path
+) -> List[StagePath]:
+    """
+    Takes a list of paths (files and directories), returning a list of all files recursively relative to the deploy root.
+    """
+
+    stage_paths = []
+    for path in local_paths_to_sync:
+        if path.is_dir():
+            for current_dir, _dirs, files in os.walk(path):
+                for file in files:
+                    deploy_path = Path(current_dir, file).relative_to(deploy_root)
+                    stage_paths.append(to_stage_path(deploy_path))
+        else:
+            stage_paths.append(to_stage_path(path.relative_to(deploy_root)))
+    return stage_paths
+
+
 class NativeAppCommandProcessor(ABC):
     @abstractmethod
     def process(self, *args, **kwargs):
         pass
 
 
 class NativeAppManager(SqlExecutionMixin):
@@ -274,24 +301,43 @@
                     which does not match the value specified in project definition file: {project_def_distribution}.
                     """
                 )
             )
             return False
         return True
 
-    def build_bundle(self) -> None:
+    def build_bundle(self) -> ArtifactDeploymentMap:
         """
         Populates the local deploy root from artifact sources.
         """
-        build_bundle(self.project_root, self.deploy_root, self.artifacts)
+        return build_bundle(self.project_root, self.deploy_root, self.artifacts)
 
-    def sync_deploy_root_with_stage(self, role: str) -> DiffResult:
+    def sync_deploy_root_with_stage(
+        self,
+        role: str,
+        prune: bool,
+        recursive: bool,
+        local_paths_to_sync: List[Path] | None = None,
+        mapped_files: Optional[ArtifactDeploymentMap] = None,
+    ) -> DiffResult:
         """
         Ensures that the files on our remote stage match the artifacts we have in
-        the local filesystem. Returns the DiffResult used to make changes.
+        the local filesystem.
+
+        Args:
+            role (str): The name of the role to use for queries and commands.
+            prune (bool): Whether to prune artifacts from the stage that don't exist locally.
+            recursive (bool): Whether to traverse directories recursively.
+            local_paths_to_sync (List[Path], optional): List of local paths to sync. Defaults to None to sync all
+             local paths. Note that providing an empty list here is equivalent to None.
+            mapped_files: the file mapping computed during the `bundle` step. Required when local_paths_to_sync is
+             provided.
+
+        Returns:
+            A `DiffResult` instance describing the changes that were performed.
         """
 
         # Does a stage already exist within the application package, or we need to create one?
         # Using "if not exists" should take care of either case.
         cc.step("Checking if stage exists, or creating a new one if none exists.")
         with self.use_role(role):
             self._execute_query(
@@ -305,28 +351,64 @@
             )
 
         # Perform a diff operation and display results to the user for informational purposes
         cc.step(
             "Performing a diff between the Snowflake stage and your local deploy_root ('%s') directory."
             % self.deploy_root
         )
-        diff: DiffResult = stage_diff(self.deploy_root, self.stage_fqn)
+        diff: DiffResult = compute_stage_diff(self.deploy_root, self.stage_fqn)
+
+        files_not_removed = []
+        if local_paths_to_sync:
+            assert mapped_files is not None
+
+            # Deploying specific files/directories
+            resolved_paths_to_sync = [
+                resolve_without_follow(p) for p in local_paths_to_sync
+            ]
+            if not recursive:
+                verify_no_directories(resolved_paths_to_sync)
+            deploy_paths_to_sync = [
+                source_path_to_deploy_path(p, mapped_files)
+                for p in resolved_paths_to_sync
+            ]
+            verify_exists(deploy_paths_to_sync)
+            stage_paths_to_sync = _get_stage_paths_to_sync(
+                deploy_paths_to_sync, self.deploy_root.resolve()
+            )
+            diff = preserve_from_diff(diff, stage_paths_to_sync)
+        else:
+            # Full deploy
+            if not recursive:
+                deploy_files = [p for p in self.deploy_root.resolve().iterdir()]
+                verify_no_directories(deploy_files)
+
+        if not prune:
+            files_not_removed = [str(path) for path in diff.only_on_stage]
+            diff.only_on_stage = []
+
+            if len(files_not_removed) > 0:
+                files_not_removed_str = "\n".join(files_not_removed)
+                cc.warning(
+                    f"The following files exist only on the stage:\n{files_not_removed_str}\n\nUse the --prune flag to delete them from the stage."
+                )
+
         cc.message(str(diff))
 
         # Upload diff-ed files to application package stage
         if diff.has_changes():
             cc.step(
                 "Uploading diff-ed files from your local %s directory to the Snowflake stage."
                 % self.deploy_root,
             )
             sync_local_diff_with_stage(
                 role=role,
                 deploy_root_path=self.deploy_root,
                 diff_result=diff,
-                stage_path=self.stage_fqn,
+                stage_fqn=self.stage_fqn,
             )
         return diff
 
     def get_existing_app_info(self) -> Optional[dict]:
         """
         Check for an existing application object by the same name as in project definition, in account.
         It executes a 'show applications like' query and returns the result as single row, if one exists.
@@ -431,21 +513,29 @@
                 cc.step(f"Applying package script: {self.package_scripts[i]}")
                 self._execute_queries(queries)
         except ProgrammingError as err:
             generic_sql_error_handler(
                 err, role=self.package_role, warehouse=self.package_warehouse
             )
 
-    def deploy(self) -> DiffResult:
+    def deploy(
+        self,
+        prune: bool,
+        recursive: bool,
+        local_paths_to_sync: List[Path] | None = None,
+        mapped_files: Optional[ArtifactDeploymentMap] = None,
+    ) -> DiffResult:
         """app deploy process"""
 
         # 1. Create an empty application package, if none exists
         self.create_app_package()
 
         with self.use_role(self.package_role):
             # 2. now that the application package exists, create shared data
             self._apply_package_scripts()
 
             # 3. Upload files from deploy root local folder to the above stage
-            diff = self.sync_deploy_root_with_stage(self.package_role)
+            diff = self.sync_deploy_root_with_stage(
+                self.package_role, prune, recursive, local_paths_to_sync, mapped_files
+            )
 
         return diff
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/policy.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/run_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,21 +67,18 @@
                 # Check for the right owner
                 ensure_correct_owner(
                     row=show_app_row, role=self.app_role, obj_name=self.app_name
                 )
 
                 # If all the above checks are in order, proceed to upgrade
                 try:
-                    if diff.has_changes():
-                        cc.step(
-                            f"Upgrading existing application object {self.app_name}."
-                        )
-                        self._execute_query(
-                            f"alter application {self.app_name} upgrade using @{self.stage_fqn}"
-                        )
+                    cc.step(f"Upgrading existing application object {self.app_name}.")
+                    self._execute_query(
+                        f"alter application {self.app_name} upgrade using @{self.stage_fqn}"
+                    )
 
                     # ensure debug_mode is up-to-date
                     self._execute_query(
                         f"alter application {self.app_name} set debug_mode = {self.debug_mode}"
                     )
 
                     return
@@ -293,9 +290,9 @@
                 policy=policy,
                 version=version,
                 patch=patch,
                 is_interactive=is_interactive,
             )
             return
 
-        diff = self.deploy()
+        diff = self.deploy(prune=True, recursive=True)
         self._create_dev_app(diff)
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/teardown_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from os import PathLike
 from pathlib import Path
 from sys import stdin, stdout
-from typing import Optional, Union
+from typing import List, Optional, Union
+
+from click import ClickException
 
 
 def needs_confirmation(needs_confirm: bool, auto_yes: bool) -> bool:
     return needs_confirm and not auto_yes
 
 
 def is_tty_interactive():
@@ -61,7 +63,21 @@
         filter=["tree:0"],
         depth=1,
     )
     # Close repo to avoid issues with permissions on Windows
     repo.close()
 
     return repo
+
+
+def verify_no_directories(paths_to_sync: List[Path]):
+    for path in paths_to_sync:
+        if path.is_dir():
+            raise ClickException(
+                f"{path} is a directory. Add the -r flag to deploy directories."  #
+            )
+
+
+def verify_exists(paths_to_sync: List[Path]):
+    for path in paths_to_sync:
+        if not path.exists():
+            raise ClickException(f"The following path does not exist: {path}")
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/version/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/nativeapp/version/version_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,17 @@
         self.create_app_package()
 
         with self.use_role(self.package_role):
             # Now that the application package exists, create shared data
             self._apply_package_scripts()
 
             # Upload files from deploy root local folder to the above stage
-            self.sync_deploy_root_with_stage(self.package_role)
+            self.sync_deploy_root_with_stage(
+                self.package_role, prune=True, recursive=True
+            )
 
         # Warn if the version exists in a release directive(s)
         existing_release_directives = (
             self.get_existing_release_directive_info_for_version(version)
         )
         if existing_release_directives:
             release_directive_names = ", ".join(
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/common.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @dataclass
 class Tag:
     name: str
     value: str
 
     def __post_init__(self):
         if not is_valid_identifier(self.name):
-            raise ValueError("name of a tag must be a valid snowflake identifier")
+            raise ValueError("name of a tag must be a valid Snowflake identifier")
 
     def value_string_literal(self):
         return to_string_literal(self.value)
 
 
 class TagError(ClickException):
     def __init__(self):
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/object/stage_deprecated/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/common.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/models.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,19 @@
     downloaded files/folders that belong to it"""
 
     requirement: Requirement
     files: List[str]
 
 
 @dataclass
-class RequirementWithWheelAndDeps:
+class RequirementWithWheel:
     """A dataclass to hold a requirement and corresponding .whl file."""
 
     requirement: Requirement
     wheel_path: Path | None
-    dependencies: List[str]
 
     def extract_files(self, destination: Path) -> None:
         if self.wheel_path is not None:
             zipfile.ZipFile(self.wheel_path).extractall(destination)
 
     def namelist(self) -> List[str]:
         if self.wheel_path is None:
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from __future__ import annotations
 
 import dataclasses
+import locale
 import logging
 import os
 import re
+import subprocess
+from pathlib import Path
 from textwrap import dedent
-from typing import List
+from typing import Dict, List, Optional
 
+from click import ClickException
 from snowflake.cli.api.constants import DEFAULT_SIZE_LIMIT_MB
 from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.plugins.snowpark.models import (
     Requirement,
     RequirementWithFiles,
-    RequirementWithWheelAndDeps,
+    RequirementWithWheel,
     WheelMetadata,
 )
 from snowflake.cli.plugins.snowpark.package.anaconda_packages import (
     AnacondaPackages,
 )
-from snowflake.cli.plugins.snowpark.venv import Venv
 
 log = logging.getLogger(__name__)
 
 PIP_PATH = os.environ.get("SNOWCLI_PIP_PATH", "pip")
 
 
 def parse_requirements(
@@ -69,16 +72,16 @@
         )
     )
 
 
 def get_package_name_from_pip_wheel(package: str, index_url: str | None = None) -> str:
     """Downloads the package using pip and returns the package name.
     If the package name cannot be determined, it returns the [package]."""
-    with Venv() as v, SecurePath.temporary_directory() as tmp_dir:
-        pip_result = v.pip_wheel(
+    with SecurePath.temporary_directory() as tmp_dir:
+        pip_result = pip_wheel(
             package_name=package,
             requirements_file=None,
             download_dir=tmp_dir.path,
             index_url=index_url,
             dependencies=False,
         )
         file_list = [
@@ -125,83 +128,169 @@
     - anaconda_packages - list of omitted packages
     - downloaded_packages - list of downloaded packages details
     """
     # pre-check of available packages to avoid potentially heavy downloads
     split_requirements = anaconda_packages.filter_available_packages(
         requirements, skip_version_check=skip_version_check
     )
-    omitted_packages = split_requirements.in_snowflake
+    packages_in_snowflake = split_requirements.in_snowflake
     requirements = split_requirements.unavailable
     if not requirements:
         # all packages are available in Snowflake
         return DownloadUnavailablePackagesResult(
             succeeded=True,
-            anaconda_packages=omitted_packages,
+            anaconda_packages=packages_in_snowflake,
         )
 
     # download all packages with their dependencies
-    with Venv() as v, SecurePath.temporary_directory() as downloads_dir:
+    with SecurePath.temporary_directory() as downloads_dir:
         # This is a Windows workaround where use TemporaryDirectory instead of NamedTemporaryFile
-        requirements_file = SecurePath(v.directory.name) / "requirements.txt"
+        requirements_file = downloads_dir / "requirements.txt"
         _write_requirements_file(requirements_file, requirements)  # type: ignore
-        pip_wheel_result = v.pip_wheel(
+        pip_wheel_result = pip_wheel(
             package_name=None,
             requirements_file=requirements_file.path,  # type: ignore
             download_dir=downloads_dir.path,
             index_url=pip_index_url,
             dependencies=True,
         )
         if pip_wheel_result != 0:
             log.info(_pip_failed_log_msg(pip_wheel_result))
             return DownloadUnavailablePackagesResult(
                 succeeded=False,
                 error_message=_pip_failed_log_msg(pip_wheel_result),
             )
 
-        # detect all downloaded packages
-        dependencies = v.get_package_dependencies(
-            requirements_file, downloads_dir=downloads_dir.path
+        # scan all downloaded packages and filter out ones available on Anaconda
+        dependencies = split_downloaded_dependencies(
+            requirements_file,
+            downloads_dir=downloads_dir.path,
+            anaconda_packages=anaconda_packages,
+            skip_version_check=skip_version_check,
         )
-        dependency_requirements = [d.requirement for d in dependencies]
         log.info(
             "Downloaded packages: %s",
-            ", ".join([d.name for d in dependency_requirements]),
-        )
-
-        # check whether some dependencies are available in Snowflake
-        log.info("Checking for dependencies available in Anaconda...")
-        split_dependencies = anaconda_packages.filter_available_packages(
-            packages=dependency_requirements, skip_version_check=skip_version_check
-        )
-        _log_dependencies_found_in_conda(split_dependencies.in_snowflake)
-        omitted_packages += split_dependencies.in_snowflake
-        dependencies_to_be_packed = _filter_dependencies_not_available_in_conda(
-            dependencies, split_dependencies.in_snowflake
+            ", ".join(
+                dep.requirement.name
+                for dep in dependencies.unavailable_dependencies_wheels
+            ),
         )
+        _log_dependencies_found_in_conda(dependencies.snowflake_dependencies)
+        packages_in_snowflake += dependencies.snowflake_dependencies
 
         # move filtered packages to target directory
         target_dir.mkdir(exist_ok=True)
-        for package in dependencies_to_be_packed:
+        for package in dependencies.unavailable_dependencies_wheels:
             package.extract_files(target_dir.path)
         return DownloadUnavailablePackagesResult(
             succeeded=True,
-            anaconda_packages=omitted_packages,
+            anaconda_packages=packages_in_snowflake,
             downloaded_packages_details=[
                 RequirementWithFiles(requirement=dep.requirement, files=dep.namelist())
-                for dep in dependencies_to_be_packed
+                for dep in dependencies.unavailable_dependencies_wheels
             ],
         )
 
 
-def _filter_dependencies_not_available_in_conda(
-    dependencies: List[RequirementWithWheelAndDeps],
-    available_in_conda: List[Requirement],
-) -> List[RequirementWithWheelAndDeps]:
-    in_conda = set(package.name for package in available_in_conda)
-    return [dep for dep in dependencies if dep.requirement.name not in in_conda]
+def pip_wheel(
+    requirements_file: Optional[str],
+    package_name: Optional[str],
+    download_dir: Path,
+    index_url: Optional[str],
+    dependencies: bool = True,
+):
+    command = ["-m", "pip", "wheel", "-w", str(download_dir)]
+    if package_name:
+        command.append(package_name)
+    if requirements_file:
+        command.extend(["-r", str(requirements_file)])
+    if index_url:
+        command.extend(["-i", index_url])
+    if not dependencies:
+        command.append("--no-deps")
+
+    try:
+        log.info(
+            "Running pip wheel with command: %s",
+            " ".join([str(com) for com in command]),
+        )
+        process = subprocess.run(
+            ["python", *command],
+            capture_output=True,
+            text=True,
+            encoding=locale.getpreferredencoding(),
+        )
+    except subprocess.CalledProcessError as e:
+        log.error("Encountered error %s", e.stderr)
+        raise ClickException(f"Encountered error while running pip wheel.")
+
+    log.info("Pip wheel command executed successfully")
+    return process.returncode
+
+
+@dataclasses.dataclass
+class SplitDownloadedDependenciesResult:
+    snowflake_dependencies: List[Requirement] = dataclasses.field(default_factory=list)
+    unavailable_dependencies_wheels: List[RequirementWithWheel] = dataclasses.field(
+        default_factory=list
+    )
+
+
+def split_downloaded_dependencies(
+    requirements_file: SecurePath,
+    downloads_dir: Path,
+    anaconda_packages: AnacondaPackages,
+    skip_version_check: bool,
+) -> SplitDownloadedDependenciesResult:
+    packages_metadata: Dict[str, WheelMetadata] = {
+        meta.name: meta
+        for meta in (
+            WheelMetadata.from_wheel(wheel_path)
+            for wheel_path in downloads_dir.glob("*.whl")
+        )
+        if meta is not None
+    }
+    available_in_snowflake_dependencies: Dict = {}
+    unavailable_dependencies: Dict = {}
+
+    def _get_dependencies(package: Requirement):
+        if (
+            package.name not in available_in_snowflake_dependencies
+            and package.name not in unavailable_dependencies
+        ):
+            if anaconda_packages.is_package_available(
+                package, skip_version_check=skip_version_check
+            ):
+                available_in_snowflake_dependencies[package.name] = package
+            else:
+                meta = packages_metadata.get(
+                    WheelMetadata.to_wheel_name_format(package.name)
+                )
+                wheel_path = meta.wheel_path if meta else None
+                requires = meta.dependencies if meta else []
+                unavailable_dependencies[package.name] = RequirementWithWheel(
+                    requirement=package,
+                    wheel_path=wheel_path,
+                )
+
+                log.debug(
+                    "Checking package %s, with dependencies: %s", package.name, requires
+                )
+
+                for package in requires:
+                    _get_dependencies(Requirement.parse_line(package))
+
+    with requirements_file.open("r", read_file_limit_mb=512) as req_file:
+        for line in req_file:
+            _get_dependencies(Requirement.parse_line(line))
+
+    return SplitDownloadedDependenciesResult(
+        snowflake_dependencies=list(available_in_snowflake_dependencies.values()),
+        unavailable_dependencies_wheels=list(unavailable_dependencies.values()),
+    )
 
 
 def detect_and_log_shared_libraries(dependencies: List[RequirementWithFiles]):
     shared_libraries = [
         dependency.requirement.name
         for dependency in dependencies
         if any(
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_package_paths.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/anaconda_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def is_package_available(
         self, package: Requirement, skip_version_check: bool = False
     ) -> bool:
         """
         Checks of a requirement is available in the Snowflake Anaconda Channel.
 
-        As snowflake currently doesn't support extra syntax (ex. `jinja2[diagrams]`), if such
+        As Snowflake currently doesn't support extra syntax (ex. `jinja2[diagrams]`), if such
         extra is present in the dependency, we mark it as unavailable.
         """
         if not package.name or package.extras:
             return False
         if package.name not in self._packages:
             return False
         if skip_version_check or not package.specs:
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/snowpark/package/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def upload(file: Path, stage: str, overwrite: bool):
     log.info("Uploading %s to Snowflake @%s/%s...", file, stage, file)
     with SecurePath.temporary_directory() as temp_dir:
         temp_app_zip_path = prepare_app_zip(SecurePath(file), temp_dir)
         sm = StageManager()
 
-        sm.create(sm.get_stage_name_from_path(stage))
+        sm.create(sm.get_stage_from_path(stage))
         put_response = sm.put(
             temp_app_zip_path.path, stage, overwrite=overwrite
         ).fetchone()
 
     message = f"Package {file} {put_response[6]} to Snowflake @{stage}/{file}."
 
     if put_response[6] == "SKIPPED":
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/__init__.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/common.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/compute_pool/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_registry/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_registry/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_repository/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/image_repository/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/services/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/spcs/services/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/sql/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/sql/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,55 @@
+from __future__ import annotations
+
+import sys
+from io import StringIO
 from pathlib import Path
-from typing import Optional
+from typing import Dict, Iterable, Optional, Tuple
+
+from click import ClickException, UsageError
+from jinja2 import UndefinedError
+from snowflake.cli.api.secure_path import UNLIMITED, SecurePath
+from snowflake.cli.api.sql_execution import SqlExecutionMixin
+from snowflake.cli.api.utils.rendering import snowflake_cli_jinja_render
+from snowflake.cli.plugins.sql.snowsql_templating import transpile_snowsql_templates
+from snowflake.connector.cursor import SnowflakeCursor
+from snowflake.connector.util_text import split_statements
+
+
+class SqlManager(SqlExecutionMixin):
+    def execute(
+        self,
+        query: Optional[str],
+        file: Optional[Path],
+        std_in: bool,
+        data: Dict | None = None,
+    ) -> Tuple[int, Iterable[SnowflakeCursor]]:
+        inputs = [query, file, std_in]
+        if not any(inputs):
+            raise UsageError("Use either query, filename or input option.")
+
+        # Check if any two inputs were provided simultaneously
+        if len([i for i in inputs if i]) > 1:
+            raise UsageError(
+                "Multiple input sources specified. Please specify only one."
+            )
+
+        if std_in:
+            query = sys.stdin.read()
+        elif file:
+            query = SecurePath(file).read_text(file_size_limit_mb=UNLIMITED)
+
+        if data:
+            # Do rendering if any data was provided
+            try:
+                query = transpile_snowsql_templates(query)
+                query = snowflake_cli_jinja_render(content=query, data=data)
+            except UndefinedError as err:
+                raise ClickException(f"SQL template rendering error: {err}")
+
+        statements = tuple(
+            statement
+            for statement, _ in split_statements(StringIO(query), remove_comments=True)
+        )
+        single_statement = len(statements) == 1
 
-import typer
-from snowflake.cli.api.commands.snow_typer import SnowTyper
-from snowflake.cli.api.output.types import CommandResult, MultipleResults, QueryResult
-from snowflake.cli.plugins.sql.manager import SqlManager
-
-# simple Typer with defaults because it won't become a command group as it contains only one command
-app = SnowTyper()
-
-
-@app.command(name="sql", requires_connection=True)
-def execute_sql(
-    query: Optional[str] = typer.Option(
-        None,
-        "--query",
-        "-q",
-        help="Query to execute.",
-    ),
-    file: Optional[Path] = typer.Option(
-        None,
-        "--filename",
-        "-f",
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-        readable=True,
-        help="File to execute.",
-    ),
-    std_in: Optional[bool] = typer.Option(
-        False,
-        "--stdin",
-        "-i",
-        help="Read the query from standard input. Use it when piping input to this command.",
-    ),
-    **options,
-) -> CommandResult:
-    """
-    Executes Snowflake query.
-
-    Query to execute can be specified using query option, filename option (all queries from file will be executed)
-    or via stdin by piping output from other command. For example `cat my.sql | snow sql -i`.
-    """
-    single_statement, cursors = SqlManager().execute(query, file, std_in)
-    if single_statement:
-        return QueryResult(next(cursors))
-    return MultipleResults((QueryResult(c) for c in cursors))
+        return single_statement, self._execute_string("\n".join(statements))
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     CollectionResult,
     CommandResult,
     ObjectResult,
     QueryResult,
     SingleQueryResult,
 )
 from snowflake.cli.api.utils.path_utils import is_stage_path
-from snowflake.cli.plugins.stage.diff import DiffResult
+from snowflake.cli.plugins.stage.diff import DiffResult, compute_stage_diff
 from snowflake.cli.plugins.stage.manager import OnErrorType, StageManager
 
 app = SnowTyper(
     name="stage",
     help="Manages stages.",
 )
 
@@ -121,22 +121,22 @@
 
     cursor = StageManager().remove(stage_name=stage_name, path=file_name)
     return SingleQueryResult(cursor)
 
 
 @app.command("diff", hidden=True, requires_connection=True)
 def stage_diff(
-    stage_name: str = typer.Argument(None, help="Fully qualified name of a stage"),
-    folder_name: str = typer.Argument(None, help="Path to local folder"),
+    stage_name: str = typer.Argument(help="Fully qualified name of a stage"),
+    folder_name: str = typer.Argument(help="Path to local folder"),
     **options,
 ) -> ObjectResult:
     """
     Diffs a stage with a local folder.
     """
-    diff: DiffResult = stage_diff(Path(folder_name), stage_name)
+    diff: DiffResult = compute_stage_diff(Path(folder_name), stage_name)
     return ObjectResult(str(diff))
 
 
 @app.command("execute", requires_connection=True)
 def execute(
     stage_path: str = typer.Argument(
         ...,
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/diff.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/diff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import hashlib
 import logging
 import re
 from dataclasses import dataclass, field
-from pathlib import Path
-from typing import Dict, List, Optional
+from pathlib import Path, PurePosixPath
+from typing import Collection, Dict, List, Optional
 
-from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
+from snowflake.cli.api.exceptions import (
+    SnowflakeSQLExecutionError,
+)
 from snowflake.cli.api.secure_path import UNLIMITED, SecurePath
-from snowflake.connector.cursor import SnowflakeCursor
+from snowflake.connector.cursor import DictCursor
 
 from .manager import StageManager
 
 MD5SUM_REGEX = r"^[A-Fa-f0-9]{32}$"
 CHUNK_SIZE_BYTES = 8192
 
 log = logging.getLogger(__name__)
 
+StagePath = PurePosixPath  # alias PurePosixPath as StagePath for clarity
+
 
 @dataclass
 class DiffResult:
     """
-    Each collection is a list of relative paths, either from
-    the stage root or from the root of the compared local directory.
+    Each collection is a list of stage paths ('/'-separated, regardless of the platform), relative to the stage root.
     """
 
-    identical: List[str] = field(default_factory=list)
+    identical: List[StagePath] = field(default_factory=list)
     "Files with matching md5sums"
 
-    different: List[str] = field(default_factory=list)
+    different: List[StagePath] = field(default_factory=list)
     "Files that may be different between the stage and the local directory"
 
-    only_local: List[str] = field(default_factory=list)
+    only_local: List[StagePath] = field(default_factory=list)
     "Files that only exist in the local directory"
 
-    only_on_stage: List[str] = field(default_factory=list)
+    only_on_stage: List[StagePath] = field(default_factory=list)
     "Files that only exist on the stage"
 
     def has_changes(self) -> bool:
         return (
             len(self.different) > 0
             or len(self.only_local) > 0
             or len(self.only_on_stage) > 0
@@ -66,24 +69,34 @@
             )
         if not self.identical:
             components.append(
                 "There are no existing files that are identical to the ones on the stage."
             )
 
         if self.only_local:
-            components.extend(["New files only on your local:", *self.only_local])
+            components.extend(
+                ["New files only on your local:", *[str(p) for p in self.only_local]]
+            )
         if self.only_on_stage:
-            components.extend(["New files only on the stage:", *self.only_on_stage])
+            components.extend(
+                ["New files only on the stage:", *[str(p) for p in self.only_on_stage]]
+            )
         if self.different:
             components.extend(
-                ["Existing files modified or status unknown:", *self.different]
+                [
+                    "Existing files modified or status unknown:",
+                    *[str(p) for p in self.different],
+                ]
             )
         if self.identical:
             components.extend(
-                ["Existing files identical to the stage:", *self.identical]
+                [
+                    "Existing files identical to the stage:",
+                    *[str(p) for p in self.identical],
+                ]
             )
 
         return "\n".join(components)
 
 
 def is_valid_md5sum(checksum: str) -> bool:
     """
@@ -135,135 +148,170 @@
             paths += enumerate_files(child)
         else:
             paths.append(child)
 
     return paths
 
 
-def strip_stage_name(path: str) -> str:
+def strip_stage_name(path: str) -> StagePath:
     """Returns the given stage path without the stage name as the first part."""
-    return "/".join(path.split("/")[1:])
+    return StagePath(*path.split("/")[1:])
 
 
-def build_md5_map(list_stage_cursor: SnowflakeCursor) -> Dict[str, str]:
+def build_md5_map(list_stage_cursor: DictCursor) -> Dict[StagePath, str]:
     """
     Returns a mapping of relative stage paths to their md5sums.
     """
     return {
-        strip_stage_name(name): md5
-        for (name, size, md5, modified) in list_stage_cursor.fetchall()
+        strip_stage_name(file["name"]): file["md5"]
+        for file in list_stage_cursor.fetchall()
     }
 
 
-def stage_diff(local_path: Path, stage_fqn: str) -> DiffResult:
+def preserve_from_diff(
+    diff: DiffResult, stage_paths_to_sync: Collection[StagePath]
+) -> DiffResult:
+    """
+    Returns a filtered version of the provided diff, keeping only the provided stage paths.
+    """
+    paths_to_preserve = set(stage_paths_to_sync)
+    preserved_diff: DiffResult = DiffResult()
+    preserved_diff.identical = [i for i in diff.identical if i in paths_to_preserve]
+    preserved_diff.different = [i for i in diff.different if i in paths_to_preserve]
+    preserved_diff.only_local = [i for i in diff.only_local if i in paths_to_preserve]
+    preserved_diff.only_on_stage = [
+        i for i in diff.only_on_stage if i in paths_to_preserve
+    ]
+    return preserved_diff
+
+
+def compute_stage_diff(
+    local_root: Path,
+    stage_fqn: str,
+) -> DiffResult:
     """
     Diffs the files in a stage with a local folder.
     """
     stage_manager = StageManager()
-    local_files = enumerate_files(local_path)
+    local_files = enumerate_files(local_root)
     remote_md5 = build_md5_map(stage_manager.list_files(stage_fqn))
 
     result: DiffResult = DiffResult()
 
     for local_file in local_files:
-        relpath = str(local_file.relative_to(local_path))
-        if relpath not in remote_md5:
+        relpath = local_file.relative_to(local_root)
+        stage_filename = to_stage_path(relpath)
+        if stage_filename not in remote_md5:
             # doesn't exist on the stage
-            result.only_local.append(relpath)
+            result.only_local.append(stage_filename)
         else:
             # N.B. we could compare local size vs remote size to skip the relatively-
             # expensive md5sum operation, but after seeing a comment that says the value
             # may not always be correctly populated, we'll ignore that column.
-            stage_md5sum = remote_md5[relpath]
+            stage_md5sum = remote_md5[stage_filename]
             if is_valid_md5sum(stage_md5sum) and stage_md5sum == compute_md5sum(
                 local_file
             ):
                 # the file definitely hasn't changed
-                result.identical.append(relpath)
+                result.identical.append(stage_filename)
             else:
                 # either the file has changed, or we can't tell if it has
-                result.different.append(relpath)
+                result.different.append(stage_filename)
 
             # mark this file as seen
-            del remote_md5[relpath]
+            del remote_md5[stage_filename]
 
     # every entry here is a file we never saw locally
-    for relpath in remote_md5.keys():
-        result.only_on_stage.append(relpath)
+    for stage_filename in remote_md5.keys():
+        result.only_on_stage.append(stage_filename)
 
     return result
 
 
-def get_stage_path_from_file(filepath: str):
-    parent = str(Path(filepath).parent)
-    stage_path = "" if parent == "." else parent
-    return stage_path
+def get_stage_subpath(stage_path: StagePath) -> str:
+    """
+    Returns the parent portion of a stage path, as a string, for inclusion in the fully qualified stage path. Note that
+    '.' treated specially here, and so the return value of this call is not a `StagePath` instance.
+    """
+    parent = str(stage_path.parent)
+    return "" if parent == "." else parent
+
+
+def to_stage_path(filename: Path) -> StagePath:
+    """
+    Returns the stage file name, with the path separator suitably transformed if needed.
+    """
+    return StagePath(*filename.parts)
+
+
+def to_local_path(stage_path: StagePath) -> Path:
+    return Path(*stage_path.parts)
 
 
 def delete_only_on_stage_files(
     stage_manager: StageManager,
     stage_fqn: str,
-    only_on_stage: List[str],
+    only_on_stage: List[StagePath],
     role: Optional[str] = None,
 ):
     """
     Deletes all files from a Snowflake stage according to the input list of filenames, using a custom role.
     """
-    for _file in only_on_stage:
-        stage_manager.remove(stage_name=stage_fqn, path=_file, role=role)
+    for _stage_filename in only_on_stage:
+        stage_manager.remove(stage_name=stage_fqn, path=str(_stage_filename), role=role)
 
 
 def put_files_on_stage(
     stage_manager: StageManager,
     stage_fqn: str,
     deploy_root_path: Path,
-    files: List[str],
+    stage_paths: List[StagePath],
     role: Optional[str] = None,
     overwrite: bool = False,
 ):
     """
     Uploads all files given input list of filenames on your local filesystem, to a Snowflake stage, using a custom role.
     """
-    for _file in files:
-        stage_sub_path = get_stage_path_from_file(_file)
+    for _stage_path in stage_paths:
+        stage_sub_path = get_stage_subpath(_stage_path)
         full_stage_path = (
             f"{stage_fqn}/{stage_sub_path}" if stage_sub_path else stage_fqn
         )
         stage_manager.put(
-            local_path=deploy_root_path / _file,
+            local_path=deploy_root_path / to_local_path(_stage_path),
             stage_path=full_stage_path,
             role=role,
             overwrite=overwrite,
         )
 
 
 def sync_local_diff_with_stage(
-    role: str, deploy_root_path: Path, diff_result: DiffResult, stage_path: str
+    role: str, deploy_root_path: Path, diff_result: DiffResult, stage_fqn: str
 ):
     """
     Syncs a given local directory's contents with a Snowflake stage, including removing old files, and re-uploading modified and new files.
     """
     stage_manager = StageManager()
     log.info(
         "Uploading diff-ed files from your local %s directory to the Snowflake stage.",
         deploy_root_path,
     )
 
     try:
         delete_only_on_stage_files(
-            stage_manager, stage_path, diff_result.only_on_stage, role
+            stage_manager, stage_fqn, diff_result.only_on_stage, role
         )
         put_files_on_stage(
             stage_manager,
-            stage_path,
+            stage_fqn,
             deploy_root_path,
             diff_result.different,
             role,
             overwrite=True,
         )
         put_files_on_stage(
-            stage_manager, stage_path, deploy_root_path, diff_result.only_local, role
+            stage_manager, stage_fqn, deploy_root_path, diff_result.only_local, role
         )
     except Exception as err:
         # Could be ProgrammingError or IntegrityError from SnowflakeCursor
         log.error(err)
         raise SnowflakeSQLExecutionError()
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/stage/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/stage/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contextlib import nullcontext
 from dataclasses import dataclass
 from os import path
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 from click import ClickException
-from snowflake.cli.api.commands.flags import OnErrorType
+from snowflake.cli.api.commands.flags import OnErrorType, parse_key_value_variables
 from snowflake.cli.api.console import cli_console
 from snowflake.cli.api.project.util import to_string_literal
 from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.api.utils.path_utils import path_resolver
 from snowflake.connector import DictCursor, ProgrammingError
 from snowflake.connector.cursor import SnowflakeCursor
@@ -24,21 +24,30 @@
 
 
 UNQUOTED_FILE_URI_REGEX = r"[\w/*?\-.=&{}$#[\]\"\\!@%^+:]+"
 EXECUTE_SUPPORTED_FILES_FORMATS = {".sql"}
 
 
 @dataclass
-class Variable:
-    key: str
-    value: str
-
-    def __init__(self, key: str, value: str):
-        self.key = key
-        self.value = value
+class StagePathParts:
+    # For path like @db.schema.stage/dir the values will be:
+    # stage = @db.schema.stage
+    stage: str
+    # stage_name = stage/dir
+    stage_name: str
+    # directory = dir
+    directory: str
+
+    @property
+    def path(self) -> str:
+        return (
+            f"{self.stage_name}{self.directory}".lower()
+            if self.stage_name.endswith("/")
+            else f"{self.stage_name}/{self.directory}".lower()
+        )
 
 
 class StageManager(SqlExecutionMixin):
     @staticmethod
     def get_standard_stage_prefix(name: str) -> str:
         # Handle embedded stages
         if name.startswith("@"):
@@ -52,15 +61,15 @@
     @staticmethod
     def get_standard_stage_directory_path(path):
         if not path.endswith("/"):
             path += "/"
         return StageManager.get_standard_stage_prefix(path)
 
     @staticmethod
-    def get_stage_name_from_path(path: str):
+    def get_stage_from_path(path: str):
         """
         Returns stage name from potential path on stage. For example
         db.schema.stage/foo/bar  -> db.schema.stage
         """
         return Path(path).parts[0]
 
     @staticmethod
@@ -192,52 +201,76 @@
 
     def execute(
         self,
         stage_path: str,
         on_error: OnErrorType,
         variables: Optional[List[str]] = None,
     ):
-        stage_path = self.get_standard_stage_prefix(stage_path)
-        all_files_list = self._get_files_list_from_stage(stage_path)
+        stage_path_with_prefix = self.get_standard_stage_prefix(stage_path)
+        stage_path_parts = self._split_stage_path(stage_path_with_prefix)
+        all_files_list = self._get_files_list_from_stage(stage_path_parts)
+
         # filter files from stage if match stage_path pattern
-        filtered_file_list = self._filter_files_list(stage_path, all_files_list)
+        filtered_file_list = self._filter_files_list(stage_path_parts, all_files_list)
 
         if not filtered_file_list:
             raise ClickException(f"No files matched pattern '{stage_path}'")
 
         # sort filtered files in alphabetical order with directories at the end
         sorted_file_list = sorted(
             filtered_file_list, key=lambda f: (path.dirname(f), path.basename(f))
         )
 
         sql_variables = self._parse_execute_variables(variables)
         results = []
         for file in sorted_file_list:
             results.append(
                 self._call_execute_immediate(
-                    file=file, variables=sql_variables, on_error=on_error
+                    stage_path_parts=stage_path_parts,
+                    file=file,
+                    variables=sql_variables,
+                    on_error=on_error,
                 )
             )
 
         return results
 
-    def _get_files_list_from_stage(self, stage_path: str) -> List[str]:
-        stage_name = self.get_stage_name_from_path(stage_path)
-        files_list_result = self.list_files(stage_name).fetchall()
+    def _split_stage_path(self, stage_path: str) -> StagePathParts:
+        """
+        Splits stage path `@stage/dir` to
+            stage -> @stage
+            stage_name -> stage
+            directory -> dir
+        For stage path with fully qualified name `@db.schema.stage/dir`
+            stage -> @db.schema.stage
+            stage_name -> stage
+            directory -> dir
+        """
+        stage = self.get_stage_from_path(stage_path)
+        stage_name = stage.split(".")[-1]
+        if stage_name.startswith("@"):
+            stage_name = stage_name[1:]
+        directory = "/".join(Path(stage_path).parts[1:])
+        return StagePathParts(stage, stage_name, directory)
+
+    def _get_files_list_from_stage(self, stage_path_parts: StagePathParts) -> List[str]:
+        files_list_result = self.list_files(stage_path_parts.stage).fetchall()
 
         if not files_list_result:
-            raise ClickException(f"No files found on stage '{stage_name}'")
+            raise ClickException(f"No files found on stage '{stage_path_parts.stage}'")
 
         return [f["name"] for f in files_list_result]
 
     def _filter_files_list(
-        self, stage_path: str, files_on_stage: List[str]
+        self, stage_path_parts: StagePathParts, files_on_stage: List[str]
     ) -> List[str]:
-        stage_path = self.remove_stage_prefix(stage_path)
-        stage_path = stage_path.lower()
+        if not stage_path_parts.directory:
+            return self._filter_supported_files(files_on_stage)
+
+        stage_path = stage_path_parts.path
 
         # Exact file path was provided if stage_path in file list
         if stage_path in files_on_stage:
             filtered_files = self._filter_supported_files([stage_path])
             if filtered_files:
                 return filtered_files
             else:
@@ -258,40 +291,38 @@
         return [f for f in files if Path(f).suffix in EXECUTE_SUPPORTED_FILES_FORMATS]
 
     @staticmethod
     def _parse_execute_variables(variables: Optional[List[str]]) -> Optional[str]:
         if not variables:
             return None
 
-        parsed_variables = StageManager._parse_variables(variables)
+        parsed_variables = parse_key_value_variables(variables)
         query_parameters = [f"{v.key}=>{v.value}" for v in parsed_variables]
         return f" using ({', '.join(query_parameters)})"
 
-    @staticmethod
-    def _parse_variables(variables: List[str]) -> List[Variable]:
-        result = []
-        for p in variables:
-            if "=" not in p:
-                raise ClickException(f"Invalid variable: '{p}'")
-
-            key, value = p.split("=", 1)
-            result.append(Variable(key.strip(), value.strip()))
-        return result
-
     def _call_execute_immediate(
-        self, file: str, variables: Optional[str], on_error: OnErrorType
+        self,
+        stage_path_parts: StagePathParts,
+        file: str,
+        variables: Optional[str],
+        on_error: OnErrorType,
     ) -> Dict:
+        file_stage_path = self._build_file_stage_path(stage_path_parts, file)
         try:
-            stage_path_prefixed = self.get_standard_stage_prefix(file)
-            query = (
-                f"execute immediate from {self.quote_stage_name(stage_path_prefixed)}"
-            )
+            query = f"execute immediate from {file_stage_path}"
             if variables:
                 query += variables
             self._execute_query(query)
-            cli_console.step(f"SUCCESS - {file}")
-            return {"File": file, "Status": "SUCCESS", "Error": None}
+            cli_console.step(f"SUCCESS - {file_stage_path}")
+            return {"File": file_stage_path, "Status": "SUCCESS", "Error": None}
         except ProgrammingError as e:
-            cli_console.warning(f"FAILURE - {file}")
+            cli_console.warning(f"FAILURE - {file_stage_path}")
             if on_error == OnErrorType.BREAK:
                 raise e
-            return {"File": file, "Status": "FAILURE", "Error": e.msg}
+            return {"File": file_stage_path, "Status": "FAILURE", "Error": e.msg}
+
+    def _build_file_stage_path(
+        self, stage_path_parts: StagePathParts, file: str
+    ) -> str:
+        stage = Path(stage_path_parts.stage).parts[0]
+        file_path = Path(file).parts[1:]
+        return f"{stage}/{'/'.join(file_path)}"
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/commands.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/streamlit/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/plugins/streamlit/manager.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/plugins/streamlit/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from pathlib import Path
 from typing import List, Optional
 
 from snowflake.cli.api.commands.experimental_behaviour import (
     experimental_behaviour_enabled,
 )
 from snowflake.cli.api.feature_flags import FeatureFlag
-from snowflake.cli.api.project.util import unquote_identifier
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
 from snowflake.cli.plugins.connection.util import (
     MissingConnectionHostError,
     make_snowsight_url,
 )
 from snowflake.cli.plugins.stage.manager import StageManager
 from snowflake.connector.cursor import SnowflakeCursor
@@ -184,13 +183,7 @@
         try:
             return make_snowsight_url(
                 self._conn,
                 f"/#/streamlit-apps/{self.qualified_name_for_url(streamlit_name, database=database, schema=schema)}",
             )
         except MissingConnectionHostError as e:
             return "https://app.snowflake.com"
-
-    def qualified_name_for_url(self, object_name: str, database=None, schema=None):
-        fqn = self.to_fully_qualified_name(
-            object_name, database=database, schema=schema
-        )
-        return ".".join(unquote_identifier(part) for part in fqn.split("."))
```

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py` & `snowflake_cli_labs-2.3.0rc0/src/snowflake/cli/templates/default_snowpark/app/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py` & `snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py` & `snowflake_cli_labs-2.3.0rc0/test_external_plugins/multilingual_hello_command_group/src/snowflakecli/test_plugins/multilingual_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py` & `snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py` & `snowflake_cli_labs-2.3.0rc0/test_external_plugins/snowpark_hello_single_command/src/snowflakecli/test_plugins/snowpark_hello/manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/conftest.py` & `snowflake_cli_labs-2.3.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_cli.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_command_registration.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_command_registration.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_common_decorators.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_common_decorators.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_common_global_context.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_common_global_context.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_config.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from tempfile import TemporaryDirectory
+from tempfile import NamedTemporaryFile, TemporaryDirectory
 from unittest import mock
 
 import pytest
 from snowflake.cli.api.config import (
     ConfigFileTooWidePermissionsError,
     config_init,
     get_config_section,
@@ -155,30 +155,36 @@
 
 
 def test_not_found_default_connection(test_root_path):
     config_init(Path(test_root_path / "empty_config.toml"))
     with pytest.raises(MissingConfiguration) as ex:
         get_default_connection_dict()
 
-    assert ex.value.message == "Connection default is not configured"
+    assert (
+        ex.value.message
+        == "Couldn't find connection for default connection `default`. Specify connection name or configure default connection."
+    )
 
 
 @mock.patch.dict(
     os.environ,
     {
         "SNOWFLAKE_DEFAULT_CONNECTION_NAME": "not_existed_connection",
     },
     clear=True,
 )
 def test_not_found_default_connection_from_evn_variable(test_root_path):
     config_init(Path(test_root_path / "empty_config.toml"))
     with pytest.raises(MissingConfiguration) as ex:
         get_default_connection_dict()
 
-    assert ex.value.message == "Connection not_existed_connection is not configured"
+    assert (
+        ex.value.message
+        == "Couldn't find connection for default connection `not_existed_connection`. Specify connection name or configure default connection."
+    )
 
 
 def test_connections_toml_override_config_toml(test_snowcli_config, snowflake_home):
     from snowflake.cli.api.config import CONFIG_MANAGER
 
     connections_toml = snowflake_home / "connections.toml"
     connections_toml.write_text(
@@ -277,7 +283,28 @@
     config_path.touch()
     config_path.chmod(0o777)
     connections_path = snowflake_home / "connections.toml"
     connections_path.touch()
     connections_path.chmod(0o777)
 
     config_init(test_snowcli_config)
+
+
+@pytest.mark.parametrize(
+    "content", ["[corrupted", "[connections.foo]\n[connections.foo]"]
+)
+def test_corrupted_config_raises_human_friendly_error(
+    snowflake_home, runner, content, snapshot
+):
+    with NamedTemporaryFile("w+", suffix=".toml") as tmp_file:
+        tmp_file.write(content)
+        tmp_file.flush()
+        result = runner.invoke_with_config_file(
+            tmp_file.name,
+            ["sql", "-q", "foo"],
+        )
+
+    # Run cli help to reset state after config load error
+    runner.invoke("--help")
+
+    assert result.exit_code == 1, result.output
+    assert result.output == snapshot
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_connection.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -363,14 +363,17 @@
         application="SNOWCLI.OBJECT.LIST",
         account="test_account",
         user="snowcli_test",
         password="top_secret",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
+        application_name="snowcli",
+        _internal_application_name="snowcli",
+        _internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch.dict(
     os.environ,
     {
         "PRIVATE_KEY_PASSPHRASE": "password",
@@ -442,14 +445,17 @@
         private_key=private_key,
         account="test_account",
         user="snowcli_test",
         authenticator="SNOWFLAKE_JWT",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
+        application_name="snowcli",
+        _internal_application_name="snowcli",
+        _internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch("snowflake.connector.connect")
 def test_session_and_master_tokens(mock_connector, mock_ctx, runner):
     ctx = mock_ctx()
     mock_connector.return_value = ctx
@@ -489,14 +495,17 @@
         account="test_account",
         user="snowcli_test",
         authenticator="SNOWFLAKE_JWT",
         database="test_dv",
         schema="PUBLIC",
         warehouse="xsmall",
         server_session_keep_alive=True,
+        application_name="snowcli",
+        _internal_application_name="snowcli",
+        _internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch.dict(
     os.environ,
     {
         "PRIVATE_KEY_PASSPHRASE": "password",
@@ -535,14 +544,17 @@
     mock_load.assert_called_once_with("~/sf_private_key.p8")
     mock_connector.assert_called_once_with(
         application="SNOWCLI.OBJECT.LIST",
         account="my_account",
         user="jdoe",
         authenticator="SNOWFLAKE_JWT",
         private_key="secret value",
+        application_name="snowcli",
+        _internal_application_name="snowcli",
+        _internal_application_version="0.0.0-test_patched",
     )
 
 
 @pytest.mark.parametrize(
     "command",
     [
         ["sql", "-q", "select 1"],
@@ -650,23 +662,26 @@
     mock_connect, env, test_snowcli_config, runner
 ):
     with mock.patch.dict(os.environ, env, clear=True):
 
         result = runner.invoke(["sql", "-q", "select 1", "-c", "empty"])
 
         assert result.exit_code == 0, result.output
-        args, kwargs = mock_connect.call_args
+        _, kwargs = mock_connect.call_args
         assert kwargs == {
             "account": "some_account",
             "application": "SNOWCLI.SQL",
             "database": "test_database",
             "warehouse": "large",
             "schema": "my_schema",
             "role": "role",
             "password": "dummy",
+            "application_name": "snowcli",
+            "_internal_application_name": "snowcli",
+            "_internal_application_version": "0.0.0-test_patched",
         }
 
 
 @pytest.mark.parametrize(
     "env",
     [
         {
@@ -708,23 +723,26 @@
                 "password_from_flag",
                 "--role",
                 "role_from_flag",
             ]
         )
 
         assert result.exit_code == 0, result.output
-        args, kwargs = mock_connect.call_args
+        _, kwargs = mock_connect.call_args
         assert kwargs == {
             "account": "account_from_flag",
             "application": "SNOWCLI.SQL",
             "database": "database_from_flag",
             "warehouse": "large",
             "schema": "schema_from_flag",
             "password": "password_from_flag",
             "role": "role_from_flag",
+            "application_name": "snowcli",
+            "_internal_application_name": "snowcli",
+            "_internal_application_version": "0.0.0-test_patched",
         }
 
 
 @mock.patch.dict(
     os.environ,
     {
         "SNOWFLAKE_CONNECTIONS_TEST_CONNECTIONS_ACCOUNT": "account_from_connection_env",
@@ -746,21 +764,24 @@
             "test_connections",
             "--account",
             "account_from_flag",
         ]
     )
 
     assert result.exit_code == 0, result.output
-    args, kwargs = mock_connect.call_args
+    _, kwargs = mock_connect.call_args
     assert kwargs == {
         "user": "python",  # from config
         "account": "account_from_flag",
         "application": "SNOWCLI.SQL",
         "database": "database_from_connection_env",
         "role": "role_from_global_env",
+        "application_name": "snowcli",
+        "_internal_application_name": "snowcli",
+        "_internal_application_version": "0.0.0-test_patched",
     }
 
 
 def test_set_default_connection_fails_if_no_connection(runner):
     with NamedTemporaryFile("w+", suffix=".toml") as tmp_file:
         result = runner.invoke_with_config_file(
             tmp_file.name, ["connection", "set-default", "foo"]
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_experimental_behaviour.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_experimental_behaviour.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_help_messages.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_help_messages.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_logs.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_main.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import sys
 import typing as t
 from pathlib import Path
 from unittest import mock
 
 import pytest
 from click import Command
-from snowflake.cli.__about__ import VERSION
 from snowflake.cli.app.cli_app import app_context_holder
 from snowflake.connector.config_manager import CONFIG_MANAGER
 from typer.core import TyperArgument, TyperOption
 
 
 def test_help_option(runner):
     result = runner.invoke(["--help"])
@@ -45,26 +44,33 @@
     mock_conn.assert_called_once_with(
         application="SNOWCLI.OBJECT.LIST",
         database="db_for_test",
         schema="test_public",
         role="test_role",
         warehouse="xs",
         password="dummy_password",
+        application_name="snowcli",
+        _internal_application_name="snowcli",
+        _internal_application_version="0.0.0-test_patched",
     )
 
 
 def test_info_callback(runner):
     result = runner.invoke(["--info"])
     assert result.exit_code == 0, result.output
     payload = json.loads(result.output)
     assert payload == [
-        {"key": "version", "value": VERSION},
+        {"key": "version", "value": "0.0.0-test_patched"},
         {"key": "default_config_file_path", "value": str(CONFIG_MANAGER.file_path)},
         {"key": "python_version", "value": sys.version},
         {"key": "system_info", "value": platform.platform()},
+        {
+            "key": "feature_flags",
+            "value": {"dummy_flag": True, "wrong_type_flag": "UNKNOWN"},
+        },
     ]
 
 
 def test_docs_callback(runner):
     result = runner.invoke(["--docs"])
     assert result.exit_code == 0, result.output
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_project_initialisation.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_project_initialisation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_snow_connector.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_snow_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     mock_connect.assert_called_once_with(
         application=expected,
         database="db_for_test",
         schema="test_public",
         role="test_role",
         warehouse="xs",
         password="dummy_password",
+        application_name="snowcli",
+        _internal_application_name="snowcli",
+        _internal_application_version="0.0.0-test_patched",
     )
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_returns_nice_error_in_case_of_connectivity_error(runner):
     result = runner.invoke(["sql", "-q", "select 1"])
     assert result.exit_code == 1
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_sql.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_sql.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from unittest import mock
 
 import pytest
 from snowflake.cli.api.constants import ObjectType
 from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
 from snowflake.cli.api.project.util import identifier_to_show_like_pattern
 from snowflake.cli.api.sql_execution import SqlExecutionMixin
+from snowflake.cli.plugins.sql.snowsql_templating import transpile_snowsql_templates
 from snowflake.connector.cursor import DictCursor
 from snowflake.connector.errors import ProgrammingError
 
 from tests.testing_utils.result_assertions import assert_that_result_is_usage_error
 
 
 @mock.patch("snowflake.cli.plugins.sql.manager.SqlExecutionMixin._execute_string")
@@ -266,7 +267,61 @@
         ObjectType.DATABASE,
     ],
 )
 @mock.patch("snowflake.cli.api.sql_execution.SqlExecutionMixin._execute_query")
 def test_use_command(mock_execute_query, _object):
     SqlExecutionMixin().use(object_type=_object, name="foo_name")
     mock_execute_query.assert_called_once_with(f"use {_object.value.sf_name} foo_name")
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        "select &{ aaa }.&{ bbb }",
+        "select &aaa.&bbb",
+        "select &aaa.&{ bbb }",
+    ],
+)
+@mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
+def test_rendering_of_sql(mock_execute_query, query, runner):
+    result = runner.invoke(["sql", "-q", query, "-D", "aaa=foo", "-D", "bbb=bar"])
+    assert result.exit_code == 0, result.output
+    mock_execute_query.assert_called_once_with("select foo.bar")
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        "select &{ aaa }.&{ bbb }",
+        "select &aaa.&bbb",
+        "select &aaa.&{ bbb }",
+    ],
+)
+@mock.patch("snowflake.cli.plugins.sql.commands.SqlManager._execute_string")
+def test_no_rendering_of_sql_if_no_data(mock_execute_query, query, runner):
+    result = runner.invoke(["sql", "-q", query])
+    assert result.exit_code == 0, result.output
+    mock_execute_query.assert_called_once_with(query)
+
+
+@pytest.mark.parametrize("query", ["select &{ foo }", "select &foo"])
+def test_execution_fails_if_unknown_variable(runner, query):
+    result = runner.invoke(["sql", "-q", query, "-D", "bbb=1"])
+    assert "SQL template rendering error: 'foo' is undefined" in result.output
+
+
+@pytest.mark.parametrize(
+    "text, expected",
+    [
+        # Test escaping
+        ("&&foo", "&foo"),
+        ("select *  from &&foo join bar", "select *  from &foo join bar"),
+        # Test basic usage
+        ("&foo", "&{ foo }"),
+        ("select *  from &foo join bar", "select *  from &{ foo } join bar"),
+        # Test templating is ignored
+        ("&{ foo }", "&{ foo }"),
+        ("select *  from &{ foo } join bar", "select *  from &{ foo } join bar"),
+    ],
+)
+def test_snowsql_compatibility(text, expected):
+    assert transpile_snowsql_templates(text) == expected
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 )
 def test_path_resolver(mock_system, argument, expected):
     mock_system.response_value = "Windows"
 
     assert path_utils.path_resolver(argument) == expected
 
 
-@patch("snowflake.cli.plugins.snowpark.package_utils.Venv.pip_wheel")
+@patch("snowflake.cli.plugins.snowpark.package_utils.pip_wheel")
 def test_pip_fail_message(mock_installer, correct_requirements_txt, caplog):
     mock_installer.return_value = 42
 
     with caplog.at_level(logging.INFO, "snowflake.cli.plugins.snowpark.package_utils"):
         requirements = package_utils.parse_requirements(
             SecurePath(correct_requirements_txt)
         )
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_zipper.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_zipper.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_connection.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/__snapshots__/test_connection.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/__snapshots__/test_help_messages.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/__snapshots__/test_help_messages.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -55,23 +55,44 @@
   
   
   '''
 # ---
 # name: test_help_messages[app.deploy]
   '''
                                                                                   
-   Usage: default app deploy [OPTIONS]                                            
+   Usage: default app deploy [OPTIONS] [FILES]...                                 
                                                                                   
    Creates an application package in your Snowflake account and syncs the local   
-   changes to the stage without creating or updating the application.             
-                                                                                  
-  ╭─ Options ────────────────────────────────────────────────────────────────────╮
-  │ --project  -p      TEXT  Path where the Snowflake Native App project         │
-  │                          resides. Defaults to current working directory.     │
-  │ --help     -h            Show this message and exit.                         │
+   changes to the stage without creating or updating the application. Running     
+   this command with no arguments at all, as in `snow app deploy`, is a shorthand 
+   for `snow app deploy --prune --recursive`.                                     
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │   files      [FILES]...  Paths, relative to the the project root, of files   │
+  │                          you want to upload to a stage. The paths must match │
+  │                          one of the artifacts src pattern entries in         │
+  │                          snowflake.yml. If unspecified, the command syncs    │
+  │                          all local changes to the stage.                     │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --prune          --no-prune          Whether to delete specified files from  │
+  │                                      the stage if they don't exist locally.  │
+  │                                      If set, the command deletes files that  │
+  │                                      exist in the stage, but not in the      │
+  │                                      local filesystem.                       │
+  │                                      [default: no-prune]                     │
+  │ --recursive  -r                      Whether to traverse and deploy files    │
+  │                                      from subdirectories. If set, the        │
+  │                                      command deploys all files and           │
+  │                                      subdirectories; otherwise, only files   │
+  │                                      in the current directory are deployed.  │
+  │ --project    -p                TEXT  Path where the Snowflake Native App     │
+  │                                      project resides. Defaults to current    │
+  │                                      working directory.                      │
+  │ --help       -h                      Show this message and exit.             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
   │                                           account. Overrides the value       │
@@ -737,15 +758,17 @@
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Commands ───────────────────────────────────────────────────────────────────╮
   │ deploy     Creates an application package in your Snowflake account and      │
   │            syncs the local changes to the stage without creating or updating │
-  │            the application.                                                  │
+  │            the application. Running this command with no arguments at all,   │
+  │            as in `snow app deploy`, is a shorthand for `snow app deploy      │
+  │            --prune --recursive`.                                             │
   │ init       Initializes a Snowflake Native App project.                       │
   │ open       Opens the Snowflake Native App inside of your browser, once it    │
   │            has been installed in your account.                               │
   │ run        Creates an application package in your Snowflake account, uploads │
   │            code files to its stage, then creates or upgrades an application  │
   │            object from the application package.                              │
   │ teardown   Attempts to drop both the application object and application      │
@@ -1081,15 +1104,15 @@
   '''
 # ---
 # name: test_help_messages[git.fetch]
   '''
                                                                                   
    Usage: default git fetch [OPTIONS] REPOSITORY_NAME                             
                                                                                   
-   Fetch changes from origin to snowflake repository.                             
+   Fetch changes from origin to Snowflake repository.                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
   │ *    repository_name      TEXT  Identifier of the git repository. For        │
   │                                 example: my_repo                             │
   │                                 [default: None]                              │
   │                                 [required]                                   │
   ╰──────────────────────────────────────────────────────────────────────────────╯
@@ -1468,24 +1491,256 @@
   │ copy            Copies all files from given state of repository to local     │
   │                 directory or stage.                                          │
   │ execute         Execute immediate all files from the repository path. Files  │
   │                 can be filtered with glob like pattern, e.g.                 │
   │                 `@my_repo/branches/main/*.sql`,                              │
   │                 `@my_repo/branches/main/dev/*`. Only files with `.sql`       │
   │                 extension will be executed.                                  │
-  │ fetch           Fetch changes from origin to snowflake repository.           │
+  │ fetch           Fetch changes from origin to Snowflake repository.           │
   │ list-branches   List all branches in the repository.                         │
   │ list-files      List files from given state of git repository.               │
   │ list-tags       List all tags in the repository.                             │
   │ setup           Sets up a git repository object.                             │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   
   
   '''
 # ---
+# name: test_help_messages[notebook.execute]
+  '''
+                                                                                  
+   Usage: default notebook execute [OPTIONS] IDENTIFIER                           
+                                                                                  
+   Executes a notebook in a headless mode.                                        
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    identifier      TEXT  Identifier of the notebook. For example:          │
+  │                            MY_NOTEBOOK                                       │
+  │                            [default: None]                                   │
+  │                            [required]                                        │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[notebook.get-url]
+  '''
+                                                                                  
+   Usage: default notebook get-url [OPTIONS] IDENTIFIER                           
+                                                                                  
+   Return a url to a notebook.                                                    
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    identifier      TEXT  Identifier of the notebook. For example:          │
+  │                            MY_NOTEBOOK                                       │
+  │                            [default: None]                                   │
+  │                            [required]                                        │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[notebook.open]
+  '''
+                                                                                  
+   Usage: default notebook open [OPTIONS] IDENTIFIER                              
+                                                                                  
+   Opens a notebook in default browser                                            
+                                                                                  
+  ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
+  │ *    identifier      TEXT  Identifier of the notebook. For example:          │
+  │                            MY_NOTEBOOK                                       │
+  │                            [default: None]                                   │
+  │                            [required]                                        │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Connection configuration ───────────────────────────────────────────────────╮
+  │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
+  │                                           in your `config.toml`. Default:    │
+  │                                           `default`.                         │
+  │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
+  │                                           account. Overrides the value       │
+  │                                           specified for the connection.      │
+  │ --user,--username                   TEXT  Username to connect to Snowflake.  │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --password                          TEXT  Snowflake password. Overrides the  │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --authenticator                     TEXT  Snowflake authenticator. Overrides │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --private-key-path                  TEXT  Snowflake private key path.        │
+  │                                           Overrides the value specified for  │
+  │                                           the connection.                    │
+  │ --database,--dbname                 TEXT  Database to use. Overrides the     │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --schema,--schemaname               TEXT  Database schema to use. Overrides  │
+  │                                           the value specified for the        │
+  │                                           connection.                        │
+  │ --role,--rolename                   TEXT  Role to use. Overrides the value   │
+  │                                           specified for the connection.      │
+  │ --warehouse                         TEXT  Warehouse to use. Overrides the    │
+  │                                           value specified for the            │
+  │                                           connection.                        │
+  │ --temporary-connection      -x            Uses connection defined with       │
+  │                                           command line parameters, instead   │
+  │                                           of one defined in config           │
+  │ --mfa-passcode                      TEXT  Token to use for multi-factor      │
+  │                                           authentication (MFA)               │
+  │ --enable-diag                             Run python connector diagnostic    │
+  │                                           test                               │
+  │ --diag-log-path                     TEXT  Diagnostic report path             │
+  │ --diag-allowlist-path               TEXT  Diagnostic report path to optional │
+  │                                           allowlist                          │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Global configuration ───────────────────────────────────────────────────────╮
+  │ --format           [TABLE|JSON]  Specifies the output format.                │
+  │                                  [default: TABLE]                            │
+  │ --verbose  -v                    Displays log entries for log levels `info`  │
+  │                                  and higher.                                 │
+  │ --debug                          Displays log entries for log levels `debug` │
+  │                                  and higher; debug logs contains additional  │
+  │                                  information.                                │
+  │ --silent                         Turns off intermediate output to console.   │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
+# name: test_help_messages[notebook]
+  '''
+                                                                                  
+   Usage: default notebook [OPTIONS] COMMAND [ARGS]...                            
+                                                                                  
+   Manages notebooks in Snowflake.                                                
+                                                                                  
+  ╭─ Options ────────────────────────────────────────────────────────────────────╮
+  │ --help  -h        Show this message and exit.                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  ╭─ Commands ───────────────────────────────────────────────────────────────────╮
+  │ execute   Executes a notebook in a headless mode.                            │
+  │ get-url   Return a url to a notebook.                                        │
+  │ open      Opens a notebook in default browser                                │
+  ╰──────────────────────────────────────────────────────────────────────────────╯
+  
+  
+  '''
+# ---
 # name: test_help_messages[object.describe]
   '''
                                                                                   
    Usage: default object describe [OPTIONS] OBJECT_TYPE OBJECT_NAME               
                                                                                   
    Provides description of an object of given type.                               
    Supported types: compute-pool, database, function, git-repository,             
@@ -4816,20 +5071,26 @@
                                                                                   
    Usage: default sql [OPTIONS]                                                   
                                                                                   
    Executes Snowflake query.                                                      
    Query to execute can be specified using query option, filename option (all     
    queries from file will be executed) or via stdin by piping output from other   
    command. For example `cat my.sql | snow sql -i`.                               
+   The command supports variable substitution that happens on client-side. Both   
+   $VARIABLE or ${ VARIABLE } syntax are supported.                               
                                                                                   
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --query     -q      TEXT  Query to execute. [default: None]                  │
   │ --filename  -f      FILE  File to execute. [default: None]                   │
   │ --stdin     -i            Read the query from standard input. Use it when    │
   │                           piping input to this command.                      │
+  │ --data      -D      TEXT  String in format of key=value. If provided the SQL │
+  │                           content will be treated as template and rendered   │
+  │                           using provided data.                               │
+  │                           [default: None]                                    │
   │ --help      -h            Show this message and exit.                        │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
   │                                           `default`.                         │
   │ --account,--accountname             TEXT  Name assigned to your Snowflake    │
@@ -5034,22 +5295,22 @@
   
   
   '''
 # ---
 # name: test_help_messages[stage.diff]
   '''
                                                                                   
-   Usage: default stage diff [OPTIONS] [STAGE_NAME] [FOLDER_NAME]                 
+   Usage: default stage diff [OPTIONS] STAGE_NAME FOLDER_NAME                     
                                                                                   
    Diffs a stage with a local folder.                                             
                                                                                   
   ╭─ Arguments ──────────────────────────────────────────────────────────────────╮
-  │   stage_name       [STAGE_NAME]   Fully qualified name of a stage            │
-  │                                   [default: None]                            │
-  │   folder_name      [FOLDER_NAME]  Path to local folder [default: None]       │
+  │ *    stage_name       TEXT  Fully qualified name of a stage [default: None]  │
+  │                             [required]                                       │
+  │ *    folder_name      TEXT  Path to local folder [default: None] [required]  │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Options ────────────────────────────────────────────────────────────────────╮
   │ --help  -h        Show this message and exit.                                │
   ╰──────────────────────────────────────────────────────────────────────────────╯
   ╭─ Connection configuration ───────────────────────────────────────────────────╮
   │ --connection,--environment  -c      TEXT  Name of the connection, as defined │
   │                                           in your `config.toml`. Default:    │
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/test_feature_flags.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/test_secure_path.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/test_secure_path.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_flags.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/commands/test_flags.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/commands/test_snow_typer.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/commands/test_snow_typer.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_flags.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/api/commands/__snapshots__/test_flags.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/api/commands/__snapshots__/test_snow_typer.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_cli_console_output.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/console/test_cli_console_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_console_abc.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/console/test_console_abc.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/api/console/test_intermediate_output.py` & `snowflake_cli_labs-2.3.0rc0/tests/api/console/test_intermediate_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/git/test_git_commands.py` & `snowflake_cli_labs-2.3.0rc0/tests/git/test_git_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,45 +396,69 @@
         origin = 'https://github.com/an-example-repo.git'
         git_credentials = repo_name_secret
         """
     )
 
 
 @pytest.mark.parametrize(
-    "repository_path, expected_files",
+    "repository_path, expected_stage, expected_files",
     [
         (
             "@repo/branches/main/",
-            ["repo/branches/main/s1.sql", "repo/branches/main/a/s3.sql"],
+            "@repo/branches/main/",
+            ["@repo/branches/main/s1.sql", "@repo/branches/main/a/s3.sql"],
         ),
         (
             "@repo/branches/main/a",
-            ["repo/branches/main/a/s3.sql"],
+            "@repo/branches/main/",
+            ["@repo/branches/main/a/s3.sql"],
+        ),
+        (
+            "@db.schema.repo/branches/main/",
+            "@db.schema.repo/branches/main/",
+            [
+                "@db.schema.repo/branches/main/s1.sql",
+                "@db.schema.repo/branches/main/a/s3.sql",
+            ],
+        ),
+        (
+            "@db.schema.repo/branches/main/s1.sql",
+            "@db.schema.repo/branches/main/",
+            ["@db.schema.repo/branches/main/s1.sql"],
         ),
     ],
 )
 @mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_execute(mock_execute, mock_cursor, runner, repository_path, expected_files):
+def test_execute(
+    mock_execute,
+    mock_cursor,
+    runner,
+    repository_path,
+    expected_stage,
+    expected_files,
+    snapshot,
+):
     mock_execute.return_value = mock_cursor(
         [
             {"name": "repo/branches/main/a/s3.sql"},
             {"name": "repo/branches/main/s1.sql"},
             {"name": "repo/branches/main/s2"},
         ],
         [],
     )
 
     result = runner.invoke(["git", "execute", repository_path])
 
     assert result.exit_code == 0, result.output
     ls_call, *execute_calls = mock_execute.mock_calls
-    assert ls_call == mock.call(f"ls @repo/branches/main/", cursor_class=DictCursor)
+    assert ls_call == mock.call(f"ls {expected_stage}", cursor_class=DictCursor)
     assert execute_calls == [
-        mock.call(f"execute immediate from @{p}") for p in expected_files
+        mock.call(f"execute immediate from {p}") for p in expected_files
     ]
+    assert result.output == snapshot
 
 
 @mock.patch(f"{STAGE_MANAGER}._execute_query")
 def test_execute_with_variables(mock_execute, mock_cursor, runner):
     mock_execute.return_value = mock_cursor([{"name": "repo/branches/main/s1.sql"}], [])
 
     result = runner.invoke(
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/patch_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/patch_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_artifacts.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_artifacts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import os
 from pathlib import Path
 from typing import List, Optional
 
 import pytest
+from click.exceptions import ClickException
 from snowflake.cli.api.project.definition import load_project_definition
 from snowflake.cli.plugins.nativeapp.artifacts import (
     ArtifactMapping,
     DeployRootError,
     GlobMatchedNothingError,
     NotInDeployRootError,
     SourceNotFoundError,
     TooManyFilesError,
     build_bundle,
+    resolve_without_follow,
+    source_path_to_deploy_path,
     translate_artifact,
 )
 
+from tests.nativeapp.utils import touch
+
 
 def trimmed_contents(path: Path) -> Optional[str]:
     if not path.is_file():
         return None
     with open(path, "r") as handle:
         return handle.read().strip()
 
@@ -159,7 +165,64 @@
         build_bundle(
             project_root,
             deploy_root=Path(project_root, "deploy"),
             artifacts=[
                 ArtifactMapping("app/streamlit/*.py", "somehow_combined_streamlits.py")
             ],
         )
+
+
+@pytest.mark.parametrize(
+    "project_path,expected_path",
+    [
+        [
+            "srcfile",
+            "deploy/file",
+        ],
+        [
+            "srcdir",
+            "deploy/dir",
+        ],
+        [
+            "srcdir/nested_file1",
+            "deploy/dir/nested_file1",
+        ],
+        [
+            "srcdir/nested_dir/nested_file2",
+            "deploy/dir/nested_dir/nested_file2",
+        ],
+        [
+            "srcdir/nested_dir",
+            "deploy/dir/nested_dir",
+        ],
+        [
+            "not-in-deploy",
+            None,
+        ],
+    ],
+)
+def test_source_path_to_deploy_path(
+    temp_dir,
+    project_path,
+    expected_path,
+):
+    # Source files
+    touch("srcfile")
+    touch("srcdir/nested_file1")
+    touch("srcdir/nested_dir/nested_file2")
+    touch("not-in-deploy")
+    # Build
+    os.mkdir("deploy")
+    os.symlink("srcfile", "deploy/file")
+    os.symlink(Path("srcdir").resolve(), Path("deploy/dir"))
+
+    files_mapping = {
+        Path("srcdir").resolve(): resolve_without_follow(Path("deploy/dir")),
+        Path("srcfile").resolve(): resolve_without_follow(Path("deploy/file")),
+    }
+
+    if expected_path:
+        result = source_path_to_deploy_path(Path(project_path).resolve(), files_mapping)
+        assert result == resolve_without_follow(Path(expected_path))
+    else:
+        with pytest.raises(ClickException):
+            source_path_to_deploy_path(Path(project_path).resolve(), files_mapping)
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_commands.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_init.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_init.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_manager.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 
 import pytest
 from snowflake.cli.api.project.definition_manager import DefinitionManager
 from snowflake.cli.plugins.nativeapp.constants import (
     LOOSE_FILES_MAGIC_VERSION,
@@ -13,31 +14,36 @@
 from snowflake.cli.plugins.nativeapp.exceptions import (
     ApplicationPackageAlreadyExistsError,
     UnexpectedOwnerError,
 )
 from snowflake.cli.plugins.nativeapp.manager import (
     NativeAppManager,
     SnowflakeSQLExecutionError,
+    _get_stage_paths_to_sync,
     ensure_correct_owner,
 )
-from snowflake.cli.plugins.stage.diff import DiffResult
+from snowflake.cli.plugins.stage.diff import (
+    DiffResult,
+    StagePath,
+)
 from snowflake.connector import ProgrammingError
 from snowflake.connector.cursor import DictCursor
 
 from tests.nativeapp.patch_utils import (
     mock_connection,
     mock_get_app_pkg_distribution_in_sf,
 )
 from tests.nativeapp.utils import (
     NATIVEAPP_MANAGER_EXECUTE,
     NATIVEAPP_MANAGER_GET_EXISTING_APP_PKG_INFO,
     NATIVEAPP_MANAGER_IS_APP_PKG_DISTRIBUTION_SAME,
     NATIVEAPP_MODULE,
     mock_execute_helper,
     mock_snowflake_yml_file,
+    touch,
 )
 from tests.testing_utils.files_and_dirs import create_named_file
 
 mock_project_definition_override = {
     "native_app": {
         "application": {
             "name": "sample_application_name",
@@ -56,56 +62,110 @@
     return NativeAppManager(
         project_definition=dm.project_definition.native_app,
         project_root=dm.project_root,
     )
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
-@mock.patch(f"{NATIVEAPP_MODULE}.stage_diff")
+@mock.patch(f"{NATIVEAPP_MODULE}.compute_stage_diff")
 @mock.patch(f"{NATIVEAPP_MODULE}.sync_local_diff_with_stage")
 def test_sync_deploy_root_with_stage(
-    mock_local_diff_with_stage, mock_stage_diff, mock_execute, temp_dir, mock_cursor
+    mock_local_diff_with_stage,
+    mock_compute_stage_diff,
+    mock_execute,
+    temp_dir,
+    mock_cursor,
 ):
     mock_execute.return_value = mock_cursor([{"CURRENT_ROLE()": "old_role"}], [])
-    mock_diff_result = DiffResult(different=["setup.sql"])
-    mock_stage_diff.return_value = mock_diff_result
+    mock_diff_result = DiffResult(different=[StagePath("setup.sql")])
+    mock_compute_stage_diff.return_value = mock_diff_result
     mock_local_diff_with_stage.return_value = None
     current_working_directory = os.getcwd()
     create_named_file(
         file_name="snowflake.yml",
         dir_name=current_working_directory,
         contents=[mock_snowflake_yml_file],
     )
 
     native_app_manager = _get_na_manager()
     assert mock_diff_result.has_changes()
-    native_app_manager.sync_deploy_root_with_stage("new_role")
+    native_app_manager.sync_deploy_root_with_stage("new_role", True, True)
 
     expected = [
         mock.call("select current_role()", cursor_class=DictCursor),
         mock.call("use role new_role"),
         mock.call(f"create schema if not exists app_pkg.app_src"),
         mock.call(
             f"""
                     create stage if not exists app_pkg.app_src.stage
                     encryption = (TYPE = 'SNOWFLAKE_SSE')
                     DIRECTORY = (ENABLE = TRUE)"""
         ),
         mock.call("use role old_role"),
     ]
     assert mock_execute.mock_calls == expected
-    mock_stage_diff.assert_called_once_with(
+    mock_compute_stage_diff.assert_called_once_with(
         native_app_manager.deploy_root, "app_pkg.app_src.stage"
     )
     mock_local_diff_with_stage.assert_called_once_with(
         role="new_role",
         deploy_root_path=native_app_manager.deploy_root,
         diff_result=mock_diff_result,
-        stage_path="app_pkg.app_src.stage",
+        stage_fqn="app_pkg.app_src.stage",
+    )
+
+
+@mock.patch(NATIVEAPP_MANAGER_EXECUTE)
+@mock.patch(f"{NATIVEAPP_MODULE}.sync_local_diff_with_stage")
+@mock.patch(f"{NATIVEAPP_MODULE}.compute_stage_diff")
+@mock.patch(f"{NATIVEAPP_MODULE}.cc.warning")
+@pytest.mark.parametrize(
+    "prune,only_on_stage_files,expected_warn",
+    [
+        [
+            True,
+            ["only-stage.txt"],
+            False,
+        ],
+        [
+            False,
+            ["only-stage-1.txt", "only-stage-2.txt"],
+            True,
+        ],
+    ],
+)
+def test_sync_deploy_root_with_stage_prune(
+    mock_warning,
+    mock_compute_stage_diff,
+    mock_local_diff_with_stage,
+    mock_execute,
+    prune,
+    only_on_stage_files,
+    expected_warn,
+    temp_dir,
+):
+    mock_compute_stage_diff.return_value = DiffResult(only_on_stage=only_on_stage_files)
+    create_named_file(
+        file_name="snowflake.yml",
+        dir_name=os.getcwd(),
+        contents=[mock_snowflake_yml_file],
     )
+    native_app_manager = _get_na_manager()
+
+    native_app_manager.sync_deploy_root_with_stage("role", prune, True)
+
+    if expected_warn:
+        files_str = "\n".join(only_on_stage_files)
+        warn_message = f"""The following files exist only on the stage:
+{files_str}
+
+Use the --prune flag to delete them from the stage."""
+        mock_warning.assert_called_once_with(warn_message)
+    else:
+        mock_warning.assert_not_called()
 
 
 @mock.patch(NATIVEAPP_MANAGER_EXECUTE)
 def test_get_app_pkg_distribution_in_snowflake(mock_execute, temp_dir, mock_cursor):
 
     side_effects, expected = mock_execute_helper(
         [
@@ -712,7 +772,36 @@
     with pytest.raises(ApplicationPackageAlreadyExistsError):
         native_app_manager.create_app_package()
 
     if not is_pkg_distribution_same:
         mock_warning.assert_called_once_with(
             "Continuing to execute `snow app run` on application package app_pkg with distribution 'internal'."
         )
+
+
+@pytest.mark.parametrize(
+    "paths_to_sync,expected_result",
+    [
+        [
+            ["deploy/dir"],
+            ["dir/nested_file1", "dir/nested_file2", "dir/nested_dir/nested_file3"],
+        ],
+        [["deploy/dir/nested_dir"], ["dir/nested_dir/nested_file3"]],
+        [
+            ["deploy/file", "deploy/dir/nested_dir/nested_file3"],
+            ["file", "dir/nested_dir/nested_file3"],
+        ],
+    ],
+)
+def test_get_paths_to_sync(
+    temp_dir,
+    paths_to_sync,
+    expected_result,
+):
+    touch("deploy/file")
+    touch("deploy/dir/nested_file1")
+    touch("deploy/dir/nested_file2")
+    touch("deploy/dir/nested_dir/nested_file3")
+
+    paths_to_sync = [Path(p) for p in paths_to_sync]
+    result = _get_stage_paths_to_sync(paths_to_sync, Path("deploy/"))
+    assert result.sort() == [StagePath(p) for p in expected_result].sort()
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_package_scripts.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_package_scripts.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_run_processor.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_run_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,20 @@
         [
             (
                 mock_cursor([{"CURRENT_ROLE()": "old_role"}], []),
                 mock.call("select current_role()", cursor_class=DictCursor),
             ),
             (None, mock.call("use role app_role")),
             (None, mock.call("use warehouse app_warehouse")),
+            (
+                None,
+                mock.call(
+                    "alter application myapp upgrade using @app_pkg.app_src.stage"
+                ),
+            ),
             (None, mock.call("alter application myapp set debug_mode = True")),
             (None, mock.call("use role old_role")),
         ]
     )
     mock_conn.return_value = MockConnectionCtx()
     mock_execute.side_effect = side_effects
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_teardown_processor.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_teardown_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_create_processor.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_version_create_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/test_version_drop_processor.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/test_version_drop_processor.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/utils.py` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from textwrap import dedent
 
 NATIVEAPP_MODULE = "snowflake.cli.plugins.nativeapp.manager"
 TEARDOWN_MODULE = "snowflake.cli.plugins.nativeapp.teardown_processor"
 TYPER_CONFIRM = "typer.confirm"
 RUN_MODULE = "snowflake.cli.plugins.nativeapp.run_processor"
 VERSION_MODULE = "snowflake.cli.plugins.nativeapp.version.version_processor"
@@ -74,7 +75,13 @@
     """
 )
 
 
 def mock_execute_helper(mock_input: list):
     side_effects, expected = map(list, zip(*mock_input))
     return side_effects, expected
+
+
+def touch(path: str):
+    file = Path(path)
+    file.parent.mkdir(exist_ok=True, parents=True)
+    file.write_text("")
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/__snapshots__/test_commands.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/nativeapp/__snapshots__/test_init.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/nativeapp/__snapshots__/test_init.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/object/test_common.py` & `snowflake_cli_labs-2.3.0rc0/tests/object/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/object/test_object.py` & `snowflake_cli_labs-2.3.0rc0/tests/object/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/object/test_stage.py` & `snowflake_cli_labs-2.3.0rc0/tests/object/test_stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/object/__snapshots__/test_object.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/object/__snapshots__/test_object.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/output/test_format_silent_enforcement.py` & `snowflake_cli_labs-2.3.0rc0/tests/output/test_format_silent_enforcement.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/output/test_printing.py` & `snowflake_cli_labs-2.3.0rc0/tests/output/test_printing.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/output/test_silent_output.py` & `snowflake_cli_labs-2.3.0rc0/tests/output/test_silent_output.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_broken_plugin.py` & `snowflake_cli_labs-2.3.0rc0/tests/plugin/test_broken_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_failing_plugin.py` & `snowflake_cli_labs-2.3.0rc0/tests/plugin/test_failing_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/plugin/test_override_by_external_plugins.py` & `snowflake_cli_labs-2.3.0rc0/tests/plugin/test_override_by_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/project/fixtures.py` & `snowflake_cli_labs-2.3.0rc0/tests/project/fixtures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/project/test_config.py` & `snowflake_cli_labs-2.3.0rc0/tests/project/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/project/test_definition_manager.py` & `snowflake_cli_labs-2.3.0rc0/tests/project/test_definition_manager.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/project/test_util.py` & `snowflake_cli_labs-2.3.0rc0/tests/project/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/project/__snapshots__/test_config.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/project/__snapshots__/test_config.ambr`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
   dict({
     'definition_version': 1,
     'native_app': dict({
       'application': None,
       'artifacts': list([
         dict({
           'dest': './',
+          'processors': None,
           'src': 'app/*',
         }),
       ]),
       'deploy_root': 'output/deploy/',
       'name': 'integration',
       'package': dict({
         'distribution': 'internal',
@@ -32,14 +33,15 @@
   dict({
     'definition_version': 1,
     'native_app': dict({
       'application': None,
       'artifacts': list([
         dict({
           'dest': './',
+          'processors': None,
           'src': 'app/*',
         }),
       ]),
       'deploy_root': 'output/deploy/',
       'name': 'integration_external',
       'package': dict({
         'distribution': 'external',
@@ -86,14 +88,15 @@
         'warehouse': None,
       }),
       'artifacts': list([
         'setup.sql',
         'app/README.md',
         dict({
           'dest': 'ui/',
+          'processors': None,
           'src': 'app/streamlit/*.py',
         }),
       ]),
       'deploy_root': 'output/deploy/',
       'name': 'myapp',
       'package': dict({
         'distribution': 'internal',
@@ -122,14 +125,15 @@
         'warehouse': None,
       }),
       'artifacts': list([
         'setup.sql',
         'app/README.md',
         dict({
           'dest': 'ui/',
+          'processors': None,
           'src': 'app/streamlit/*.py',
         }),
       ]),
       'deploy_root': 'output/deploy/',
       'name': 'myapp',
       'package': dict({
         'distribution': 'internal',
@@ -206,16 +210,16 @@
           'handler': 'app.hello_function',
           'imports': list([
           ]),
           'name': 'custom_db.custom_schema.fqn_function',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -227,16 +231,16 @@
           'handler': 'app.hello_function',
           'imports': list([
           ]),
           'name': 'custom_schema.fqn_function_only_schema',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -248,16 +252,16 @@
           'handler': 'app.hello_function',
           'imports': list([
           ]),
           'name': 'schema_function',
           'returns': 'string',
           'runtime': None,
           'schema_name': 'custom_schema',
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -269,16 +273,16 @@
           'handler': 'app.hello_function',
           'imports': list([
           ]),
           'name': 'database_function',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -290,16 +294,16 @@
           'handler': 'app.hello_function',
           'imports': list([
           ]),
           'name': 'custom_schema.database_function',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -311,16 +315,16 @@
           'handler': 'app.hello_function',
           'imports': list([
           ]),
           'name': 'custom_database.custom_schema.fqn_function_error',
           'returns': 'string',
           'runtime': None,
           'schema_name': 'custom_schema',
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -392,16 +396,16 @@
           'handler': 'app.func1_handler',
           'imports': list([
           ]),
           'name': 'func1',
           'returns': 'string',
           'runtime': '3.10',
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': 'default value',
               'name': 'a',
             }),
             dict({
@@ -479,16 +483,16 @@
           'handler': 'app.hello_procedure',
           'imports': list([
           ]),
           'name': 'custom_db.custom_schema.fqn_procedure',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -501,16 +505,16 @@
           'handler': 'app.hello_procedure',
           'imports': list([
           ]),
           'name': 'custom_schema.fqn_procedure_only_schema',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -523,16 +527,16 @@
           'handler': 'app.hello_procedure',
           'imports': list([
           ]),
           'name': 'schema_procedure',
           'returns': 'string',
           'runtime': None,
           'schema_name': 'custom_schema',
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -545,16 +549,16 @@
           'handler': 'app.hello_procedure',
           'imports': list([
           ]),
           'name': 'database_procedure',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -567,16 +571,16 @@
           'handler': 'app.hello_procedure',
           'imports': list([
           ]),
           'name': 'custom_schema.database_procedure',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -589,16 +593,16 @@
           'handler': 'app.hello_procedure',
           'imports': list([
           ]),
           'name': 'custom_database.custom_schema.fqn_procedure_error',
           'returns': 'string',
           'runtime': None,
           'schema_name': 'custom_schema',
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -667,16 +671,16 @@
           'handler': 'hello',
           'imports': list([
           ]),
           'name': 'procedureName',
           'returns': 'string',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
@@ -689,16 +693,16 @@
           'handler': 'test',
           'imports': list([
           ]),
           'name': 'test',
           'returns': 'string',
           'runtime': '3.10',
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': '',
         }),
       ]),
       'project_name': 'my_snowpark_project',
       'src': 'app/',
       'stage_name': 'dev_deployment',
     }),
@@ -721,16 +725,16 @@
           'handler': 'foo.func',
           'imports': list([
           ]),
           'name': 'foo',
           'returns': 'variant',
           'runtime': None,
           'schema_name': None,
-          'secrets': list([
-          ]),
+          'secrets': dict({
+          }),
           'signature': list([
             dict({
               'arg_type': 'string',
               'default': None,
               'name': 'name',
             }),
           ]),
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/mocks.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/mocks.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_anaconda.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_anaconda.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_build.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_build.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_common.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_function.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_function.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_models.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_models.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_package.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         assert result.exit_code == 0
         assert result.output == snapshot
 
     @patch(
         "snowflake.cli.plugins.snowpark.package.commands.download_unavailable_packages"
     )
     @patch(
-        "snowflake.cli.plugins.snowpark.package_utils.Venv.pip_wheel",
+        "snowflake.cli.plugins.snowpark.package_utils.pip_wheel",
     )
     @pytest.mark.parametrize(
         "extra_flags", [[], ["--skip-version-check"], ["--ignore-anaconda"]]
     )
     def test_package_create(
         self,
         mock_pip_wheel,
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/test_procedure.py` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/test_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_package.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_package.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/snowpark/__snapshots__/test_procedure.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_common.py` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/test_common.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_image_repository.py` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_jobs.py` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_registry.py` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/test_services.py` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/__snapshots__/test_image_repository.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/spcs/__snapshots__/test_registry.ambr` & `snowflake_cli_labs-2.3.0rc0/tests/spcs/__snapshots__/test_registry.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/stage/test_diff.py` & `snowflake_cli_labs-2.3.0rc0/tests/stage/test_diff.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,141 @@
 import hashlib
+import typing
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Union
 from unittest import mock
 
 import pytest
-from snowflake.cli.api.exceptions import SnowflakeSQLExecutionError
+from snowflake.cli.api.exceptions import (
+    SnowflakeSQLExecutionError,
+)
 from snowflake.cli.plugins.stage.diff import (
     DiffResult,
+    StagePath,
+    build_md5_map,
+    compute_stage_diff,
     delete_only_on_stage_files,
     enumerate_files,
-    get_stage_path_from_file,
+    get_stage_subpath,
+    preserve_from_diff,
     put_files_on_stage,
-    stage_diff,
     sync_local_diff_with_stage,
 )
 from snowflake.cli.plugins.stage.manager import StageManager
 
 from tests.testing_utils.files_and_dirs import temp_local_dir
 
 STAGE_MANAGER = "snowflake.cli.plugins.stage.manager.StageManager"
+STAGE_DIFF = "snowflake.cli.plugins.object.stage.diff"
 
 FILE_CONTENTS = {
     "README.md": "This is a README\n",
     "ui/streamlit.py": "# this is a streamlit\n",
     "my.jar": b"083hgia2r92tha",
 }
 DEFAULT_LAST_MODIFIED = "Tue, 5 Sep 2023 17:59:21 GMT"
 STAGE_LS_COLUMNS = ["name", "size", "md5", "last_modified"]
 
 
+def as_stage_paths(paths: typing.Iterable[str]) -> List[StagePath]:
+    return [StagePath(p) for p in paths]
+
+
 def md5_of(contents: Union[str, bytes]) -> str:
     hash_value = hashlib.md5()
     if isinstance(contents, bytes):
         hash_value.update(contents)
     else:
         hash_value.update(contents.encode("UTF-8"))
     return hash_value.hexdigest()
 
 
 def stage_contents(
     files: Dict[str, Union[str, bytes]], last_modified: str = DEFAULT_LAST_MODIFIED
-) -> List[Tuple[str, int, str, str]]:
+) -> List[Dict[str, Union[str, int]]]:
     """
     Return file contents as they would be listed by a SNOWFLAKE_SSE stage
     if they were uploaded with the given structure and contents.
     """
     return [
-        (f"stage/{relpath}", len(contents), md5_of(contents), last_modified)
+        {
+            "name": f"stage/{relpath}",
+            "size": len(contents),
+            "md5": md5_of(contents),
+            "last_modified": last_modified,
+        }
         for (relpath, contents) in files.items()
     ]
 
 
 @mock.patch(f"{STAGE_MANAGER}.list_files")
 def test_empty_stage(mock_list, mock_cursor):
     mock_list.return_value = mock_cursor(rows=[], columns=STAGE_LS_COLUMNS)
 
     with temp_local_dir(FILE_CONTENTS) as local_path:
-        diff_result = stage_diff(local_path, "a.b.c")
+        diff_result = compute_stage_diff(local_path, "a.b.c")
         assert len(diff_result.only_on_stage) == 0
         assert len(diff_result.different) == 0
         assert len(diff_result.identical) == 0
-        assert sorted(diff_result.only_local) == sorted(FILE_CONTENTS.keys())
+        assert sorted(diff_result.only_local) == sorted(
+            as_stage_paths(FILE_CONTENTS.keys())
+        )
 
 
 @mock.patch(f"{STAGE_MANAGER}.list_files")
 def test_empty_dir(mock_list, mock_cursor):
     mock_list.return_value = mock_cursor(
         rows=stage_contents(FILE_CONTENTS),
         columns=STAGE_LS_COLUMNS,
     )
 
     with temp_local_dir({}) as local_path:
-        diff_result = stage_diff(local_path, "a.b.c")
-        assert sorted(diff_result.only_on_stage) == sorted(FILE_CONTENTS.keys())
+        diff_result = compute_stage_diff(local_path, "a.b.c")
+        assert sorted(diff_result.only_on_stage) == sorted(
+            as_stage_paths(FILE_CONTENTS.keys())
+        )
         assert len(diff_result.different) == 0
         assert len(diff_result.identical) == 0
         assert len(diff_result.only_local) == 0
 
 
 @mock.patch(f"{STAGE_MANAGER}.list_files")
 def test_identical_stage(mock_list, mock_cursor):
     mock_list.return_value = mock_cursor(
         rows=stage_contents(FILE_CONTENTS),
         columns=STAGE_LS_COLUMNS,
     )
 
     with temp_local_dir(FILE_CONTENTS) as local_path:
-        diff_result = stage_diff(local_path, "a.b.c")
+        diff_result = compute_stage_diff(local_path, "a.b.c")
         assert len(diff_result.only_on_stage) == 0
         assert len(diff_result.different) == 0
-        assert sorted(diff_result.identical) == sorted(FILE_CONTENTS.keys())
+        assert sorted(diff_result.identical) == sorted(
+            as_stage_paths(FILE_CONTENTS.keys())
+        )
         assert len(diff_result.only_local) == 0
 
 
 @mock.patch(f"{STAGE_MANAGER}.list_files")
 def test_new_local_file(mock_list, mock_cursor):
     mock_list.return_value = mock_cursor(
         rows=stage_contents(FILE_CONTENTS),
         columns=STAGE_LS_COLUMNS,
     )
 
     with temp_local_dir(
         {**FILE_CONTENTS, "a/new/README.md": "### I am a new markdown readme"}
     ) as local_path:
-        diff_result = stage_diff(local_path, "a.b.c")
+        diff_result = compute_stage_diff(local_path, "a.b.c")
         assert len(diff_result.only_on_stage) == 0
         assert len(diff_result.different) == 0
-        assert sorted(diff_result.identical) == sorted(FILE_CONTENTS.keys())
-        assert diff_result.only_local == ["a/new/README.md"]
+        assert sorted(diff_result.identical) == sorted(
+            as_stage_paths(FILE_CONTENTS.keys())
+        )
+        assert diff_result.only_local == as_stage_paths(["a/new/README.md"])
 
 
 @mock.patch(f"{STAGE_MANAGER}.list_files")
 def test_modified_file(mock_list, mock_cursor):
     mock_list.return_value = mock_cursor(
         rows=stage_contents(FILE_CONTENTS),
         columns=STAGE_LS_COLUMNS,
@@ -119,18 +143,20 @@
 
     with temp_local_dir(
         {
             **FILE_CONTENTS,
             "README.md": "This is a modification to the existing README",
         }
     ) as local_path:
-        diff_result = stage_diff(local_path, "a.b.c")
+        diff_result = compute_stage_diff(local_path, "a.b.c")
         assert len(diff_result.only_on_stage) == 0
-        assert sorted(diff_result.different) == ["README.md"]
-        assert sorted(diff_result.identical) == ["my.jar", "ui/streamlit.py"]
+        assert sorted(diff_result.different) == as_stage_paths(["README.md"])
+        assert sorted(diff_result.identical) == as_stage_paths(
+            ["my.jar", "ui/streamlit.py"]
+        )
         assert len(diff_result.only_local) == 0
 
 
 def test_get_stage_path_from_file():
     expected = [
         "",
         "ui/streamlit.py",
@@ -145,24 +171,26 @@
             "ui/nested/environment.yml": "# this is a environment file\n",
             "module-add/src/python/app.py": "# this is an app file\n",
         }
     ) as local_path:
         local_files = enumerate_files(local_path)
         for local_file in local_files:
             relpath = str(local_file.relative_to(local_path))
-            actual.append(get_stage_path_from_file(relpath))
+            actual.append(get_stage_subpath(StagePath(relpath)))
     assert actual.sort() == expected
 
 
 @mock.patch(f"{STAGE_MANAGER}.remove")
 def test_delete_only_on_stage_files(mock_remove):
     stage_name = "some_stage_name"
     random_file = "some_file_on_stage"
 
-    delete_only_on_stage_files(StageManager(), stage_name, [random_file], "some_role")
+    delete_only_on_stage_files(
+        StageManager(), stage_name, as_stage_paths([random_file]), "some_role"
+    )
     mock_remove.assert_has_calls(
         [mock.call(stage_name=stage_name, path=random_file, role="some_role")]
     )
 
 
 @mock.patch(f"{STAGE_MANAGER}.put")
 @pytest.mark.parametrize("overwrite_param", [True, False])
@@ -174,15 +202,15 @@
             "README.md": "# this is an app file\n",
         }
     ) as local_path:
         put_files_on_stage(
             stage_manager=StageManager(),
             stage_fqn=stage_name,
             deploy_root_path=local_path,
-            files=["ui/nested/environment.yml", "README.md"],
+            stage_paths=as_stage_paths(["ui/nested/environment.yml", "README.md"]),
             role="some_role",
             overwrite=overwrite_param,
         )
         expected = [
             mock.call(
                 local_path=local_path / "ui/nested/environment.yml",
                 stage_path=f"{stage_name}/ui/nested",  # TODO: verify if trailing slash is needed, doesn't seem so from regression tests
@@ -195,23 +223,80 @@
                 role="some_role",
                 overwrite=overwrite_param,
             ),
         ]
         assert mock_put.mock_calls == expected
 
 
+def test_build_md5_map(mock_cursor):
+    actual = build_md5_map(
+        mock_cursor(
+            rows=stage_contents(FILE_CONTENTS),
+            columns=STAGE_LS_COLUMNS,
+        )
+    )
+
+    expected = {
+        StagePath("README.md"): "9b650974f65cc49be96a5ed34ac6d1fd",
+        StagePath("my.jar"): "fc605d0e2e50cf3e71873d57f4c598b0",
+        StagePath("ui/streamlit.py"): "a7dfdfaf892ecfc5f164914123c7f2cc",
+    }
+
+    assert actual == expected
+
+
 @mock.patch(f"{STAGE_MANAGER}.remove")
 def test_sync_local_diff_with_stage(mock_remove, other_directory):
     temp_dir = Path(other_directory)
     mock_remove.side_effect = Exception("Mock Exception")
     mock_remove.return_value = None
-    diff: DiffResult = DiffResult()
+    diff = DiffResult()
     diff.only_on_stage = ["some_file_on_stage"]
     stage_name = "some_stage_name"
 
     with pytest.raises(SnowflakeSQLExecutionError):
         sync_local_diff_with_stage(
             role="some_role",
             deploy_root_path=temp_dir,
             diff_result=diff,
-            stage_path=stage_name,
+            stage_fqn=stage_name,
         )
+
+
+def test_filter_from_diff():
+    diff = DiffResult()
+    diff.different = [
+        "different",
+        "different-2",
+        "dir/different",
+        "dir/different-2",
+    ]
+    diff.only_local = [
+        "only_local",
+        "only_local-2",
+        "dir/only_local",
+        "dir/only_local-2",
+    ]
+    diff.only_on_stage = [
+        "only_on_stage",
+        "only_on_stage-2",
+        "dir/only_on_stage",
+        "dir/only_on_stage-2",
+    ]
+
+    paths_to_sync = [
+        "different",
+        "only-local",
+        "only-stage",
+        "dir/different",
+        "dir/only-local",
+        "dir/only-stage",
+    ]
+    new_diff = preserve_from_diff(diff, as_stage_paths(paths_to_sync))
+
+    for path in new_diff.different:
+        assert path in paths_to_sync
+    for path in new_diff.only_local:
+        assert path in paths_to_sync
+    for path in new_diff.only_on_stage:
+        assert path in paths_to_sync
+    assert new_diff.identical == diff.identical
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/stage/test_stage.py` & `snowflake_cli_labs-2.3.0rc0/tests/stage/test_stage.py`

 * *Files 3% similar despite different names*

```diff
@@ -659,57 +659,86 @@
             ),
             mock.call("use role old_role"),
         ]
         assert mock_execute.mock_calls == expected
 
 
 @pytest.mark.parametrize(
-    "stage_path, expected_files",
+    "stage_path, expected_stage, expected_files",
     [
-        ("@exe", ["exe/s1.sql", "exe/a/s3.sql", "exe/a/b/s4.sql"]),
+        ("@exe", "@exe", ["@exe/s1.sql", "@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
         (
             "snow://exe",
-            ["exe/s1.sql", "exe/a/s3.sql", "exe/a/b/s4.sql"],
+            "@exe",
+            ["@exe/s1.sql", "@exe/a/s3.sql", "@exe/a/b/s4.sql"],
+        ),
+        ("exe", "@exe", ["@exe/s1.sql", "@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/", "@exe", ["@exe/s1.sql", "@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/*", "@exe", ["@exe/s1.sql", "@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/*.sql", "@exe", ["@exe/s1.sql", "@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/a", "@exe", ["@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/a/", "@exe", ["@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/a/*", "@exe", ["@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/a/*.sql", "@exe", ["@exe/a/s3.sql", "@exe/a/b/s4.sql"]),
+        ("exe/a/b", "@exe", ["@exe/a/b/s4.sql"]),
+        ("exe/a/b/", "@exe", ["@exe/a/b/s4.sql"]),
+        ("exe/a/b/*", "@exe", ["@exe/a/b/s4.sql"]),
+        ("exe/a/b/*.sql", "@exe", ["@exe/a/b/s4.sql"]),
+        ("exe/s?.sql", "@exe", ["@exe/s1.sql"]),
+        ("exe/s1.sql", "@exe", ["@exe/s1.sql"]),
+        (
+            "@db.schema.exe",
+            "@db.schema.exe",
+            [
+                "@db.schema.exe/s1.sql",
+                "@db.schema.exe/a/s3.sql",
+                "@db.schema.exe/a/b/s4.sql",
+            ],
+        ),
+        (
+            "db.schema.exe",
+            "@db.schema.exe",
+            [
+                "@db.schema.exe/s1.sql",
+                "@db.schema.exe/a/s3.sql",
+                "@db.schema.exe/a/b/s4.sql",
+            ],
         ),
-        ("exe", ["exe/s1.sql", "exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/", ["exe/s1.sql", "exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/*", ["exe/s1.sql", "exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/*.sql", ["exe/s1.sql", "exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/a", ["exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/a/", ["exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/a/*", ["exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/a/*.sql", ["exe/a/s3.sql", "exe/a/b/s4.sql"]),
-        ("exe/a/b", ["exe/a/b/s4.sql"]),
-        ("exe/a/b/", ["exe/a/b/s4.sql"]),
-        ("exe/a/b/*", ["exe/a/b/s4.sql"]),
-        ("exe/a/b/*.sql", ["exe/a/b/s4.sql"]),
-        ("exe/s?.sql", ["exe/s1.sql"]),
-        ("exe/s1.sql", ["exe/s1.sql"]),
+        ("@db.schema.exe/s1.sql", "@db.schema.exe", ["@db.schema.exe/s1.sql"]),
     ],
 )
 @mock.patch(f"{STAGE_MANAGER}._execute_query")
-def test_execute(mock_execute, mock_cursor, runner, stage_path, expected_files):
+def test_execute(
+    mock_execute,
+    mock_cursor,
+    runner,
+    stage_path,
+    expected_stage,
+    expected_files,
+    snapshot,
+):
     mock_execute.return_value = mock_cursor(
         [
             {"name": "exe/a/s3.sql"},
             {"name": "exe/a/b/s4.sql"},
             {"name": "exe/s1.sql"},
             {"name": "exe/s2"},
         ],
         [],
     )
 
     result = runner.invoke(["stage", "execute", stage_path])
 
     assert result.exit_code == 0, result.output
     ls_call, *execute_calls = mock_execute.mock_calls
-    assert ls_call == mock.call(f"ls @exe", cursor_class=DictCursor)
+    assert ls_call == mock.call(f"ls {expected_stage}", cursor_class=DictCursor)
     assert execute_calls == [
-        mock.call(f"execute immediate from @{p}") for p in expected_files
+        mock.call(f"execute immediate from {p}") for p in expected_files
     ]
+    assert result.output == snapshot
 
 
 @mock.patch(f"{STAGE_MANAGER}._execute_query")
 def test_execute_with_variables(mock_execute, mock_cursor, runner):
     mock_execute.return_value = mock_cursor([{"name": "exe/s1.sql"}], [])
 
     result = runner.invoke(
@@ -799,29 +828,29 @@
         ("exe/*.txt", "No files matched pattern 'exe/*.txt'"),
         ("exe/directory", "No files matched pattern 'exe/directory'"),
         ("exe/some_file.sql", "No files matched pattern 'exe/some_file.sql'"),
     ],
 )
 @mock.patch(f"{STAGE_MANAGER}._execute_query")
 def test_execute_no_files_for_stage_path(
-    mock_execute, mock_cursor, runner, snapshot, stage_path, expected_message
+    mock_execute, mock_cursor, runner, stage_path, expected_message
 ):
     mock_execute.return_value = mock_cursor(
         [
             {"name": "exe/a/s3.sql"},
             {"name": "exe/a/b/s4.sql"},
             {"name": "exe/s1.sql"},
         ],
         [],
     )
 
     result = runner.invoke(["stage", "execute", stage_path, "--on-error", "continue"])
 
     assert result.exit_code == 1
-    assert result.output == snapshot
+    assert expected_message in result.output
 
 
 @mock.patch(f"{STAGE_MANAGER}._execute_query")
 def test_execute_stop_on_error(mock_execute, mock_cursor, runner):
     error_message = "Error"
     mock_execute.side_effect = [
         mock_cursor(
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_commands.py` & `snowflake_cli_labs-2.3.0rc0/tests/streamlit/test_commands.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/streamlit/test_config.py` & `snowflake_cli_labs-2.3.0rc0/tests/streamlit/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/anaconda_channel_data.json` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/anaconda_channel_data.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/packages_available_in_snowflake_sql_result_rows.json`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/test_data.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/Zendesk-1.1.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_core-1.29.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/azure_eventhub-5.11.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/local_packages/.packages/httplib2-0.22.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration/app/manifest.yml` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/integration_external/app/manifest.yml` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/integration_external/app/manifest.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_function_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_functions/app.zip` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_functions/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedure_secrets_without_external_access/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures/app.zip` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures/app.zip`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py` & `snowflake_cli_labs-2.3.0rc0/tests/test_data/projects/snowpark_procedures_coverage/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/testing_utils/files_and_dirs.py` & `snowflake_cli_labs-2.3.0rc0/tests/testing_utils/files_and_dirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,7 +42,20 @@
             path.parent.mkdir(parents=True, exist_ok=True)
             mode = "wb" if isinstance(contents, bytes) else "w"
             encoding = None if isinstance(contents, bytes) else "UTF-8"
             with open(path, mode=mode, encoding=encoding) as fh:
                 fh.write(contents)
 
         yield Path(tmpdir)
+
+
+def merge_left(target: Dict, source: Dict) -> None:
+    """
+    Recursively merges key/value pairs from source into target.
+    Modifies the original dict-like "target".
+    """
+    for k, v in source.items():
+        if k in target and isinstance(target[k], dict):
+            # assumption: all inputs have been validated.
+            merge_left(target[k], v)
+        else:
+            target[k] = v
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests/testing_utils/fixtures.py` & `snowflake_cli_labs-2.3.0rc0/tests/testing_utils/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,29 @@
 from io import StringIO
 from pathlib import Path
 from typing import Generator, List, NamedTuple, Optional, Union
 from unittest import mock
 
 import pytest
 import yaml
-from snowflake.cli.api.project.definition import merge_left
+from snowflake.cli.api.project.schemas.project_definition import ProjectDefinition
+from snowflake.cli.api.project.schemas.snowpark.argument import Argument
+from snowflake.cli.api.project.schemas.snowpark.callable import FunctionSchema
 from snowflake.cli.app.cli_app import app_factory
 from snowflake.connector.cursor import SnowflakeCursor
 from snowflake.connector.errors import ProgrammingError
 from typer import Typer
 from typer.testing import CliRunner
 
 from tests.test_data import test_data
-from tests.testing_utils.files_and_dirs import create_named_file, create_temp_file
+from tests.testing_utils.files_and_dirs import (
+    create_named_file,
+    create_temp_file,
+    merge_left,
+)
 
 REQUIREMENTS_SNOWFLAKE = "requirements.snowflake.txt"
 REQUIREMENTS_TXT = "requirements.txt"
 TEST_DIR = Path(__file__).parent.parent
 
 
 class SnowCLIRunner(CliRunner):
@@ -259,15 +265,14 @@
     """
     Set up the default location of config files to [temp_dir]/.snowflake
     """
     with tempfile.TemporaryDirectory() as tmp_dir:
         snowflake_home = Path(tmp_dir) / ".snowflake"
         snowflake_home.mkdir()
         monkeypatch.setenv("SNOWFLAKE_HOME", str(snowflake_home))
-
         for module in [
             sys.modules["snowflake.connector.constants"],
             sys.modules["snowflake.connector.config_manager"],
             sys.modules["snowflake.cli.api.config"],
         ]:
             importlib.reload(module)
 
@@ -296,7 +301,40 @@
             else:
                 current_object[evaluated_part] = value
 
         with open(snowflake_yml_path, "w+") as fh:
             yaml.safe_dump(yml, fh)
 
     return _update
+
+
+@pytest.fixture()
+def argument_instance():
+    return Argument(name="Foo", type="Bar")
+
+
+@pytest.fixture()
+def function_instance():
+    return FunctionSchema(
+        name="func1",
+        handler="app.func1_handler",
+        signature=[{"name": "a", "type": "string"}, {"name": "b", "type": "variant"}],
+        returns="string",
+    )
+
+
+@pytest.fixture()
+def native_app_project_instance():
+    return ProjectDefinition(
+        **{
+            "definition_version": "1",
+            "native_app": {
+                "artifacts": [{"dest": "./", "src": "app/*"}],
+                "name": "napp_test",
+                "package": {
+                    "scripts": [
+                        "package/001.sql",
+                    ]
+                },
+            },
+        }
+    )
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_e2e/conftest.py` & `snowflake_cli_labs-2.3.0rc0/tests_e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_installation.py` & `snowflake_cli_labs-2.3.0rc0/tests_e2e/test_installation.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_e2e/test_snowpark_examples.py` & `snowflake_cli_labs-2.3.0rc0/tests_e2e/test_snowpark_examples.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_e2e/__snapshots__/test_installation.ambr` & `snowflake_cli_labs-2.3.0rc0/tests_e2e/__snapshots__/test_installation.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/conftest.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import pytest
 import yaml
 
 from snowflake.cli.api.cli_global_context import cli_context_manager
-from snowflake.cli.api.project.definition import merge_left
 from snowflake.cli.app.cli_app import app_factory
 from typer import Typer
 from typer.testing import CliRunner
 
 from tests.conftest import clean_logging_handlers_fixture  # noqa: F401
 from tests.testing_utils.fixtures import (
     alter_snowflake_yml,  # noqa: F401
     snowflake_home,
 )
+from tests.testing_utils.files_and_dirs import merge_left
 
 pytest_plugins = [
     "tests_integration.testing_utils",
     "tests_integration.snowflake_connector",
 ]
 
 TEST_DIR = Path(__file__).parent
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/snowflake_connector.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_config.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_connection.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,8 +39,11 @@
 def test_connection_not_existing_schema(
     runner, test_database, snowflake_session, snowflake_home
 ):
     schema = "schema_which_does_not_exist"
     with mock_single_env_var(SCHEMA_ENV_PARAMETER, value=schema):
         result = runner.invoke_with_connection(["connection", "test"])
         assert result.exit_code == 1, result.output
-        assert "Object does not exist" in result.output
+        assert (
+            f'Could not use schema "{schema.upper()}". Object does not exist'
+            in result.output
+        )
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_external_plugins.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_external_plugins.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_git.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_git.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,15 +228,15 @@
             assert (
                 err.raw_msg
                 == "The specified tag 'no-such-tag' cannot be found in the Git Repository."
             )
 
 
 @pytest.mark.integration
-def test_execute(runner, sf_git_repository, snapshot):
+def test_execute(runner, test_database, sf_git_repository, snapshot):
     result = runner.invoke_with_connection_json(
         [
             "git",
             "execute",
             f"@{sf_git_repository}/branches/main/tests_integration/test_data/projects/stage_execute/script_template.sql",
             "-D",
             "text='string'",
@@ -249,14 +249,42 @@
         ]
     )
 
     assert result.exit_code == 0
     assert result.json == snapshot
 
 
+@pytest.mark.integration
+def test_execute_fqn_repo(runner, test_database, sf_git_repository):
+    result_fqn = runner.invoke_with_connection_json(
+        [
+            "git",
+            "execute",
+            f"@{test_database}.public.{sf_git_repository}/branches/main/tests_integration/test_data/projects/stage_execute/script_template.sql",
+            "-D",
+            "text='string'",
+            "-D",
+            "value=1",
+            "-D",
+            "boolean=TRUE",
+            "-D",
+            "null_value=NULL",
+        ]
+    )
+
+    assert result_fqn.exit_code == 0
+    assert result_fqn.json == [
+        {
+            "File": f"@{test_database}.public.{sf_git_repository}/branches/main/tests_integration/test_data/projects/stage_execute/script_template.sql",
+            "Status": "SUCCESS",
+            "Error": None,
+        }
+    ]
+
+
 def _filter_key(objects, *, key):
     return [o[key] for o in objects]
 
 
 def _assert_invalid_repo_path_error_message(output):
     assert "Error" in output
     assert (
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_nativeapp.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_nativeapp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import uuid
 
 from snowflake.cli.api.project.util import generate_user_env
 from snowflake.cli.api.secure_path import SecurePath
 from snowflake.cli.plugins.nativeapp.init import OFFICIAL_TEMPLATES_GITHUB_URL
+from tests.nativeapp.utils import touch
+from click import ClickException
 
 from tests.project.fixtures import *
 from tests_integration.test_utils import (
     contains_row_with,
     not_contains_row_with,
     row_from_snowflake_session,
 )
@@ -314,14 +316,67 @@
             result = runner.invoke_with_connection_json(
                 ["app", "teardown", "--force"],
                 env=TEST_ENV,
             )
             assert result.exit_code == 0
 
 
+# Verifies that running "app run" after "app deploy" upgrades the app
+@pytest.mark.integration
+def test_nativeapp_run_after_deploy(
+    runner,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    app_name = f"{project_name}_{USER_NAME}"
+    stage_fqn = f"{project_name}_pkg_{USER_NAME}.app_src.stage"
+
+    result = runner.invoke_json(
+        ["app", "init", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_name)):
+        try:
+            # Run #1
+            result = runner.invoke_with_connection_json(
+                ["app", "run"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+            # Make a change & deploy
+            with open("app/README.md", "a") as file:
+                file.write("### Test")
+            result = runner.invoke_with_connection_json(
+                ["app", "deploy"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+            # Run #2
+            result = runner.invoke_with_connection_json(
+                ["app", "run", "--debug"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+            assert (
+                f"alter application {app_name} upgrade using @{stage_fqn}"
+                in result.output
+            )
+
+        finally:
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+
 # Tests a simple flow of an existing project, executing snow app version create, drop and teardown, all with distribution=internal
 @pytest.mark.integration
 @pytest.mark.parametrize("project_definition_files", ["integration"], indirect=True)
 def test_nativeapp_version_create_and_drop(
     runner,
     snowflake_session,
     project_definition_files: List[Path],
@@ -496,15 +551,15 @@
             assert result.exit_code == 0
         finally:
             single_template_repo.close()
 
 
 # Tests a simple flow of executing "snow app deploy", verifying that an application package was created, and an application was not
 @pytest.mark.integration
-def test_nativeapp_init_deploy(
+def test_nativeapp_deploy(
     runner,
     snowflake_session,
     temporary_working_directory,
 ):
     project_name = "myapp"
     result = runner.invoke_json(
         ["app", "init", project_name],
@@ -546,21 +601,283 @@
                     snowflake_session.execute_string(
                         f"show applications like '{app_name}'",
                     )
                 ),
                 dict(name=app_name),
             )
 
+            # re-deploying should be a no-op; make sure we don't issue any PUT commands
+            result = runner.invoke_with_connection_json(
+                ["app", "deploy", "--debug"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+            assert "Successfully uploaded chunk 0 of file" not in result.output
+
+            # make sure we always delete the package
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+        finally:
+            # teardown is idempotent, so we can execute it again with no ill effects
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+
+@pytest.mark.integration
+@pytest.mark.parametrize(
+    "command,contains,not_contains",
+    [
+        # deploy --prune removes remote-only files
+        ["app deploy --prune", ["stage/manifest.yml"], ["stage/README.md"]],
+        # deploy removes remote-only files (--prune is the default value)
+        ["app deploy", ["stage/manifest.yml"], ["stage/README.md"]],
+        # deploy --no-prune does not delete remote-only files
+        ["app deploy --no-prune", ["stage/README.md"], []],
+    ],
+)
+def test_nativeapp_deploy_prune(
+    command,
+    contains,
+    not_contains,
+    runner,
+    snowflake_session,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    result = runner.invoke_json(
+        ["app", "init", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_name)):
+        result = runner.invoke_with_connection_json(
+            ["app", "deploy"],
+            env=TEST_ENV,
+        )
+        assert result.exit_code == 0
+
+        try:
+            # delete a file locally
+            os.remove(os.path.join("app", "README.md"))
+
+            # deploy
+            result = runner.invoke_with_connection_json(
+                command.split(),
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+            # verify the file does not exist on the stage
+            package_name = f"{project_name}_pkg_{USER_NAME}".upper()
+            stage_name = "app_src.stage"  # as defined in native-apps-templates/basic
+            stage_files = runner.invoke_with_connection_json(
+                ["stage", "list-files", f"{package_name}.{stage_name}"],
+                env=TEST_ENV,
+            )
+            for name in contains:
+                assert contains_row_with(stage_files.json, {"name": name})
+            for name in not_contains:
+                assert not_contains_row_with(stage_files.json, {"name": name})
+
+            # make sure we always delete the app
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+        finally:
+            # teardown is idempotent, so we can execute it again with no ill effects
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+
+# Tests a simple flow of executing "snow app deploy [files]", verifying that only the specified files are synced to the stage
+@pytest.mark.integration
+def test_nativeapp_deploy_files(
+    runner,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    result = runner.invoke_json(
+        ["app", "init", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_name)):
+        # sync only two specific files to stage
+        result = runner.invoke_with_connection_json(
+            ["app", "deploy", "app/manifest.yml", "app/setup_script.sql"],
+            env=TEST_ENV,
+        )
+        assert result.exit_code == 0
+
+        try:
+            # manifest and script files exist, readme doesn't exist
+            package_name = f"{project_name}_pkg_{USER_NAME}".upper()
+            stage_name = "app_src.stage"  # as defined in native-apps-templates/basic
+            stage_files = runner.invoke_with_connection_json(
+                ["stage", "list-files", f"{package_name}.{stage_name}"],
+                env=TEST_ENV,
+            )
+            assert contains_row_with(stage_files.json, {"name": "stage/manifest.yml"})
+            assert contains_row_with(
+                stage_files.json, {"name": "stage/setup_script.sql"}
+            )
+            assert not_contains_row_with(stage_files.json, {"name": "stage/README.md"})
+
+            # make sure we always delete the app
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+        finally:
+            # teardown is idempotent, so we can execute it again with no ill effects
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+
+# Tests that files inside of a symlinked directory are deployed
+@pytest.mark.integration
+def test_nativeapp_deploy_nested_directories(
+    runner,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    project_dir = "app root"
+    result = runner.invoke_json(
+        ["app", "init", project_dir, "--name", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_dir)):
+        # create nested file under app/
+        touch("app/nested/dir/file.txt")
+
+        result = runner.invoke_with_connection_json(
+            ["app", "deploy", "app/nested/dir/file.txt"],
+            env=TEST_ENV,
+        )
+        assert result.exit_code == 0
+
+        try:
+            package_name = f"{project_name}_pkg_{USER_NAME}".upper()
+            stage_name = "app_src.stage"  # as defined in native-apps-templates/basic
+            stage_files = runner.invoke_with_connection_json(
+                ["stage", "list-files", f"{package_name}.{stage_name}"],
+                env=TEST_ENV,
+            )
+            assert contains_row_with(
+                stage_files.json, {"name": "stage/nested/dir/file.txt"}
+            )
+
+            # make sure we always delete the app
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+        finally:
+            # teardown is idempotent, so we can execute it again with no ill effects
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 0
+
+
+# Tests that deploying a directory recursively syncs all of its contents
+@pytest.mark.integration
+def test_nativeapp_deploy_directory(
+    runner,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    project_dir = "app root"
+    result = runner.invoke_json(
+        ["app", "init", project_dir, "--name", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_dir)):
+        touch("app/dir/file.txt")
+        result = runner.invoke_with_connection_json(
+            ["app", "deploy", "app/dir", "-r"],
+            env=TEST_ENV,
+        )
+        assert result.exit_code == 0
+
+        try:
+            package_name = f"{project_name}_pkg_{USER_NAME}".upper()
+            stage_name = "app_src.stage"  # as defined in native-apps-templates/basic
+            stage_files = runner.invoke_with_connection_json(
+                ["stage", "list-files", f"{package_name}.{stage_name}"],
+                env=TEST_ENV,
+            )
+            assert contains_row_with(stage_files.json, {"name": "stage/dir/file.txt"})
+
             # make sure we always delete the app
             result = runner.invoke_with_connection_json(
                 ["app", "teardown"],
                 env=TEST_ENV,
             )
             assert result.exit_code == 0
 
         finally:
             # teardown is idempotent, so we can execute it again with no ill effects
             result = runner.invoke_with_connection_json(
                 ["app", "teardown", "--force"],
                 env=TEST_ENV,
             )
+            assert result.exit_code == 0
+
+
+# Tests that deploying a directory without specifying -r returns an error
+@pytest.mark.integration
+def test_nativeapp_deploy_directory_no_recursive(
+    runner,
+    temporary_working_directory,
+):
+    project_name = "myapp"
+    project_dir = "app root"
+    result = runner.invoke_json(
+        ["app", "init", project_dir, "--name", project_name],
+        env=TEST_ENV,
+    )
+    assert result.exit_code == 0
+
+    with pushd(Path(os.getcwd(), project_dir)):
+        try:
+            touch("app/nested/dir/file.txt")
+            result = runner.invoke_with_connection_json(
+                ["app", "deploy", "app/nested"],
+                env=TEST_ENV,
+            )
+            assert result.exit_code == 1, result.output
+
+        finally:
+            # teardown is idempotent, so we can execute it again with no ill effects
+            result = runner.invoke_with_connection_json(
+                ["app", "teardown", "--force"],
+                env=TEST_ENV,
+            )
             assert result.exit_code == 0
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_object.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_object.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_package.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_package.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
-import sys
 import tempfile
 from pathlib import Path
 from typing import List
 from zipfile import ZipFile
 
 import pytest
 
 from tests_integration.test_utils import contains_row_with, row_from_snowflake_session
-from tests_integration.testing_utils.assertions.test_result_assertions import (
-    assert_that_result_is_successful,
-)
 
 
 class TestPackage:
     STAGE_NAME = "PACKAGE_TEST"
 
     @pytest.mark.integration
     def test_package_upload(self, runner, snowflake_session, test_database):
@@ -157,18 +153,15 @@
                 "--skip-version-check",
             ]
         )
         assert result.exit_code == 0, result.output
         assert Path("july.zip").exists()
         files = self._get_filenames_from_zip("july.zip")
         # july is not available on anaconda
-        # packaging dependency defines extras
-        assert all(
-            [name.startswith("july") or name.startswith("packaging") for name in files]
-        )
+        assert all([name.startswith("july") for name in files])
 
     @pytest.mark.integration
     def test_package_from_github(self, directory_for_test, runner):
         result = runner.invoke_with_connection_json(
             [
                 "snowpark",
                 "package",
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_session_token.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_session_token.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_snowpark.py`

 * *Files 5% similar despite different names*

```diff
@@ -713,14 +713,28 @@
             in result.output
         )
         assert "--allow-shared-libraries." in result.output
         assert "Build done." not in result.output
 
 
 @pytest.mark.integration
+def test_dependency_search_optimization(
+    runner, project_directory, alter_requirements_txt
+):
+    with project_directory("snowpark") as tmp_dir:
+        alter_requirements_txt(tmp_dir / "requirements.txt", ["july"])
+        result = runner.invoke_with_connection(["snowpark", "build"])
+        assert result.exit_code == 0, result.output
+        snowflake_deps_txt = tmp_dir / "requirements.snowflake.txt"
+        assert snowflake_deps_txt.exists()
+        deps = set(snowflake_deps_txt.read_text().splitlines())
+        assert deps == {"matplotlib", "numpy", "snowflake-snowpark-python"}
+
+
+@pytest.mark.integration
 def test_build_package_from_github(
     runner, project_directory, alter_requirements_txt, test_database
 ):
     with project_directory("snowpark") as tmp_dir:
         alter_requirements_txt(
             tmp_dir / "requirements.txt",
             [
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_snowpark_external_access.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_snowpark_external_access.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_sql.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_stage.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,7 +181,31 @@
             "boolean=TRUE",
             "-D",
             "null_value= NULL",
         ]
     )
     assert result.exit_code == 0
     assert result.json == snapshot
+
+    result_fqn = runner.invoke_with_connection_json(
+        [
+            "stage",
+            "execute",
+            f"@{test_database}.public.{stage_name}/script_template.sql",
+            "-D",
+            " text = 'string' ",
+            "-D",
+            "value=1",
+            "-D",
+            "boolean=TRUE",
+            "-D",
+            "null_value= NULL",
+        ]
+    )
+    assert result_fqn.exit_code == 0
+    assert result_fqn.json == [
+        {
+            "File": f"@{test_database}.public.{stage_name}/script_template.sql",
+            "Status": "SUCCESS",
+            "Error": None,
+        }
+    ]
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_streamlit.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_temporary_connection.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_temporary_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_function.ambr` & `snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_function.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/__snapshots__/test_stage.ambr` & `snowflake_cli_labs-2.3.0rc0/tests_integration/__snapshots__/test_stage.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # serializer version: 1
 # name: test_stage_execute
   list([
     dict({
       'Error': None,
-      'File': 'test_stage_execute/script1.sql',
+      'File': '@test_stage_execute/script1.sql',
       'Status': 'SUCCESS',
     }),
     dict({
       'Error': None,
-      'File': 'test_stage_execute/directory/script2.sql',
+      'File': '@test_stage_execute/directory/script2.sql',
       'Status': 'SUCCESS',
     }),
     dict({
       'Error': None,
-      'File': 'test_stage_execute/directory/subdirectory/script3.sql',
+      'File': '@test_stage_execute/directory/subdirectory/script3.sql',
       'Status': 'SUCCESS',
     }),
   ])
 # ---
 # name: test_stage_execute.1
   list([
     dict({
       'Error': None,
-      'File': 'test_stage_execute/script_template.sql',
+      'File': '@test_stage_execute/script_template.sql',
       'Status': 'SUCCESS',
     }),
   ])
 # ---
```

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/scripts/integration_account_setup.sql` & `snowflake_cli_labs-2.3.0rc0/tests_integration/scripts/integration_account_setup.sql`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_compute_pool.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_compute_pool.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_image_repository.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_image_repository.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_jobs.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_jobs.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_registry.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_registry.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/test_services.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/test_services.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/docker/echo_service.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/docker/echo_service.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/testing_utils/compute_pool_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/testing_utils/spcs_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/spcs/testing_utils/spcs_services_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark/app/app.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_coverage/app/module/procedures.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_external_access/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_external_access/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_fully_qualified_name/app/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml` & `snowflake_cli_labs-2.3.0rc0/tests_integration/test_data/projects/snowpark_with_default_values/snowflake.yml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/naming_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/naming_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/snowpark_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/snowpark_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/sql_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/working_directory_utils.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/working_directory_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py` & `snowflake_cli_labs-2.3.0rc0/tests_integration/testing_utils/assertions/test_result_assertions.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/LICENSE` & `snowflake_cli_labs-2.3.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-2.2.0rc0/README.md` & `snowflake_cli_labs-2.3.0rc0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+[![Code quality checks](https://github.com/snowflakedb/snowflake-cli/actions/workflows/lint.yaml/badge.svg)](https://github.com/snowflakedb/snowflake-cli/actions/workflows/lint.yaml)
+[![Integration testing](https://github.com/snowflakedb/snowflake-cli/actions/workflows/integration_test.yaml/badge.svg)](https://github.com/snowflakedb/snowflake-cli/actions/workflows/integration_test.yaml)
+[![CLI Action testing](https://github.com/snowflakedb/snowflake-cli/actions/workflows/test_cli_action.yaml/badge.svg?branch=main)](https://github.com/snowflakedb/snowflake-cli/actions/workflows/test_cli_action.yaml)
+
+[//]: # ([![Python 3.11]&#40;https://img.shields.io/badge/python-3.11-blue.svg&#41;]&#40;https://www.python.org/downloads/release/python-311/&#41;)
+
 # Snowflake CLI
 
 Snowflake CLI is an open-source command-line tool explicitly designed for developer-centric workloads in addition to SQL operations. It is a flexible and extensible tool that can accommodate modern development practices and technologies.
 
 With Snowflake CLI, developers can create, manage, update, and view apps running on Snowflake across workloads such as Streamlit in Snowflake, the Snowflake Native App Framework, Snowpark Container Services, and Snowpark. It supports a range of Snowflake features, including user-defined functions, stored procedures, Streamlit in Snowflake, and SQL execution.
```

### Comparing `snowflake_cli_labs-2.2.0rc0/pyproject.toml` & `snowflake_cli_labs-2.3.0rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 authors = [{ name = "Snowflake Inc." }]
 license = { file = "LICENSE" }
 dynamic = ["version"]
 requires-python = ">=3.8"
 description = "Snowflake CLI"
 readme = "README.md"
 dependencies = [
-  "jinja2==3.1.3",
-  "pluggy==1.4.0",
+  "jinja2==3.1.4",
+  "pluggy==1.5.0",
   "PyYAML==6.0.1",
   "rich==13.7.1",
   "requests==2.31.0",
   "requirements-parser==0.9.0",
   "setuptools==69.5.1",
-  "snowflake-connector-python[secure-local-storage]==3.8.1",
+  "snowflake-connector-python[secure-local-storage]==3.10.0",
   "tomlkit==0.12.3",
   "typer==0.12.3",
   "urllib3>=1.21.1,<2.3",
   "GitPython==3.1.43",
   "pip",
-  "pydantic==2.7.0"
+  "pydantic==2.7.1",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: System Administrators",
@@ -36,17 +36,17 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: SQL",
   "Topic :: Database",
 ]
 
 [project.optional-dependencies]
 development = [
-  "coverage==7.4.4",
+  "coverage==7.5.0",
   "pre-commit>=3.5.0",
-  "pytest==8.1.1",
+  "pytest==8.2.0",
   "pytest-randomly==3.15.0",
   "syrupy==4.6.1",
 ]
 
 [project.urls]
 "Source code" = "https://github.com/snowflakedb/snowflake-cli"
 "Bug Tracker" = "https://github.com/snowflakedb/snowflake-cli/issues"
@@ -97,14 +97,17 @@
   "pip install test_external_plugins/snowpark_hello_single_command",
   "pip install test_external_plugins/multilingual_hello_command_group",
 ]
 features = ["development"]
 
 [tool.hatch.envs.integration.scripts]
 test = ["pytest -m integration --snapshot-warn-unused"]
+test-experimental = [
+  "pytest -m integration_experimental --snapshot-warn-unused",
+]
 
 [[tool.hatch.envs.local.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.coverage.run]
 source = ["snowflake.cli"]
 
@@ -121,18 +124,20 @@
   "TID252", # relative imports
   "SLF",    # Accessing private methods
   "F401",   # unused imports
   "F403",   # star imports
 ]
 
 [tool.pytest.ini_options]
-addopts = "-m 'not integration and not performance and not e2e and not spcs and not loaded_modules'"
+addopts = "-m 'not integration and not performance and not e2e and not spcs and not loaded_modules and not integration_experimental'"
 markers = [
   "integration: mark test as integration test",
   "performance: mark test as performance test",
   "e2e: mark test to execute on Snowflake CLI installed in fresh virtual environment",
   "loaded_modules: checks loaded modules",
+  "patch_app_version: sets app version to 0.0.0-test_patched",
+  "integration_experimental: experimental integration test",
 ]
 
 
 [tool.codespell]
 skip = 'tests/*'
```

### Comparing `snowflake_cli_labs-2.2.0rc0/PKG-INFO` & `snowflake_cli_labs-2.3.0rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake-cli-labs
-Version: 2.2.0rc0
+Version: 2.3.0rc0
 Summary: Snowflake CLI
 Project-URL: Source code, https://github.com/snowflakedb/snowflake-cli
 Project-URL: Bug Tracker, https://github.com/snowflakedb/snowflake-cli/issues
 Author: Snowflake Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -214,35 +214,41 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Requires-Python: >=3.8
 Requires-Dist: gitpython==3.1.43
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: pip
-Requires-Dist: pluggy==1.4.0
-Requires-Dist: pydantic==2.7.0
+Requires-Dist: pluggy==1.5.0
+Requires-Dist: pydantic==2.7.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requirements-parser==0.9.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: setuptools==69.5.1
-Requires-Dist: snowflake-connector-python[secure-local-storage]==3.8.1
+Requires-Dist: snowflake-connector-python[secure-local-storage]==3.10.0
 Requires-Dist: tomlkit==0.12.3
 Requires-Dist: typer==0.12.3
 Requires-Dist: urllib3<2.3,>=1.21.1
 Provides-Extra: development
-Requires-Dist: coverage==7.4.4; extra == 'development'
+Requires-Dist: coverage==7.5.0; extra == 'development'
 Requires-Dist: pre-commit>=3.5.0; extra == 'development'
 Requires-Dist: pytest-randomly==3.15.0; extra == 'development'
-Requires-Dist: pytest==8.1.1; extra == 'development'
+Requires-Dist: pytest==8.2.0; extra == 'development'
 Requires-Dist: syrupy==4.6.1; extra == 'development'
 Description-Content-Type: text/markdown
 
+[![Code quality checks](https://github.com/snowflakedb/snowflake-cli/actions/workflows/lint.yaml/badge.svg)](https://github.com/snowflakedb/snowflake-cli/actions/workflows/lint.yaml)
+[![Integration testing](https://github.com/snowflakedb/snowflake-cli/actions/workflows/integration_test.yaml/badge.svg)](https://github.com/snowflakedb/snowflake-cli/actions/workflows/integration_test.yaml)
+[![CLI Action testing](https://github.com/snowflakedb/snowflake-cli/actions/workflows/test_cli_action.yaml/badge.svg?branch=main)](https://github.com/snowflakedb/snowflake-cli/actions/workflows/test_cli_action.yaml)
+
+[//]: # ([![Python 3.11]&#40;https://img.shields.io/badge/python-3.11-blue.svg&#41;]&#40;https://www.python.org/downloads/release/python-311/&#41;)
+
 # Snowflake CLI
 
 Snowflake CLI is an open-source command-line tool explicitly designed for developer-centric workloads in addition to SQL operations. It is a flexible and extensible tool that can accommodate modern development practices and technologies.
 
 With Snowflake CLI, developers can create, manage, update, and view apps running on Snowflake across workloads such as Streamlit in Snowflake, the Snowflake Native App Framework, Snowpark Container Services, and Snowpark. It supports a range of Snowflake features, including user-defined functions, stored procedures, Streamlit in Snowflake, and SQL execution.
```


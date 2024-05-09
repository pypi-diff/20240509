# Comparing `tmp/typed_settings-24.2.0.tar.gz` & `tmp/typed_settings-24.3.0.tar.gz`

## Comparing `typed_settings-24.2.0.tar` & `typed_settings-24.3.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/Makefile
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/apiref.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/changelog.md
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/conf.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/conftest.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/development.md
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples.md
--rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/getting-started.md
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/index.md
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/license.md
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/why.md
--rw-r--r--   0        0        0   366071 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/1password-test-dark.png
--rw-r--r--   0        0        0   351000 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/1password-test-light.png
--rw-r--r--   0        0        0   387873 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/cli-argparse-dark.png
--rw-r--r--   0        0        0   361129 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/cli-argparse-light.png
--rw-r--r--   0        0        0   596177 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/cli-click-dark.png
--rw-r--r--   0        0        0   562046 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/cli-click-light.png
--rw-r--r--   0        0        0   394639 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/cli-rich_click-dark.png
--rw-r--r--   0        0        0   373242 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/cli-rich_click-light.png
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/custom.css
--rw-r--r--   0        0        0    33208 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/typed-settings-spacing.svg
--rw-r--r--   0        0        0    36882 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/typed-settings.png
--rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/_static/typed-settings.svg
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/black-pyproject.toml/black.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/black-pyproject.toml/pyproject.toml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/black-pyproject.toml/test.console
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pypirc_0/pypirc.toml
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pypirc_0/pypirc_0.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pypirc_0/test.console
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pypirc_1/pypirc.toml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pypirc_1/pypirc_1.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pypirc_1/test.console
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pytest-plugins/pytest.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/pytest-plugins/test.console
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/python-gitlab/python-gitlab.toml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/python-gitlab/python_gitlab.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/examples/python-gitlab/test.console
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/1password.md
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/basic-settings-loading.md
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/clis-argparse-or-click.md
--rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/clis-argparse.md
--rw-r--r--   0        0        0    27564 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/clis-click.md
--rw-r--r--   0        0        0    13655 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/config-files.md
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/environment-variables.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/index.md
--rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/post-processing.md
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/settings-classes.md
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 typed_settings-24.2.0/docs/guides/writing-custom-loaders.md
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/_compat.py
--rw-r--r--   0        0        0    14148 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/_core.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/_file_utils.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/_onepassword.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/argparse_utils.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/attrs.py
--rw-r--r--   0        0        0    20838 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/cli_argparse.py
--rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/cli_click.py
--rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/cli_utils.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/click_utils.py
--rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/cls_attrs.py
--rw-r--r--   0        0        0    15293 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/cls_utils.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/constants.py
--rw-r--r--   0        0        0    31222 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/converters.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/dict_utils.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/exceptions.py
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/loaders.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/mypy.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/processors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/py.typed
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 typed_settings-24.2.0/src/typed_settings/types.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/conftest.py
--rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/op
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_api.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_cli_argparse.py
--rw-r--r--   0        0        0    28460 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_cli_click.py
--rw-r--r--   0        0        0    26475 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_cli_param_types.py
--rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_cli_utils.py
--rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_cls_attrs.py
--rw-r--r--   0        0        0    21644 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_cls_utils.py
--rw-r--r--   0        0        0    20812 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_converters.py
--rw-r--r--   0        0        0    21577 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_core.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_dict_utils.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_file_utils.py
--rw-r--r--   0        0        0    19243 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_loaders.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_no_optionals.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_onepassword.py
--rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_processors.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_readme.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 typed_settings-24.2.0/tests/test_types.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 typed_settings-24.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 typed_settings-24.2.0/LICENSE
--rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 typed_settings-24.2.0/README.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 typed_settings-24.2.0/pyproject.toml
--rw-r--r--   0        0        0    10665 2020-02-02 00:00:00.000000 typed_settings-24.2.0/PKG-INFO
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/Makefile
+-rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/apiref.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/changelog.md
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/conf.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/conftest.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/development.md
+-rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples.md
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/getting-started.md
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/index.md
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/license.md
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/why.md
+-rw-r--r--   0        0        0   366071 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/1password-test-dark.png
+-rw-r--r--   0        0        0   351000 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/1password-test-light.png
+-rw-r--r--   0        0        0   387873 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/cli-argparse-dark.png
+-rw-r--r--   0        0        0   361129 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/cli-argparse-light.png
+-rw-r--r--   0        0        0   596177 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/cli-click-dark.png
+-rw-r--r--   0        0        0   562046 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/cli-click-light.png
+-rw-r--r--   0        0        0   394639 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/cli-rich_click-dark.png
+-rw-r--r--   0        0        0   373242 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/cli-rich_click-light.png
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    33208 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/typed-settings-spacing.svg
+-rw-r--r--   0        0        0    36882 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/typed-settings.png
+-rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/_static/typed-settings.svg
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/black-pyproject.toml/black.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/black-pyproject.toml/pyproject.toml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/black-pyproject.toml/test.console
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pypirc_0/pypirc.toml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pypirc_0/pypirc_0.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pypirc_0/test.console
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pypirc_1/pypirc.toml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pypirc_1/pypirc_1.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pypirc_1/test.console
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pytest-plugins/pytest.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/pytest-plugins/test.console
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/python-gitlab/python-gitlab.toml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/python-gitlab/python_gitlab.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/examples/python-gitlab/test.console
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/1password.md
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/basic-settings-loading.md
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/clis-argparse-or-click.md
+-rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/clis-argparse.md
+-rw-r--r--   0        0        0    27564 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/clis-click.md
+-rw-r--r--   0        0        0    13655 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/config-files.md
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/environment-variables.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/index.md
+-rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/post-processing.md
+-rw-r--r--   0        0        0     8702 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/settings-classes.md
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 typed_settings-24.3.0/docs/guides/writing-custom-loaders.md
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/_compat.py
+-rw-r--r--   0        0        0    14159 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/_core.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/_file_utils.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/_onepassword.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/argparse_utils.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/attrs.py
+-rw-r--r--   0        0        0    21833 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/cli_argparse.py
+-rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/cli_click.py
+-rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/cli_utils.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/click_utils.py
+-rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/cls_attrs.py
+-rw-r--r--   0        0        0    15465 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/cls_utils.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/constants.py
+-rw-r--r--   0        0        0    36629 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/converters.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/dict_utils.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/exceptions.py
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/loaders.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/mypy.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/processors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/py.typed
+-rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 typed_settings-24.3.0/src/typed_settings/types.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/conftest.py
+-rwxr-xr-x   0        0        0     2319 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/op
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_api.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_cli_argparse.py
+-rw-r--r--   0        0        0    28460 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_cli_click.py
+-rw-r--r--   0        0        0    29925 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_cli_param_types.py
+-rw-r--r--   0        0        0    14419 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_cli_utils.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_cls_attrs.py
+-rw-r--r--   0        0        0    21644 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_cls_utils.py
+-rw-r--r--   0        0        0    29343 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_converters.py
+-rw-r--r--   0        0        0    21577 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_core.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_dict_utils.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_file_utils.py
+-rw-r--r--   0        0        0    19243 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_loaders.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_no_optionals.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_onepassword.py
+-rw-r--r--   0        0        0    12217 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_processors.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_readme.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 typed_settings-24.3.0/tests/test_types.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 typed_settings-24.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 typed_settings-24.3.0/LICENSE
+-rw-r--r--   0        0        0     7479 2020-02-02 00:00:00.000000 typed_settings-24.3.0/README.md
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 typed_settings-24.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12422 2020-02-02 00:00:00.000000 typed_settings-24.3.0/PKG-INFO
```

### Comparing `typed_settings-24.2.0/docs/Makefile` & `typed_settings-24.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/apiref.rst` & `typed_settings-24.3.0/docs/apiref.rst`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/conf.py` & `typed_settings-24.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/conftest.py` & `typed_settings-24.3.0/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/examples.md` & `typed_settings-24.3.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/getting-started.md` & `typed_settings-24.3.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/index.md` & `typed_settings-24.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/why.md` & `typed_settings-24.3.0/docs/why.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 - Settings classes can be nested if you want to group your settings.
 
 - If it is installed, [cattrs] is used for converting the loaded values to the proper types.
   Typed Settings has a built-in converter that is used as a fallback.
   You can extend the existing converters or drop in your own.
 
-  - By default, all basic data types (bool, int, float, str) are supported, as well as enums, paths and datetimes.
+  - By default, all basic data types (bool, int, float, str) are supported, as well as enums, paths, datetimes and timedeltas.
     Most built-in collection types are supported, as well as optional values.
   - You can extend the converter to support additional types.
 
 
 ### Loading Settings
 
 - You define a list of settings loaders that are run one after another.
```

### Comparing `typed_settings-24.2.0/docs/_static/1password-test-dark.png` & `typed_settings-24.3.0/docs/_static/1password-test-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/1password-test-light.png` & `typed_settings-24.3.0/docs/_static/1password-test-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/cli-argparse-dark.png` & `typed_settings-24.3.0/docs/_static/cli-argparse-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/cli-argparse-light.png` & `typed_settings-24.3.0/docs/_static/cli-argparse-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/cli-click-dark.png` & `typed_settings-24.3.0/docs/_static/cli-click-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/cli-click-light.png` & `typed_settings-24.3.0/docs/_static/cli-click-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/cli-rich_click-dark.png` & `typed_settings-24.3.0/docs/_static/cli-rich_click-dark.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/cli-rich_click-light.png` & `typed_settings-24.3.0/docs/_static/cli-rich_click-light.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/custom.css` & `typed_settings-24.3.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/typed-settings-spacing.svg` & `typed_settings-24.3.0/docs/_static/typed-settings-spacing.svg`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/typed-settings.png` & `typed_settings-24.3.0/docs/_static/typed-settings.png`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/_static/typed-settings.svg` & `typed_settings-24.3.0/docs/_static/typed-settings.svg`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/examples/black-pyproject.toml/black.py` & `typed_settings-24.3.0/docs/examples/black-pyproject.toml/black.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/examples/black-pyproject.toml/test.console` & `typed_settings-24.3.0/docs/examples/black-pyproject.toml/test.console`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/examples/pytest-plugins/pytest.py` & `typed_settings-24.3.0/docs/examples/pytest-plugins/pytest.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/examples/pytest-plugins/test.console` & `typed_settings-24.3.0/docs/examples/pytest-plugins/test.console`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/examples/python-gitlab/python_gitlab.py` & `typed_settings-24.3.0/docs/examples/python-gitlab/python_gitlab.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/1password.md` & `typed_settings-24.3.0/docs/guides/1password.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/basic-settings-loading.md` & `typed_settings-24.3.0/docs/guides/basic-settings-loading.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/clis-argparse-or-click.md` & `typed_settings-24.3.0/docs/guides/clis-argparse-or-click.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/clis-argparse.md` & `typed_settings-24.3.0/docs/guides/clis-argparse.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/clis-click.md` & `typed_settings-24.3.0/docs/guides/clis-click.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/config-files.md` & `typed_settings-24.3.0/docs/guides/config-files.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/environment-variables.md` & `typed_settings-24.3.0/docs/guides/environment-variables.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/post-processing.md` & `typed_settings-24.3.0/docs/guides/post-processing.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/docs/guides/settings-classes.md` & `typed_settings-24.3.0/docs/guides/settings-classes.md`

 * *Files 8% similar despite different names*

```diff
@@ -256,7 +256,26 @@
 
 ```{code-block} ini
 :caption: mypy.ini
 
  [mypy]
  plugins=typed_settings.mypy
 ```
+
+
+## Forward References
+
+```{hint}
+Type annotations that are encoded as string literals (e.g. `x: "int"`) are called [forward references].
+
+Forward references can be resolved to actual types at runtime using functions like {func}`typing.get_type_hints()` or {func}`attrs.resolve_types()`}.
+
+[forward references]: https://peps.python.org/pep-0484/#forward-references
+```
+
+Typed Settings tries to resolve forward references when loading settings or
+combining settings from attrs classes to new classes.
+
+This may not always work reliably,
+especially if classes are defined inside nested scopes (i.e., inside functions or other classes).
+
+In these cases, you can try to manually pass your settings class to {func}`typing.get_type_hints()` or {func}`attrs.resolve_types()`.
```

### Comparing `typed_settings-24.2.0/docs/guides/writing-custom-loaders.md` & `typed_settings-24.3.0/docs/guides/writing-custom-loaders.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/__init__.py` & `typed_settings-24.3.0/src/typed_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/_core.py` & `typed_settings-24.3.0/src/typed_settings/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,18 @@
     for processor in state.processors:
         settings_dict = processor(settings_dict, state.settings_class, state.options)
     merged_settings = dict_utils.update_settings(merged_settings, settings_dict)
 
     return merged_settings
 
 
-def convert(merged_settings: MergedSettings, state: SettingsState[ST]) -> ST:
+def convert(
+    merged_settings: MergedSettings,
+    state: SettingsState[ST],
+) -> ST:
     """
     Create an instance of *cls* from the settings in *merged_settings*.
 
     Args:
         merged_settings: The loaded and merged settings by settings name.
         state: The state and configuration for this run.
```

### Comparing `typed_settings-24.2.0/src/typed_settings/_file_utils.py` & `typed_settings-24.3.0/src/typed_settings/_file_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/_onepassword.py` & `typed_settings-24.3.0/src/typed_settings/_onepassword.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 
     Raise:
         ValueError: If the CLI is not properly installed or the invocation
             failed.
     """
     cmd = ("op", *args)
     try:
-        result = subprocess.run(
-            cmd, capture_output=True, text=True, check=True  # noqa: S603
-        )
+        result = subprocess.run(cmd, capture_output=True, text=True, check=True)  # noqa: S603
     except FileNotFoundError:
         raise ValueError(
             "The 1Password CLI is not properly installed.  You can find help "
             "here: https://developer.1password.com/docs/cli/"
         ) from None
     except subprocess.CalledProcessError as e:
         _level, _date, _time, msg = e.stderr.strip().split(" ", maxsplit=3)
```

### Comparing `typed_settings-24.2.0/src/typed_settings/cli_argparse.py` & `typed_settings-24.3.0/src/typed_settings/cli_argparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Utilities for generating an :mod:`argparse` based CLI.
 
 .. versionadded:: 2.0.0
 """
 
 import argparse
 import itertools
-from datetime import datetime
+from datetime import date, datetime, timedelta
 from enum import Enum
-from functools import wraps
+from functools import partial, wraps
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Collection,
     Dict,
@@ -25,27 +25,27 @@
     Union,
 )
 
 
 if TYPE_CHECKING:
     from argparse import FileType
 
-from . import _core
+from . import _core, converters
 from .cli_utils import (
     DEFAULT_SENTINEL,
     DEFAULT_SENTINEL_NAME,
     NO_DEFAULT,
     Default,
     StrDict,
     TypeArgsMaker,
     TypeHandlerFunc,
     get_default,
 )
 from .constants import ARGPARSE_METADATA_KEY as METADATA_KEY
-from .converters import Converter, default_converter
+from .converters import Converter
 from .loaders import Loader
 from .processors import Processor
 from .types import (
     SECRET_REPR,
     ST,
     LoadedValue,
     LoaderMeta,
@@ -75,24 +75,54 @@
 
 
 def handle_datetime(type: type, default: Default, is_optional: bool) -> StrDict:
     """
     Handle isoformatted datetimes.
     """
     kwargs: StrDict = {
-        "type": datetime.fromisoformat,
+        "type": partial(converters.to_datetime, cls=datetime),
         "metavar": "YYYY-MM-DD[Thh:mm:ss[+xx:yy]]",
     }
     if isinstance(default, datetime):
         kwargs["default"] = default.isoformat()
     elif is_optional:
         kwargs["default"] = None
     return kwargs
 
 
+def handle_date(type: type, default: Default, is_optional: bool) -> StrDict:
+    """
+    Handle isoformatted datetimes.
+    """
+    kwargs: StrDict = {
+        "type": partial(converters.to_date, cls=date),
+        "metavar": "YYYY-MM-DD",
+    }
+    if isinstance(default, date):
+        kwargs["default"] = default.isoformat()
+    elif is_optional:
+        kwargs["default"] = None
+    return kwargs
+
+
+def handle_timedelta(type: type, default: Default, is_optional: bool) -> StrDict:
+    """
+    Handle isoformatted datetimes.
+    """
+    kwargs: StrDict = {
+        "type": partial(converters.to_timedelta, cls=timedelta),
+        "metavar": "[-][Dd][HHh][MMm][SS[.ffffff]s]",
+    }
+    if isinstance(default, timedelta):
+        kwargs["default"] = converters.timedelta_to_str(default)
+    elif is_optional:
+        kwargs["default"] = None
+    return kwargs
+
+
 def handle_enum(type: Type[Enum], default: Default, is_optional: bool) -> StrDict:
     """
     Use *choices* as option type and use the enum value's name as default.
     """
     kwargs: StrDict = {"choices": list(type.__members__)}
     if isinstance(default, type):
         # Convert Enum instance to string
@@ -115,14 +145,16 @@
 
     return kwargs
 
 
 #: Default handlers for argparse option types.
 DEFAULT_TYPES: Dict[type, TypeHandlerFunc] = {
     datetime: handle_datetime,
+    date: handle_date,
+    timedelta: handle_timedelta,
     Enum: handle_enum,
     Path: handle_path,
 }
 
 
 class ArgparseHandler:
     """
@@ -276,15 +308,15 @@
     .. versionchanged:: 23.0.0
        Added the *processors* argument
     .. versionchanged:: 23.1.0
        Added the *base_dir* argument
     """
     if isinstance(loaders, str):
         loaders = _core.default_loaders(loaders)
-    converter = converter or default_converter()
+    converter = converter or converters.default_converter()
     state = _core.SettingsState(settings_cls, loaders, processors, converter, base_dir)
     type_args_maker = type_args_maker or TypeArgsMaker(ArgparseHandler())
 
     decorator = _get_decorator(state, type_args_maker, **parser_kwargs)
     return decorator
 
 
@@ -341,15 +373,15 @@
     .. versionchanged:: 23.0.0
        Added the *processors* argument
     .. versionchanged:: 23.1.0
        Added the *base_dir* argument
     """
     if isinstance(loaders, str):
         loaders = _core.default_loaders(loaders)
-    converter = converter or default_converter()
+    converter = converter or converters.default_converter()
     state = _core.SettingsState(settings_cls, loaders, processors, converter, base_dir)
     type_args_maker = type_args_maker or TypeArgsMaker(ArgparseHandler())
 
     return _mk_parser(state, type_args_maker, **parser_kwargs)
 
 
 def namespace2settings(
@@ -379,15 +411,15 @@
             settings.
 
     Return: An instance of *settings_cls*.
 
     .. versionchanged:: 23.1.0
        Added the *base_dir* argument
     """
-    converter = converter or default_converter()
+    converter = converter or converters.default_converter()
     state = _core.SettingsState(settings_cls, [], [], converter, base_dir)
     return _ns2settings(namespace, state, merged_settings)
 
 
 def _get_decorator(
     state: _core.SettingsState[ST],
     type_args_maker: TypeArgsMaker,
```

### Comparing `typed_settings-24.2.0/src/typed_settings/cli_click.py` & `typed_settings-24.3.0/src/typed_settings/cli_click.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Utilities for generating Click options.
 """
 
-from datetime import datetime
+from datetime import date, datetime, timedelta
 from enum import Enum
 from functools import partial, update_wrapper
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Collection,
@@ -24,15 +24,15 @@
     cast,
     overload,
 )
 
 import click
 from click.core import ParameterSource
 
-from . import _core, cls_utils
+from . import _core, cls_utils, converters
 from .cli_utils import (
     DEFAULT_SENTINEL_NAME,
     NO_DEFAULT,
     Default,
     StrDict,
     TypeArgsMaker,
     TypeHandlerFunc,
@@ -462,14 +462,50 @@
     if isinstance(default, datetime):
         kwargs["default"] = default.isoformat()
     elif is_optional:
         kwargs["default"] = None
     return kwargs
 
 
+def handle_date(type: type, default: Default, is_optional: bool) -> StrDict:
+    """
+    Use :class:`click.DateTime` as option type and convert the default value
+    to an ISO string.
+    """
+    typ = partial(converters.to_date, cls=date)
+    typ.__name__ = converters.to_date.__name__  # type: ignore[attr-defined]
+    kwargs: StrDict = {
+        "type": typ,
+        "metavar": "[%Y-%m-%d]",
+    }
+    if isinstance(default, date):
+        kwargs["default"] = default.isoformat()
+    elif is_optional:
+        kwargs["default"] = None
+    return kwargs
+
+
+def handle_timedelta(type: type, default: Default, is_optional: bool) -> StrDict:
+    """
+    Use :class:`click.DateTime` as option type and convert the default value
+    to an ISO string.
+    """
+    typ = partial(converters.to_timedelta, cls=timedelta)
+    typ.__name__ = converters.to_timedelta.__name__  # type: ignore[attr-defined]
+    kwargs: StrDict = {
+        "type": typ,
+        "metavar": "[-][Dd][HHh][MMm][SS[.ffffff]s]",
+    }
+    if isinstance(default, timedelta):
+        kwargs["default"] = converters.timedelta_to_str(default)
+    elif is_optional:
+        kwargs["default"] = None
+    return kwargs
+
+
 def handle_enum(type: Type[Enum], default: Default, is_optional: bool) -> StrDict:
     """
     Use :class:`click.Choice` as option type and use the enum value's name as
     default.
     """
     kwargs: StrDict = {"type": click.Choice(list(type.__members__))}
     if isinstance(default, type):
@@ -480,14 +516,16 @@
 
     return kwargs
 
 
 #: Default handlers for click option types.
 DEFAULT_TYPES: Dict[type, TypeHandlerFunc] = {
     datetime: handle_datetime,
+    date: handle_date,
+    timedelta: handle_timedelta,
     Enum: handle_enum,
 }
 
 
 class ClickHandler:
     """
     Implementation of the :class:`~typed_settings.cli_utils.TypeHandler`
```

### Comparing `typed_settings-24.2.0/src/typed_settings/cli_utils.py` & `typed_settings-24.3.0/src/typed_settings/cli_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/cls_attrs.py` & `typed_settings-24.3.0/src/typed_settings/cls_attrs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Helpers for and additions to :mod:`attrs`.
 """
 
+import sys
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Mapping,
     Optional,
@@ -376,17 +377,15 @@
         init_name = attr_name if attr_name[0] != "_" else attr_name[1:]
         old_value = getattr(inst, attr_name)
         if init_name not in changes:
             # Add original value to changes
             changes[init_name] = old_value
         elif attrs.has(old_value) and isinstance(changes[init_name], Mapping):
             # Evolve nested attrs classes
-            changes[init_name] = evolve(
-                old_value, **changes[init_name]  # type: ignore[arg-type]
-            )
+            changes[init_name] = evolve(old_value, **changes[init_name])  # type: ignore[arg-type]
 
     return cls(**changes)
 
 
 def combine(
     name: str,
     base_cls: Type[attrs.AttrsInstance],
@@ -465,15 +464,26 @@
             kw_only=a.kw_only,
             eq=a.eq,
             order=a.order,
             on_setattr=a.on_setattr,
         )
         for a in attr.fields(base_cls)  # type: ignore[misc]
     }
+    annotations = dict(base_cls.__annotations__)
     for aname, default in nested.items():
         if aname in attribs:
             raise ValueError(f"Duplicate attribute for nested class: {aname}")
         attribs[aname] = attr.attrib(default=default, type=default.__class__)
+        annotations[aname] = default.__class__
+
+    try:
+        globalns = sys.modules[base_cls.__module__].__dict__
+    except KeyError:  # pragma: no cover
+        globalns = None
 
     cls = attr.make_class(name, attribs)
+    cls.__annotations__ = annotations
     cls.__doc__ = base_cls.__doc__
+    # Store globals in class so that they can later be used,
+    # see ".cls_utils.Attrs.iter_fields()".
+    cls.__globals__ = globalns  # type: ignore[attr-defined]
     return cls
```

### Comparing `typed_settings-24.2.0/src/typed_settings/cls_utils.py` & `typed_settings-24.3.0/src/typed_settings/cls_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,19 @@
     @staticmethod
     def iter_fields(cls: type) -> types.OptionList:
         import attrs
 
         result: List[types.OptionInfo] = []
 
         def iter_attribs(r_cls: type, prefix: str) -> None:
-            r_cls = attrs.resolve_types(r_cls)  # type: ignore[type-var]
+            # Resolve types, optionally using the globals we stored in the class in
+            # ".cls_attrs.combine()":
+            r_cls = attrs.resolve_types(
+                r_cls, globalns=getattr(r_cls, "__globals__", None)
+            )
             for field in attrs.fields(r_cls):  # type: ignore[misc]
                 if field.init is False:
                     continue
                 if field.type is not None and attrs.has(field.type):
                     iter_attribs(field.type, f"{prefix}{field.name}.")
                 else:
                     is_nothing = field.default is attrs.NOTHING
```

### Comparing `typed_settings-24.2.0/src/typed_settings/converters.py` & `typed_settings-24.3.0/src/typed_settings/converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Converters and structure hooks for various data types.
 """
 
 import dataclasses
-from datetime import datetime
+import re
+from datetime import date, datetime, timedelta
 from enum import Enum
 from pathlib import Path
 from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -21,15 +22,15 @@
     Tuple,
     Type,
     Union,
     get_args,
     get_origin,
 )
 
-from ._compat import PY_310
+from ._compat import PY_310, PY_311
 
 
 if PY_310:
     from types import UnionType
 else:
     from typing import Union as UnionType  # type: ignore
 
@@ -44,15 +45,15 @@
 # __all__ = [
 #     "Converter",
 #     "TSConverter",
 #     "default_converter",
 #     "get_default_structure_hooks",
 #     "register_attrs_hook_factory",
 #     "register_strlist_hook",
-#     "to_dt",
+#     "to_datetime",
 #     "to_bool",
 #     "to_enum",
 #     "to_path",
 #     "to_resolved_path",
 # ]
 
 
@@ -102,15 +103,17 @@
 
         self.scalar_converters: Dict[Any, Callable[[Any, type], Any]] = {
             Any: to_any,
             bool: to_bool,
             int: to_type,
             float: to_type,
             str: to_type,
-            datetime: to_dt,
+            datetime: to_datetime,
+            date: to_date,  # Must come after "datetime" b/c of subclassing!
+            timedelta: to_timedelta,
             Enum: to_enum,
             Path: to_resolved_path if resolve_paths else to_path,
         }
         try:
             import pydantic
 
             self.scalar_converters[pydantic.SecretBytes] = to_pydantic_secretbytes
@@ -180,15 +183,17 @@
         :class:`TSConverter`.  The converters are configured to handle the following
         types:
 
         - :class:`bool` (see :func:`to_bool()` for supported inputs)
         - :class:`int`
         - :class:`float`
         - :class:`str`
-        - :class:`datetime.datetime` (see :func:`to_dt()`)
+        - :class:`datetime.datetime` (see :func:`to_datetime()`)
+        - :class:`datetime.date` (see :func:`to_date()`)
+        - :class:`datetime.timedelta` (see :func:`to_timedelta()`)
         - :class:`enum.Enum` using (see :func:`to_enum()`)
         - :class:`pathlib.Path` (see :func:`to_path()` and :func:`to_resolved_path()`)
         - :class:`list`
         - :class:`tuple`
         - :class:`dict`
         - :class:`types.MappingProxyType` ("read-only" dicts)
         - :class:`set`
@@ -204,14 +209,16 @@
 
     This converter can also be used as a base for converters with custom
     structure hooks.
 
     .. versionchanged:: 23.1.0
        Return a :program:`cattrs` converter if it is installed or else a Typed Settings
        converter.
+    .. versionchanged:: 24.3.0
+       Added :func:`to_date()` and :func:`to_timedelta()`.
     """
     try:
         import cattrs  # noqa: F401
     except ImportError:
         return get_default_ts_converter(resolve_paths=resolve_paths)
     else:
         return get_default_cattrs_converter(resolve_paths=resolve_paths)
@@ -277,15 +284,17 @@
     Return:
         A list of tuples that can be used as args for
         :meth:`cattrs.BaseConverter.register_structure_hook()`.
     """
     path_hook = to_resolved_path if resolve_paths else to_path
     hooks: List[Tuple[type, Callable[[Any, type], Any]]] = [
         (bool, to_bool),
-        (datetime, to_dt),
+        (datetime, to_datetime),
+        (date, to_date),
+        (timedelta, to_timedelta),
         (Enum, to_enum),
         (Path, path_hook),
     ]
     try:
         import pydantic
 
         hooks.append((pydantic.SecretBytes, to_pydantic_secretbytes))
@@ -507,44 +516,213 @@
             return False
     except TypeError:
         # Raised when "val" is not hashable (e.g., lists)
         pass
     raise ValueError(f"Cannot convert value to bool: {value}")
 
 
-def to_dt(value: Union[datetime, str], _cls: type = datetime) -> datetime:
+def to_date(value: Union[datetime, str], cls: Type[date] = date) -> date:
     """
-    Convert an ISO formatted string to :class:`datetime.datetime`.  Leave the
-    input untouched if it is already a datetime.
+    Convert an ISO formatted string to :class:`datetime.date`.  Leave the input
+    untouched if it is already a date.
+
+    See: :meth:`datetime.date.fromisoformat()`
+
+    Args:
+        value: The input data
+        cls: The target type.  Must be :class:`datetime.date` or a subclass.
+
+    Return:
+        The converted date instance
+
+    Raise:
+        TypeError: If *value* is neither a string nor a date
+        ValueError: If *value* cannot be parsed as date.
+
+    .. versionadded:: 24.3.0
+    """
+    if not isinstance(value, (date, str)):
+        raise TypeError(
+            f"Invalid type {type(value).__name__!r}; expected 'date' or " f"'str'."
+        )
+    if isinstance(value, str):
+        return cls.fromisoformat(value)
+    return value
+
+
+def to_datetime(
+    value: Union[datetime, str], cls: Type[datetime] = datetime
+) -> datetime:
+    """
+    Convert an ISO formatted string to :class:`datetime.datetime`.  Leave the input
+    untouched if it is already a datetime.
 
     See: :meth:`datetime.datetime.fromisoformat()`
 
-    The ``Z`` suffix is also supported and will be replaced with ``+00:00``.
+    The ``Z`` suffix is supported on Python versions prior to 3.11, too.
 
     Args:
         value: The input data
-        _cls: (ignored)
+        cls: The target type.  Must be :class:`datetime.datetime` or a subclass.
 
     Return:
         The converted datetime instance
 
     Raise:
-        TypeError: If *val* is neither a string nor a datetime
+        TypeError: If *value* is neither a string nor a datetime
+        ValueError: If *value* cannot be parsed as datetime.
     """
     if not isinstance(value, (datetime, str)):
         raise TypeError(
             f"Invalid type {type(value).__name__!r}; expected 'datetime' or " f"'str'."
         )
     if isinstance(value, str):
-        if value[-1] == "Z":
+        if not PY_311 and value[-1] == "Z":
             value = value.replace("Z", "+00:00")
-        return datetime.fromisoformat(value)
+        return cls.fromisoformat(value)
     return value
 
 
+_SIGN = "(?P<sign>[+-])?"
+_DAYS = "(?P<days>[0-9]+)"
+_HOURS = "(?P<hours>[0-9]+)"
+_MINUTES = "(?P<minutes>[0-9]+)"
+_SECONDS = r"(?P<seconds>[0-9]+)(\.(?P<micros>[0-9]{1,6}))?"
+# [±][{D}d[,]][[{HH}:]{MM}:]{SS}[.{ffffff}]
+RE_TIMEDELTA_SIMPLE = re.compile(
+    f"^{_SIGN}({_DAYS}D,?)?(({_HOURS}:)?{_MINUTES}:)?{_SECONDS}$", flags=re.IGNORECASE
+)
+# [±][{D}d][{HH}h][{MM}m][{SS}[.{ffffff}]s]
+RE_TIMEDELTA_SIMPLE_ISO = re.compile(
+    f"^{_SIGN}({_DAYS}D)?({_HOURS}H)?({_MINUTES}M)?({_SECONDS}S)?$", flags=re.IGNORECASE
+)
+# [±]P[{D}D][T[{HH}H][{MM}M][{SS}[.{ffffff}]S]]
+RE_TIMEDELTA_ISO = re.compile(
+    f"^{_SIGN}"
+    r"P(?!\b)"  # "P", but not on a word boundary (e.g., at the end of the string)
+    f"({_DAYS}D)?"
+    f"("
+    r"T(?!\b)"  # "T", but not on a word boundary (e.g., at the end of the string)
+    f"({_HOURS}H)?"
+    f"({_MINUTES}M)?"
+    f"({_SECONDS}S)?"
+    r")?$",
+    flags=re.IGNORECASE,
+)
+
+
+def to_timedelta(
+    value: Union[timedelta, int, float, str], cls: Type[timedelta]
+) -> timedelta:
+    """
+    Convert *value* to a :class:`datetime.timedelta`.
+
+    Accepts strings, integers and floats, and timedelta instances.
+
+    Timedelta instances are returned unchanged.
+
+    Integers and floats are interpreted as seconds.
+
+    Supported string formats (all are case-insensitive):
+
+    - :samp:`[±]P[{D}D][T[{HH}H][{MM}M][{SS}[.{ffffff}]S]]` (`ISO durations`_), e.g.:
+
+      - ``P1DT03H04M05S``
+      - ``-P180D``
+      - ``PT4H30M``
+      - ``P1DT30S``
+
+    - :samp:`[±][{D}d][{HH}h][{MM}m][{SS}[.{ffffff}]s]` (simplified ISO variant), e.g.:
+
+      - ``1d3h4m5s``
+      - ``-180d``
+      - ``4h30m``
+      - ``1d30s``
+
+    - :samp:`[±][{D}d[,]][[{HH}:]{MM}:]{SS}[.{ffffff}]`, e.g.:
+
+      - ``1d,03:04:05``
+      - ``-180D``
+      - ``4:30:00``
+      - ``1d30``
+
+    .. _iso durations: https://en.wikipedia.org/wiki/ISO_8601#Durations
+
+    Args:
+        value: The input data
+        cls: The target type.  Must be :class:`datetime.timedelta` or a subclass.
+
+    Return:
+        The converted timedelta instance
+
+    Raise:
+        TypeError: If *value* is neither a string, float, or int nor a timedelta.
+        ValueError: If *value* cannot be parsed as timedelta.
+
+    .. versionadded:: 24.3.0
+    """
+    if not isinstance(value, (timedelta, str, float, int)):
+        raise TypeError(
+            f"Invalid type {type(value).__name__!r}; expected 'timedelta', 'float', "
+            f"'int', or 'str'."
+        )
+
+    if isinstance(value, timedelta):
+        return value
+
+    if isinstance(value, (int, float)):
+        return cls(seconds=value)
+
+    for regex in (RE_TIMEDELTA_ISO, RE_TIMEDELTA_SIMPLE_ISO, RE_TIMEDELTA_SIMPLE):
+        match = regex.match(value)
+        if match:
+            break
+    else:
+        raise ValueError(f"Cannot parse value as timedelta: {value}")
+
+    parts = match.groupdict(default="0")
+    days = int(parts["days"])
+    hours = int(parts["hours"])
+    minutes = int(parts["minutes"])
+    seconds = int(parts["seconds"])
+    # Append "0" to "micros" to get a 6-digit number (.7 -> 7 -> 700_000)
+    micros = int(f"{parts['micros']:<06}")
+
+    td = cls(
+        days=days, hours=hours, minutes=minutes, seconds=seconds, microseconds=micros
+    )
+    if parts["sign"] == "-":
+        return -td
+    return td
+
+
+def timedelta_to_str(td: timedelta) -> str:
+    """
+    Serialize a timedelta to a string that can be parsed by :func:`to_timedelta()`.
+    """
+    if td == abs(td):
+        is_negative = False
+    else:
+        is_negative = True
+        td = -td
+    days = td.days
+    hours, seconds = divmod(td.seconds, 3600)
+    minutes, seconds = divmod(seconds, 60)
+    micros = f".{td.microseconds:>06}".rstrip("0") if td.microseconds else ""
+    result = (
+        f"{f'{days}d' if days else ''}"
+        f"{f'{hours}h' if hours else ''}"
+        f"{f'{minutes}m' if minutes else ''}"
+        f"{f'{seconds}{micros}s' if seconds or micros else ''}"
+    )
+    if result and is_negative:
+        result = f"-{result}"
+    return result
+
+
 def to_enum(value: Any, cls: Type[ET]) -> ET:
     """
     Return an instance of the enum *cls* for *value*.
 
     If the to be converted value is not already an enum, the converter will
     create one by name (``MyEnum[val]``).
 
@@ -767,17 +945,15 @@
 
             if not isinstance(value, dict):
                 raise TypeError(
                     f'Invalid type "{type(value).__name__}"; expected '
                     f'"{cls.__name__}" or "dict".'
                 )
 
-            fields = {
-                f.name: f for f in dataclasses.fields(cls)  # type: ignore[arg-type]
-            }
+            fields = {f.name: f for f in dataclasses.fields(cls)}  # type: ignore[arg-type]
             values = {
                 n: converter.structure(v, fields[n].type)  # type: ignore[arg-type]
                 for n, v in value.items()
             }
             return cls(**values)
 
         return convert
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typed_settings-24.2.0/src/typed_settings/dict_utils.py` & `typed_settings-24.3.0/src/typed_settings/dict_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/exceptions.py` & `typed_settings-24.3.0/src/typed_settings/exceptions.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/loaders.py` & `typed_settings-24.3.0/src/typed_settings/loaders.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/mypy.py` & `typed_settings-24.3.0/src/typed_settings/mypy.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/processors.py` & `typed_settings-24.3.0/src/typed_settings/processors.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/src/typed_settings/types.py` & `typed_settings-24.3.0/src/typed_settings/types.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/conftest.py` & `typed_settings-24.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/op` & `typed_settings-24.3.0/tests/op`

 * *Files 8% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """
     try:
         _schema, _, vault, item, field = resource.split("/")
         data = VAULT_DATA[vault][item][field]
     except (KeyError, ValueError):
         click.echo(
             (
-                f"[ERROR] YYYY/MM/DD HH:MM:SS could not read secret {resource}: "
+                f"[ERROR] YYYY/MM/DD HH:MM:SS could not read secret '{resource}': "
                 f"invalid secret reference"
             ),
             err=True,
         )
         ctx.exit(1)
 
     click.echo(data)
```

### Comparing `typed_settings-24.2.0/tests/test_api.py` & `typed_settings-24.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_cli_argparse.py` & `typed_settings-24.3.0/tests/test_cli_argparse.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_cli_click.py` & `typed_settings-24.3.0/tests/test_cli_click.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_cli_param_types.py` & `typed_settings-24.3.0/tests/test_cli_param_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tests for supported CLI param types for both, Click and argparse.
 """
 
 import re
-from datetime import datetime, timezone
+from datetime import date, datetime, timedelta, timezone
 from enum import Enum
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     ClassVar,
     Dict,
@@ -336,14 +336,129 @@
     expected_settings = Settings(
         datetime(2020, 5, 4),
         datetime(2020, 5, 4, 13, 37),
         datetime(2020, 5, 4, 13, 37, tzinfo=timezone.utc),
     )
 
 
+class TestDateParam(ParamBase):
+    """
+    Test date cli_options.
+    """
+
+    @settings
+    class Settings:
+        a: date
+        b: date = date(1970, 1, 1)
+        c: Optional[date] = None
+
+    click_expected_help = [
+        "  --a [%Y-%m-%d]  [required]",
+        "  --b [%Y-%m-%d]  [default: 1970-01-01]",
+        "  --c [%Y-%m-%d]",
+    ]
+    argparse_expected_help = [
+        "  --a YYYY-MM-DD  [required]",
+        "  --b YYYY-MM-DD  [default: 1970-01-01]",
+        "  --c YYYY-MM-DD",
+    ]
+
+    env_vars = {
+        "A": "2021-05-04",
+    }
+    click_expected_env_var_defaults = [
+        "  --a [%Y-%m-%d]  [default: 2021-05-04]",
+        "  --b [%Y-%m-%d]  [default: 1970-01-01]",
+        "  --c [%Y-%m-%d]",
+    ]
+    argparse_expected_env_var_defaults = [
+        "  --a YYYY-MM-DD  [default: 2021-05-04]",
+        "  --b YYYY-MM-DD  [default: 1970-01-01]",
+        "  --c YYYY-MM-DD",
+    ]
+
+    default_options = ["--a=2020-05-04"]
+    expected_defaults = Settings(date(2020, 5, 4))
+
+    cli_options = [
+        "--a=2020-05-04",
+    ]
+    expected_settings = Settings(date(2020, 5, 4))
+
+
+class TestTimedeltaParam(ParamBase):
+    """
+    Test date cli_options.
+    """
+
+    @settings
+    class Settings:
+        a: timedelta
+        b: timedelta = timedelta(days=1, seconds=4)
+        c: timedelta = timedelta(days=1, seconds=4)
+        d: Optional[timedelta] = None
+
+    click_expected_help = [
+        "  --a [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                                  [required]",
+        "  --b [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                                  [default: 1d4s]",
+        "  --c [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                                  [default: 1d4s]",
+        "  --d [-][Dd][HHh][MMm][SS[.ffffff]s]",
+    ]
+    argparse_expected_help = [
+        "  --a [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                        [required]",
+        "  --b [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                        [default: 1d4s]",
+        "  --c [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                        [default: 1d4s]",
+        "  --d [-][Dd][HHh][MMm][SS[.ffffff]s]",
+    ]
+
+    env_vars = {
+        "A": "P1DT03H04M",
+        "B": "3h4m",
+        "C": "03:04:02",
+    }
+    click_expected_env_var_defaults = [
+        "  --a [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                                  [default: 1d3h4m]",
+        "  --b [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                                  [default: 3h4m]",
+        "  --c [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                                  [default: 3h4m2s]",
+        "  --d [-][Dd][HHh][MMm][SS[.ffffff]s]",
+    ]
+    argparse_expected_env_var_defaults = [
+        "  --a [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                        [default: 1d3h4m]",
+        "  --b [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                        [default: 3h4m]",
+        "  --c [-][Dd][HHh][MMm][SS[.ffffff]s]",
+        "                        [default: 3h4m2s]",
+        "  --d [-][Dd][HHh][MMm][SS[.ffffff]s]",
+    ]
+
+    default_options = ["--a=1d"]
+    expected_defaults = Settings(timedelta(days=1))
+
+    cli_options = [
+        "--a=1d",
+        "--b=1h",
+        "--c=1d2h3m4s",
+    ]
+    expected_settings = Settings(
+        timedelta(days=1),
+        timedelta(hours=1),
+        timedelta(days=1, hours=2, minutes=3, seconds=4),
+    )
+
+
 class TestEnumParam(ParamBase):
     """
     Test enum cli_options.
     """
 
     @settings
     class Settings:
```

### Comparing `typed_settings-24.2.0/tests/test_cli_utils.py` & `typed_settings-24.3.0/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_cls_attrs.py` & `typed_settings-24.3.0/tests/test_cls_attrs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tests for "typed_settings.cls_attrs".
 """
 
 import typing as t
+from pathlib import Path
 
 import attrs
 import pytest
 
 from typed_settings import cli_argparse, cli_click, constants
 from typed_settings.cls_attrs import (
     SECRET,
@@ -303,17 +304,15 @@
 
         Composed = combine(
             "Composed",
             BaseSettings,
             {"n1": Nested1(), "n2": Nested2()},
         )
         assert Composed.__name__ == "Composed"
-        assert [
-            (f.name, f.type, f.default) for f in attrs.fields(Composed)  # type: ignore
-        ] == [
+        assert [(f.name, f.type, f.default) for f in attrs.fields(Composed)] == [  # type: ignore
             ("a", str, ""),
             ("n1", Nested1, Nested1()),
             ("n2", Nested2, Nested2()),
         ]
 
     def test_duplicate_attrib(self) -> None:
         """
@@ -351,7 +350,40 @@
         class BaseSettings:
             """Le doc string."""
 
             a: str = ""
 
         Composed = combine("Composed", BaseSettings, {"n1": Nested1()})
         assert Composed.__doc__ == "Le doc string."
+
+    def test_postponed_annotations(self) -> None:
+        """
+        The created class copies the annotations from the base and adds entries for all
+        nested classes.
+
+        See: https://gitlab.com/sscherfke/typed-settings/-/issues/54
+        """
+
+        @attrs.define
+        class Nested1:
+            a: "str" = ""
+
+        @attrs.define
+        class BaseSettings:
+            a: "bool" = False
+            p: "Path" = Path.cwd()
+
+        Composed = combine("Composed", BaseSettings, {"n1": Nested1()})
+
+        # Composed has __annotations__ populated with base and nested attribs
+        assert Composed.__annotations__ == {
+            "a": "bool",
+            "p": "Path",
+            "n1": Nested1,
+        }
+
+        # Types can be resolved
+        Composed = attrs.resolve_types(Composed, globalns=globals())
+        fields = attrs.fields(Composed)
+        assert fields.a.type is bool
+        assert fields.p.type is Path
+        assert fields.n1.type is Nested1
```

### Comparing `typed_settings-24.2.0/tests/test_cls_utils.py` & `typed_settings-24.3.0/tests/test_cls_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_converters.py` & `typed_settings-24.3.0/tests/test_converters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Tests for `typed_settings.attrs.converters`.
 """
 
 import dataclasses
 import json
-from datetime import datetime, timedelta, timezone
+from datetime import date, datetime, timedelta, timezone
 from enum import Enum
 from pathlib import Path
 from types import MappingProxyType
 from typing import (
     Any,
     Callable,
     Dict,
@@ -21,17 +21,18 @@
     Union,
 )
 
 import attrs
 import cattrs
 import pydantic
 import pytest
+from hypothesis import assume, given, strategies
 
 from typed_settings import converters
-from typed_settings._compat import PY_39, PY_310
+from typed_settings._compat import PY_39, PY_310, PY_311
 from typed_settings.cls_attrs import option, secret, settings
 
 
 def custom_converter(v: Union[str, Path]) -> Path:
     """A custom converter for attrs fields."""
     return Path(v).resolve()
 
@@ -174,15 +175,15 @@
     ("int('42')", "42", 42, int),
     ("float(3.14)", 3.14, 3.14, float),
     ("float('.815')", ".815", 0.815, float),
     ("str('spam')", "spam", "spam", str),
 ]
 SUPPORTED_TYPES_DATA += SUPPORTED_STDTYPES
 
-# datetime - can be parsed from a limit set of ISO formats
+# datetime - can be parsed from ISO format
 SUPPORTED_DATETIME: Example3T = [
     ("datetime(naive-space)", "2020-05-04 13:37:00", datetime(2020, 5, 4, 13, 37)),
     ("datetime(naive-T)", "2020-05-04T13:37:00", datetime(2020, 5, 4, 13, 37)),
     (
         "datetime(tz-Z)",
         "2020-05-04T13:37:00Z",
         datetime(2020, 5, 4, 13, 37, tzinfo=timezone.utc),
@@ -197,14 +198,79 @@
         "2020-05-04T13:37:00+02:00",
         datetime(2020, 5, 4, 13, 37, tzinfo=timezone(timedelta(seconds=7200))),
     ),
     ("datetime(inst)", datetime(2020, 5, 4, 13, 37), datetime(2020, 5, 4, 13, 37)),
 ]
 SUPPORTED_TYPES_DATA += [(n, v, e, datetime) for n, v, e in SUPPORTED_DATETIME]
 
+# date - can be parsed from ISO format
+SUPPORTED_DATE: Example3T = [
+    ("date(str)", "2020-05-04", date(2020, 5, 4)),
+    ("date(str-no-dashes)", "20200504" if PY_311 else "2020-05-04", date(2020, 5, 4)),
+    ("date(inst)", date(2020, 5, 4), date(2020, 5, 4)),
+]
+SUPPORTED_TYPES_DATA += [(n, v, e, date) for n, v, e in SUPPORTED_DATE]
+
+# timedelta - can be parsed from ISO and simpliefied string formats
+SUPPORTED_TIMEDELTA: Example3T = [
+    (f"timedelta({kind}-{example})", td_str, td)
+    for (td, example), examples in {
+        (timedelta(seconds=1), "s"): [
+            ("iso", "PT01S"),
+            ("simple-iso", "1s"),
+            ("simple", "1"),
+        ],
+        (timedelta(minutes=1, seconds=1), "ms"): [
+            ("iso", "PT01M01S"),
+            ("simple-iso", "1m1s"),
+            ("simple", "1:01"),
+        ],
+        (timedelta(hours=1, minutes=1, seconds=1), "hms"): [
+            ("iso", "PT01H01M01S"),
+            ("simple-iso", "1h1m1s"),
+            ("simple", "1:01:01"),
+        ],
+        (timedelta(days=1, hours=1, minutes=1, seconds=1), "dhms"): [
+            ("iso", "P01DT01H01M01S"),
+            ("simple-iso", "1d1h1m1s"),
+            ("simple", "1d,1:01:01"),
+        ],
+        (timedelta(days=1, seconds=1), "ds"): [
+            ("iso", "P1DT1S"),
+            ("simple-iso", "1d1s"),
+            ("simple", "1d1"),
+        ],
+        (timedelta(hours=1, seconds=1), "hs"): [
+            ("iso", "PT01H01S"),
+            ("simple-iso", "1h1s"),
+            ("simple", "1:0:01"),
+        ],
+        (timedelta(seconds=-(24 * 60 * 60 + 1)), "-ds"): [
+            ("iso", "-P01DT01S"),
+            ("simple-iso", "-1d1s"),
+            ("simple", "-1D00:00:01"),
+        ],
+        (timedelta(microseconds=1), "mic1"): [
+            ("iso", "PT0.000001S"),
+            ("simple-iso", "0.000001s"),
+            ("simple", "0.000001"),
+        ],
+        (timedelta(microseconds=100_000), "mic1hk"): [
+            ("iso", "PT0.1S"),
+            ("simple-iso", "0.1s"),
+            ("simple", "0.1"),
+        ],
+    }.items()
+    for kind, td_str in examples
+] + [
+    ("timedelta(float)", 1.0, timedelta(seconds=1)),
+    ("timedelta(inst)", timedelta(days=1, seconds=2), timedelta(days=1, seconds=2)),
+]
+SUPPORTED_TYPES_DATA += [(n, v, e, timedelta) for n, v, e in SUPPORTED_TIMEDELTA]
+
 # Enum - Enums are parsed from their "key"
 SUPPORTED_ENUM: Example3T = [
     ("enum(str)", "eggs", LeEnum.eggs),
     ("enum(inst)", LeEnum.eggs, LeEnum.eggs),
 ]
 SUPPORTED_TYPES_DATA += [(n, v, e, LeEnum) for n, v, e in SUPPORTED_ENUM]
 
@@ -516,50 +582,195 @@
     The list :data:`SUPPORTED_TYPES_DATA` is the officially source of truth.
 
     Please create an issue if something is missing here.
     """
     assert converter.structure(value, typ) == expected
 
 
-@pytest.mark.parametrize(
-    "converter",
-    [
-        pytest.param(converters.get_default_cattrs_converter, id="converter:cattrs"),
-        pytest.param(converters.get_default_ts_converter, id="converter:ts"),
-    ],
-)
-@pytest.mark.parametrize(
-    "value, expected", [pytest.param(v, e, id=n) for n, v, e in SUPPORTED_PATH]
-)
-@pytest.mark.parametrize("resolve_paths", [True, False])
-def test_resolve_path(
-    converter: Callable[[bool], converters.Converter],
-    value: Any,
-    expected: Any,
-    resolve_paths: bool,
-) -> None:
+class TestToTimedelta:
     """
-    The path-resolving behavior can be explicitly set.
+    Tests for "to_timedelta()".
     """
-    if not resolve_paths:
-        expected = expected.relative_to(Path.cwd())
-    c = converter(resolve_paths)
-    assert c.structure(value, Path) == expected
+
+    @given(
+        simple_fmt=strategies.booleans(),
+        left_pad=strategies.booleans(),
+        sign=strategies.sampled_from([None, "+", "-"]),
+        days=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        hours=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        minutes=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        seconds=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        micros=strategies.one_of(strategies.none(), strategies.integers(0, 999999)),
+    )
+    def test_from_iso_string(
+        self,
+        simple_fmt: bool,
+        left_pad: bool,
+        sign: Optional[str],
+        days: Optional[int],
+        hours: Optional[int],
+        minutes: Optional[int],
+        seconds: Optional[int],
+        micros: Optional[int],
+    ) -> None:
+        """
+        Timedeltas can be parsed from ISO strings and simplified ISO strings (missing
+        the "P" and the "T").
+
+        - P[nnD][T[nnH][nnM][nnS]]
+        - [nnD][nnH][nnM][nnS]
+
+        The regex is case-insensitive.  Numbers may be left-padded with 0 (e.g., "02")
+        and they can also be > 99.
+
+        All places (days, hours, minutes, seconds) are optional.
+        """
+        # Ditch examples where everything is None
+        assume(any(i is not None for i in [days, hours, minutes, seconds, micros]))
+
+        if micros is not None and not seconds:
+            seconds = 0
+
+        fmt = ">02d" if left_pad else "d"
+
+        # Strip trailing "0" from microseconds and make shure "x." -> "x.0"
+        micros_str = "" if micros is None else f".{micros:>06}".rstrip("0")
+        micros_str = ".0" if micros_str == "." else micros_str
+        time_str = "" if hours is None else f"{hours:{fmt}}H"
+        time_str += "" if minutes is None else f"{minutes:{fmt}}M"
+        time_str += "" if seconds is None else f"{seconds:{fmt}}{micros_str}S"
+        td_str = "" if sign is None else sign
+        td_str += "P"
+        td_str += "" if days is None else f"{days}D"
+        td_str += f"T{time_str}" if time_str else ""
+        if simple_fmt:
+            td_str = td_str.replace("P", "").replace("T", "").lower()
+
+        _kwargs = {
+            "days": days,
+            "hours": hours,
+            "minutes": minutes,
+            "seconds": seconds,
+            "microseconds": micros,
+        }
+        kwargs = {
+            k: (-v if sign == "-" else v) for k, v in _kwargs.items() if v is not None
+        }
+        assert converters.to_timedelta(td_str, timedelta) == timedelta(**kwargs), td_str
+
+    @given(
+        left_pad=strategies.booleans(),
+        sign=strategies.sampled_from([None, "+", "-"]),
+        comma=strategies.sampled_from(["", ","]),
+        days=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        hours=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        minutes=strategies.one_of(strategies.none(), strategies.integers(0, 9999)),
+        seconds=strategies.integers(0, 9999),
+        micros=strategies.one_of(strategies.none(), strategies.integers(0, 999999)),
+    )
+    def test_from_simple_string(
+        self,
+        left_pad: bool,
+        sign: Optional[str],
+        comma: str,
+        days: Optional[int],
+        hours: Optional[int],
+        minutes: Optional[int],
+        seconds: int,
+        micros: Optional[int],
+    ) -> None:
+        """
+        Timedeltas can be parsed a simple string format..
+
+        - [dD[,]][[hh:]mm:]ss[.ffffff]
+
+        Numbers may be left-padded with 0 (e.g., "02") and they can also be > 99.
+        """
+        if hours is not None and minutes is None:
+            minutes = 0
+        fmt = ">02d" if left_pad else "d"
+        micros_str = "" if micros is None else f".{micros:>06}".rstrip("0")
+        micros_str = ".0" if micros_str == "." else micros_str
+        td_str = f"{seconds:{fmt}}{micros_str}"
+        td_str = td_str if minutes is None else f"{minutes:{fmt}}:{td_str}"
+        td_str = td_str if hours is None else f"{hours:{fmt}}:{td_str}"
+        td_str = td_str if days is None else f"{days}D{comma}{td_str}"
+        td_str = td_str if sign is None else f"{sign}{td_str}"
+
+        _kwargs = {
+            "days": days,
+            "hours": hours,
+            "minutes": minutes,
+            "seconds": seconds,
+            "microseconds": micros,
+        }
+        kwargs = {
+            k: (-v if sign == "-" else v) for k, v in _kwargs.items() if v is not None
+        }
+        assert converters.to_timedelta(td_str, timedelta) == timedelta(**kwargs), td_str
+
+    @given(
+        positive=strategies.booleans(),
+        days=strategies.integers(0, 5),
+        hours=strategies.integers(0, 23),
+        minutes=strategies.integers(0, 59),
+        seconds=strategies.integers(0, 59),
+        micros=strategies.integers(0, 999999),
+    )
+    def test_timedelta_to_str(
+        self,
+        positive: bool,
+        days: int,
+        hours: int,
+        minutes: int,
+        seconds: int,
+        micros: int,
+    ) -> None:
+        """
+        Timedeltas can be converted back to a timedelta string (in simplified ISO
+        format).
+        """
+        td = timedelta(
+            days=days,
+            hours=hours,
+            minutes=minutes,
+            seconds=seconds,
+            microseconds=micros,
+        )
+        if not positive:
+            td = -td
+
+        micros_str = f".{micros:>06}".rstrip("0") if micros else ""
+        seconds_str = f"{seconds}{micros_str}s" if seconds or micros_str else ""
+        expected = ""
+        expected += f"{days}d" if days else ""
+        expected += f"{hours}h" if hours else ""
+        expected += f"{minutes}m" if minutes else ""
+        expected += seconds_str
+        if expected and not positive:
+            expected = f"-{expected}"
+
+        result = converters.timedelta_to_str(td)
+        assert result == expected
+        assert converters.to_timedelta(result, timedelta) == td
 
 
 @pytest.mark.parametrize(
     "cls, value",
     [
         # "to_bool()" is flexible, but does not accept anything
         (bool, ""),
         (bool, []),
         (bool, "spam"),
         (bool, 2),
         (bool, -1),
         (datetime, 3),
+        (date, 3),
+        (timedelta, datetime(1, 1, 1)),
+        (timedelta, "1s1h"),  # Not ordered properly
         # len(value) does not match len(tuple-args)
         (Tuple[int, int], (1,)),
         (Tuple[int, int], (1, 2, 3)),
         (Union[int, datetime, None], "3.1"),  # float is not part of the Union
         (Sequence, [0, 1]),  # Type not supported
         (AttrsCls, {"foo": 3}),  # Invalid attribute
         (AttrsCls, {"opt", "x"}),  # Invalid value
@@ -575,14 +786,40 @@
     "_core.convert()".
     """
     converter = converters.TSConverter()
     with pytest.raises((KeyError, TypeError, ValueError)):
         converter.structure(value, cls)
 
 
+@pytest.mark.parametrize(
+    "converter",
+    [
+        pytest.param(converters.get_default_cattrs_converter, id="converter:cattrs"),
+        pytest.param(converters.get_default_ts_converter, id="converter:ts"),
+    ],
+)
+@pytest.mark.parametrize(
+    "value, expected", [pytest.param(v, e, id=n) for n, v, e in SUPPORTED_PATH]
+)
+@pytest.mark.parametrize("resolve_paths", [True, False])
+def test_resolve_path(
+    converter: Callable[[bool], converters.Converter],
+    value: Any,
+    expected: Any,
+    resolve_paths: bool,
+) -> None:
+    """
+    The path-resolving behavior can be explicitly set.
+    """
+    if not resolve_paths:
+        expected = expected.relative_to(Path.cwd())
+    c = converter(resolve_paths)
+    assert c.structure(value, Path) == expected
+
+
 STRLIST_TEST_DATA = [
     (List[int], [1, 2, 3]),
     (Set[int], {1, 2, 3}),
     (FrozenSet[int], frozenset({1, 2, 3})),
     (Tuple[int, ...], (1, 2, 3)),
     (Tuple[int, int, int], (1, 2, 3)),
 ]
```

### Comparing `typed_settings-24.2.0/tests/test_core.py` & `typed_settings-24.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_dict_utils.py` & `typed_settings-24.3.0/tests/test_dict_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_file_utils.py` & `typed_settings-24.3.0/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_loaders.py` & `typed_settings-24.3.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_no_optionals.py` & `typed_settings-24.3.0/tests/test_no_optionals.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_onepassword.py` & `typed_settings-24.3.0/tests/test_onepassword.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,10 +102,10 @@
     assert result == "eggs"
 
 
 def test_get_resource_not_exists() -> None:
     """
     A ValueError with the "op" output is raised if a resource does not exist.
     """
-    msg = '"op" error: could not read secret xyz: invalid secret reference.*'
+    msg = "\"op\" error: could not read secret 'op://Test/x': invalid secret reference"
     with pytest.raises(ValueError, match=msg):
-        op.get_resource("xyz")
+        op.get_resource("op://Test/x")
```

### Comparing `typed_settings-24.2.0/tests/test_processors.py` & `typed_settings-24.3.0/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_readme.py` & `typed_settings-24.3.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/tests/test_types.py` & `typed_settings-24.3.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/LICENSE` & `typed_settings-24.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/README.md` & `typed_settings-24.3.0/README.md`

 * *Files identical despite different names*

### Comparing `typed_settings-24.2.0/pyproject.toml` & `typed_settings-24.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "typed-settings"
-version = "24.2.0"
+version = "24.3.0"
 description = "Typed settings based on attrs classes"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [
     { name = "Stefan Scherfke", email = "stefan@sofa-rockers.org" },
 ]
@@ -79,14 +79,15 @@
     "ruff",
     "mypy",
     "types-toml",
 ]
 test = [
     "typed-settings[all]",
     "coverage[toml]>=5.3",
+    "hypothesis",
     "pytest-cov",
     "pytest>=7.2.0",
     "rich-click>=1.6",
     "sybil>=6",
     "typing-extensions",
 ]
 dev = [  # Everything needed for development
@@ -108,38 +109,20 @@
     "/src",
     "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 
 [tool.hatch.envs.default]
+path = "./.venv"
 features = ["dev"]
 post-install-commands = [
     "pre-commit install --install-hooks",
 ]
-
-[tool.hatch.envs.default.scripts]
-test = "pytest {args:docs src tests}"
-cov = "pytest --cov --cov-config=pyproject.toml --cov-report=term-missing {args:docs src tests}"
-lint = [
-  "ruff .",
-  "mypy src/ tests/ ./noxfile.py",
-  "mypy docs/conf.py docs/conftest.py",
-  "mypy docs/examples",
-]
-fix = [
-  "ruff --fix-only {args:.}",
-  "black {args:.}",
-]
-docs = [
-  "make -C docs html",
-]
-clean-docs = [
-  "make -C docs clean html",
-]
+uv = true
 
 [tool.black]
 line-length = 88
 
 [tool.coverage.paths]
 source = [
     "src",
@@ -178,14 +161,19 @@
 module = "typed_settings.*"
 disallow_untyped_defs = true
 
 [tool.pytest.ini_options]
 addopts = "--ignore=README.md --ignore=docs/_build"
 
 [tool.ruff]
+line-length = 88
+src = ["src", "tests"]
+target-version = "py38"
+
+[tool.ruff.lint]
 select = [  # see: https://beta.ruff.rs/docs/rules/
     "F",  # pyflakes
     "E",  # pycodestyle error
     "W",  # pycodestyle warning
     "C90",  # mccabe
     "I",  # isort
     "D",  # pydocstyle
@@ -201,24 +189,21 @@
     "D107",  # I never document __init__()
     "D102",
     "D105",  # I don't always write docstrings for __ meths, esp. for __str__.
     "D200",  # Allow putting the """ in separate lines in one-line docstrings
     "D205",  # Allow the first line spanning another line.
     "D212",  # Allow putting the """ in separate lines in multi-line docstrings
 ]
-line-length = 88
-src = ["src", "tests"]
-target-version = "py38"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "docs/examples/*" = ["D100", "D101", "D103", "D415"]
 "examples/*" = ["D101"]
 "tests/*" = ["RUF012"]
 "tests/op" = ["D100"]
 "tests/test_cli_param_types.py" = ["D106"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-after-imports = 2
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 ignore-decorators = ["typing.overload"]
```

### Comparing `typed_settings-24.2.0/PKG-INFO` & `typed_settings-24.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: typed-settings
-Version: 24.2.0
+Version: 24.3.0
 Summary: Typed settings based on attrs classes
 Project-URL: Homepage, https://gitlab.com/sscherfke/typed-settings
 Project-URL: Documentation, https://typed-settings.readthedocs.io
 Project-URL: Changelog, https://typed-settings.readthedocs.io/en/latest/changelog.html
 Project-URL: Issues, https://gitlab.com/sscherfke/typed-settings/-/issues
 Project-URL: Source Code, https://gitlab.com/sscherfke/typed-settings
 Author-email: Stefan Scherfke <stefan@sofa-rockers.org>
@@ -25,52 +25,94 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: tomli>=2; python_version < '3.11'
 Provides-Extra: all
-Requires-Dist: typed-settings[attrs,cattrs,click,jinja,option-groups,pydantic]; extra == 'all'
+Requires-Dist: attrs>=23.1; extra == 'all'
+Requires-Dist: cattrs>=22.2; extra == 'all'
+Requires-Dist: click-option-group; extra == 'all'
+Requires-Dist: click>=7; extra == 'all'
+Requires-Dist: jinja2; extra == 'all'
+Requires-Dist: pydantic>=2; extra == 'all'
 Provides-Extra: attrs
 Requires-Dist: attrs>=23.1; extra == 'attrs'
 Provides-Extra: cattrs
 Requires-Dist: cattrs>=22.2; extra == 'cattrs'
 Provides-Extra: click
 Requires-Dist: click>=7; extra == 'click'
 Provides-Extra: dev
+Requires-Dist: attrs>=23.1; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: cattrs>=22.2; extra == 'dev'
+Requires-Dist: click-option-group; extra == 'dev'
+Requires-Dist: click>=7; extra == 'dev'
+Requires-Dist: coverage[toml]>=5.3; extra == 'dev'
+Requires-Dist: furo>=2023.9; extra == 'dev'
+Requires-Dist: hypothesis; extra == 'dev'
+Requires-Dist: jinja2; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: myst-parser>=2.0; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: pip-audit; extra == 'dev'
-Requires-Dist: typed-settings[docs,lint,test]; extra == 'dev'
+Requires-Dist: pydantic>=2; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: pytest>=7.2.0; extra == 'dev'
+Requires-Dist: rich-click>=1.6; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'dev'
+Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'dev'
+Requires-Dist: sphinx>=7.2; extra == 'dev'
+Requires-Dist: sybil>=6; extra == 'dev'
+Requires-Dist: types-toml; extra == 'dev'
+Requires-Dist: typing-extensions; extra == 'dev'
 Provides-Extra: docs
+Requires-Dist: attrs>=23.1; extra == 'docs'
+Requires-Dist: cattrs>=22.2; extra == 'docs'
+Requires-Dist: click-option-group; extra == 'docs'
+Requires-Dist: click>=7; extra == 'docs'
 Requires-Dist: furo>=2023.9; extra == 'docs'
+Requires-Dist: jinja2; extra == 'docs'
 Requires-Dist: myst-parser>=2.0; extra == 'docs'
+Requires-Dist: pydantic>=2; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
 Requires-Dist: sphinx>=7.2; extra == 'docs'
-Requires-Dist: typed-settings[all]; extra == 'docs'
 Provides-Extra: jinja
 Requires-Dist: jinja2; extra == 'jinja'
 Provides-Extra: lint
+Requires-Dist: attrs>=23.1; extra == 'lint'
 Requires-Dist: black; extra == 'lint'
+Requires-Dist: cattrs>=22.2; extra == 'lint'
+Requires-Dist: click-option-group; extra == 'lint'
+Requires-Dist: click>=7; extra == 'lint'
+Requires-Dist: jinja2; extra == 'lint'
 Requires-Dist: mypy; extra == 'lint'
+Requires-Dist: pydantic>=2; extra == 'lint'
 Requires-Dist: ruff; extra == 'lint'
-Requires-Dist: typed-settings[all]; extra == 'lint'
 Requires-Dist: types-toml; extra == 'lint'
 Provides-Extra: option-groups
 Requires-Dist: click-option-group; extra == 'option-groups'
 Requires-Dist: click>=7; extra == 'option-groups'
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2; extra == 'pydantic'
 Provides-Extra: test
+Requires-Dist: attrs>=23.1; extra == 'test'
+Requires-Dist: cattrs>=22.2; extra == 'test'
+Requires-Dist: click-option-group; extra == 'test'
+Requires-Dist: click>=7; extra == 'test'
 Requires-Dist: coverage[toml]>=5.3; extra == 'test'
+Requires-Dist: hypothesis; extra == 'test'
+Requires-Dist: jinja2; extra == 'test'
+Requires-Dist: pydantic>=2; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.2.0; extra == 'test'
 Requires-Dist: rich-click>=1.6; extra == 'test'
 Requires-Dist: sybil>=6; extra == 'test'
-Requires-Dist: typed-settings[all]; extra == 'test'
 Requires-Dist: typing-extensions; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Typed Settings
 
 Load and merge settings from multiple different sources and present them in a structured, typed, and validated way!
```


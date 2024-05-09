# Comparing `tmp/narwhals-0.8.5.tar.gz` & `tmp/narwhals-0.8.6.tar.gz`

## Comparing `narwhals-0.8.5.tar` & `narwhals-0.8.6.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.5/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.5/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.5/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.5/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.5/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.5/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/why.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/index.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/series.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.5/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/__init__.py
--rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/dependencies.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/dtypes.py
--rw-r--r--   0        0        0    35843 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/py.typed
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/typing.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    14909 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.5/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/group_by_test.py
--rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_common.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/cum_sum_test.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/diff_test.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/fill_null_test.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/over_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/str/head_test.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/frame/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/frame/pipe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.5/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.5/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.5/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.5/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.5/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.5/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.5/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.6/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.6/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/why.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/index.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/series.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/__init__.py
+-rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/dtypes.py
+-rw-r--r--   0        0        0    35843 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/py.typed
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/typing.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    14909 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/group_by_test.py
+-rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_common.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/over_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/frame/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/frame/pipe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.6/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.6/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.6/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.6/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.6/PKG-INFO
```

### Comparing `narwhals-0.8.5/.pre-commit-config.yaml` & `narwhals-0.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/CONTRIBUTING.md` & `narwhals-0.8.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/mkdocs.yml` & `narwhals-0.8.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/.github/workflows/extremes.yml` & `narwhals-0.8.6/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/.github/workflows/mkdocs.yml` & `narwhals-0.8.6/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.6/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/.github/workflows/pytest.yml` & `narwhals-0.8.6/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/extending.md` & `narwhals-0.8.6/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/generate_members.py` & `narwhals-0.8.6/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/index.md` & `narwhals-0.8.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/quick_start.md` & `narwhals-0.8.6/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/related.md` & `narwhals-0.8.6/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/roadmap.md` & `narwhals-0.8.6/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/why.md` & `narwhals-0.8.6/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/api-reference/index.md` & `narwhals-0.8.6/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/api-reference/series.md` & `narwhals-0.8.6/docs/api-reference/series.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/assets/image.png` & `narwhals-0.8.6/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/basics/column.md` & `narwhals-0.8.6/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/basics/complete_example.md` & `narwhals-0.8.6/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/basics/dataframe.md` & `narwhals-0.8.6/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/docs/other/pandas_index.md` & `narwhals-0.8.6/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/__init__.py` & `narwhals-0.8.6/narwhals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.5"
+__version__ = "0.8.6"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.5/narwhals/dataframe.py` & `narwhals-0.8.6/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/dependencies.py` & `narwhals-0.8.6/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/dtypes.py` & `narwhals-0.8.6/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/expression.py` & `narwhals-0.8.6/narwhals/expression.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/functions.py` & `narwhals-0.8.6/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/group_by.py` & `narwhals-0.8.6/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/series.py` & `narwhals-0.8.6/narwhals/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/translate.py` & `narwhals-0.8.6/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/typing.py` & `narwhals-0.8.6/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/utils.py` & `narwhals-0.8.6/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.6/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/expr.py` & `narwhals-0.8.6/narwhals/_pandas_like/expr.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.6/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.6/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/series.py` & `narwhals-0.8.6/narwhals/_pandas_like/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/typing.py` & `narwhals-0.8.6/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/narwhals/_pandas_like/utils.py` & `narwhals-0.8.6/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/conftest.py` & `narwhals-0.8.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/test_common.py` & `narwhals-0.8.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/test_dt.py` & `narwhals-0.8.6/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/test_group_by.py` & `narwhals-0.8.6/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/test_series.py` & `narwhals-0.8.6/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/test_str.py` & `narwhals-0.8.6/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/tpch_q1_test.py` & `narwhals-0.8.6/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/utils.py` & `narwhals-0.8.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/customer.parquet` & `narwhals-0.8.6/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/lineitem.parquet` & `narwhals-0.8.6/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/nation.parquet` & `narwhals-0.8.6/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/orders.parquet` & `narwhals-0.8.6/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/part.parquet` & `narwhals-0.8.6/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/partsupp.parquet` & `narwhals-0.8.6/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/region.parquet` & `narwhals-0.8.6/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/data/supplier.parquet` & `narwhals-0.8.6/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/expr/cum_sum_test.py` & `narwhals-0.8.6/tests/expr/cum_sum_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/expr/diff_test.py` & `narwhals-0.8.6/tests/expr/diff_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/expr/fill_null_test.py` & `narwhals-0.8.6/tests/expr/fill_null_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/expr/over_test.py` & `narwhals-0.8.6/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/expr/str/head_test.py` & `narwhals-0.8.6/tests/expr/str/head_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/expr/str/to_datetime_test.py` & `narwhals-0.8.6/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/frame/pipe_test.py` & `narwhals-0.8.6/tests/frame/pipe_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.6/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/hypothesis/test_concat.py` & `narwhals-0.8.6/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tests/hypothesis/test_join.py` & `narwhals-0.8.6/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/q1.py` & `narwhals-0.8.6/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/q2.py` & `narwhals-0.8.6/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/q3.py` & `narwhals-0.8.6/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/q4.py` & `narwhals-0.8.6/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/q5.py` & `narwhals-0.8.6/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.6/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/utils/bump_version.py` & `narwhals-0.8.6/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/utils/check_api_reference.py` & `narwhals-0.8.6/utils/check_api_reference.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/LICENSE.md` & `narwhals-0.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/README.md` & `narwhals-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.5/pyproject.toml` & `narwhals-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.5"
+version = "0.8.6"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.5/PKG-INFO` & `narwhals-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.5
+Version: 0.8.6
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


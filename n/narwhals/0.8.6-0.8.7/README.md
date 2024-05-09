# Comparing `tmp/narwhals-0.8.6.tar.gz` & `tmp/narwhals-0.8.7.tar.gz`

## Comparing `narwhals-0.8.6.tar` & `narwhals-0.8.7.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.6/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.6/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.6/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/why.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/index.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/series.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.6/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/__init__.py
--rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/dependencies.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/dtypes.py
--rw-r--r--   0        0        0    35843 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/py.typed
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/typing.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    14909 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 narwhals-0.8.6/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/group_by_test.py
--rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_common.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/cum_sum_test.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/diff_test.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/fill_null_test.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/over_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/str/head_test.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/frame/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/frame/pipe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.6/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.6/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.6/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.6/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.6/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.6/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.6/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.7/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.7/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/why.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/index.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/series.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/__init__.py
+-rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/dtypes.py
+-rw-r--r--   0        0        0    37580 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/py.typed
+-rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/typing.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    16348 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    14015 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/group_by_test.py
+-rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_common.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/over_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/frame/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/frame/pipe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.7/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.7/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.7/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.7/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.7/PKG-INFO
```

### Comparing `narwhals-0.8.6/.pre-commit-config.yaml` & `narwhals-0.8.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/CONTRIBUTING.md` & `narwhals-0.8.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/mkdocs.yml` & `narwhals-0.8.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.7/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/.github/workflows/extremes.yml` & `narwhals-0.8.7/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/.github/workflows/mkdocs.yml` & `narwhals-0.8.7/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/.github/workflows/pytest.yml` & `narwhals-0.8.7/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/extending.md` & `narwhals-0.8.7/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/generate_members.py` & `narwhals-0.8.7/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/index.md` & `narwhals-0.8.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/quick_start.md` & `narwhals-0.8.7/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/related.md` & `narwhals-0.8.7/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/roadmap.md` & `narwhals-0.8.7/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/why.md` & `narwhals-0.8.7/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/api-reference/index.md` & `narwhals-0.8.7/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/api-reference/series.md` & `narwhals-0.8.7/docs/api-reference/series.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/assets/image.png` & `narwhals-0.8.7/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/basics/column.md` & `narwhals-0.8.7/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/basics/complete_example.md` & `narwhals-0.8.7/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/basics/dataframe.md` & `narwhals-0.8.7/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/docs/other/pandas_index.md` & `narwhals-0.8.7/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/__init__.py` & `narwhals-0.8.7/narwhals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.6"
+__version__ = "0.8.7"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.6/narwhals/dataframe.py` & `narwhals-0.8.7/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/dependencies.py` & `narwhals-0.8.7/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/dtypes.py` & `narwhals-0.8.7/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/expression.py` & `narwhals-0.8.7/narwhals/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         Examples:
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> df_pd = pd.DataFrame({'a': [True, False], 'b': [True, True]})
             >>> df_pl = pl.DataFrame({'a': [True, False], 'b': [True, True]})
 
-            We define a data-frame agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
             ...     df = df.select(nw.col('a', 'b').any())
             ...     return nw.to_native(df)
 
             We can then pass either pandas or Polars to `func`:
@@ -899,15 +899,15 @@
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> data = {'lyrics': ['Atatata', 'taata', 'taatatata', 'zukkyun']}
             >>> df_pd = pd.DataFrame(data)
             >>> df_pl = pl.DataFrame(data)
 
-            We define a data-frame agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
             ...     df = df.with_columns(lyrics_head = nw.col('lyrics').str.head())
             ...     return nw.to_native(df)
 
             We can then pass either pandas or Polars to `func`:
@@ -957,15 +957,15 @@
         Examples:
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> df_pd = pd.DataFrame({'a': ['2020-01-01', '2020-01-02']})
             >>> df_pl = pl.DataFrame({'a': ['2020-01-01', '2020-01-02']})
 
-            We define a data-frame agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
             ...     df = df.select(nw.col('a').str.to_datetime(format='%Y-%m-%d'))
             ...     return nw.to_native(df)
 
             We can then pass either pandas or Polars to `func`:
@@ -993,14 +993,68 @@
 class ExprDateTimeNamespace:
     def __init__(self, expr: Expr) -> None:
         self._expr = expr
 
     def year(self) -> Expr:
         return self._expr.__class__(lambda plx: self._expr._call(plx).dt.year())
 
+    def month(self) -> Expr:
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.month())
+
+    def day(self) -> Expr:
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.day())
+
+    def hour(self) -> Expr:
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.hour())
+
+    def minute(self) -> Expr:
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.minute())
+
+    def second(self) -> Expr:
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.second())
+
+    def ordinal_day(self) -> Expr:
+        """
+        Get ordinal day.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> from datetime import datetime
+            >>> import narwhals as nw
+            >>> data = {'a': [datetime(2020, 1, 1), datetime(2020, 8, 3)]}
+            >>> df_pd = pd.DataFrame(data)
+            >>> df_pl = pl.DataFrame(data)
+
+            We define a dataframe-agnostic function:
+
+            >>> def func(df_any):
+            ...     df = nw.from_native(df_any)
+            ...     df = df.select(nw.col('a').dt.ordinal_day())
+            ...     return nw.to_native(df)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(df_pd)
+                 a
+            0    1
+            1  216
+            >>> func(df_pl)
+            shape: (2, 1)
+            ┌─────┐
+            │ a   │
+            │ --- │
+            │ i16 │
+            ╞═════╡
+            │ 1   │
+            │ 216 │
+            └─────┘
+        """
+        return self._expr.__class__(lambda plx: self._expr._call(plx).dt.ordinal_day())
+
 
 def col(*names: str | Iterable[str]) -> Expr:
     """
     Instantiate an expression, similar to `polars.col`.
     """
     return Expr(lambda plx: plx.col(*names))
```

### Comparing `narwhals-0.8.6/narwhals/functions.py` & `narwhals-0.8.7/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/group_by.py` & `narwhals-0.8.7/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/series.py` & `narwhals-0.8.7/narwhals/series.py`

 * *Files 20% similar despite different names*

```diff
@@ -107,55 +107,122 @@
     def all(self) -> Any:
         return self._series.all()
 
     def min(self) -> Any:
         return self._series.min()
 
     def max(self) -> Any:
+        """
+        Get the maximum value in this Series.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> s = [1, 2, 3]
+            >>> s_pd = pd.Series(s)
+            >>> s_pl = pl.Series(s)
+
+            We define a library agnostic function:
+
+            >>> def func(s_any):
+            ...     s = nw.from_native(s_any, series_only=True)
+            ...     return s.max()
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(s_pd)
+            3
+            >>> func(s_pl)
+            3
+        """
         return self._series.max()
 
     def sum(self) -> Any:
         return self._series.sum()
 
     def std(self, *, ddof: int = 1) -> Any:
         return self._series.std(ddof=ddof)
 
     def is_in(self, other: Any) -> Self:
         return self._from_series(self._series.is_in(self._extract_native(other)))
 
     def drop_nulls(self) -> Self:
+        """
+        Drop all null values.
+
+        See Also:
+          drop_nans
+
+        Notes:
+          A null value is not the same as a NaN value.
+          To drop NaN values, use :func:`drop_nans`.
+
+        Examples:
+          >>> import pandas as pd
+          >>> import polars as pl
+          >>> import numpy as np
+          >>> import narwhals as nw
+          >>> s_pd = pd.Series([2, 4, None, 3, 5])
+          >>> s_pl = pl.Series('a', [2, 4, None, 3, 5])
+
+          Now define a dataframe-agnostic function with a `column` argument for the column to evaluate :
+
+          >>> def func(s_any):
+          ...   s = nw.from_native(s_any, series_only=True)
+          ...   s = s.drop_nulls()
+          ...   return nw.to_native(s)
+
+          Then we can pass either Series (polars or pandas) to `func`:
+
+          >>> func(s_pd)
+          0    2.0
+          1    4.0
+          3    3.0
+          4    5.0
+          dtype: float64
+          >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
+          shape: (4,)
+          Series: 'a' [i64]
+          [
+             2
+             4
+             3
+             5
+          ]
+        """
         return self._from_series(self._series.drop_nulls())
 
     def cum_sum(self) -> Self:
         """
         Calculate the cumulative sum.
 
         Examples:
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> s = [2, 4, 3]
             >>> s_pd = pd.Series(s)
             >>> s_pl = pl.Series(s)
 
-            We define a data-frame agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(s_any):
             ...     s = nw.from_native(s_any, series_only=True)
             ...     s = s.cum_sum()
             ...     return nw.to_native(s)
 
             We can then pass either pandas or Polars to `func`:
 
             >>> func(s_pd)
             0    2
             1    6
             2    9
             dtype: int64
-            >>> func(s_pl)  # doctest:+SKIP
+            >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
             shape: (3,)
             Series: '' [i64]
             [
                2
                6
                9
             ]
@@ -184,29 +251,29 @@
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> s = [2, 4, 3]
             >>> s_pd = pd.Series(s)
             >>> s_pl = pl.Series(s)
 
-            We define a data-frame agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(s_any):
             ...     s = nw.from_native(s_any, series_only=True)
             ...     s = s.diff()
             ...     return nw.to_native(s)
 
             We can then pass either pandas or Polars to `func`:
 
             >>> func(s_pd)
             0    NaN
             1    2.0
             2   -1.0
             dtype: float64
-            >>> func(s_pl)  # doctest:+SKIP
+            >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
             shape: (3,)
             Series: '' [i64]
             [
                null
                2
                -1
             ]
@@ -304,31 +371,31 @@
             >>> import pandas as pd
             >>> import polars as pl
             >>> import narwhals as nw
             >>> lyrics = ['Atatata', 'taata', 'taatatata', 'zukkyun']
             >>> s_pd = pd.Series(lyrics)
             >>> s_pl = pl.Series(lyrics)
 
-            We define a data-frame agnostic function:
+            We define a dataframe-agnostic function:
 
             >>> def func(s_any):
             ...     s = nw.from_native(s_any, series_only=True)
             ...     s = s.str.head()
             ...     return nw.to_native(s)
 
             We can then pass either pandas or Polars to `func`:
 
             >>> func(s_pd)
             0    Atata
             1    taata
             2    taata
             3    zukky
             dtype: object
-            >>> func(s_pl)  # doctest: +SKIP
-            shape: (2,)
+            >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (4,)
             Series: '' [str]
             [
                "Atata"
                "taata"
                "taata"
                "zukky"
             ]
@@ -340,7 +407,58 @@
 
 class SeriesDateTimeNamespace:
     def __init__(self, series: Series) -> None:
         self._series = series
 
     def year(self) -> Series:
         return self._series.__class__(self._series._series.dt.year())
+
+    def month(self) -> Series:
+        return self._series.__class__(self._series._series.dt.month())
+
+    def day(self) -> Series:
+        return self._series.__class__(self._series._series.dt.day())
+
+    def hour(self) -> Series:
+        return self._series.__class__(self._series._series.dt.hour())
+
+    def minute(self) -> Series:
+        return self._series.__class__(self._series._series.dt.minute())
+
+    def second(self) -> Series:
+        return self._series.__class__(self._series._series.dt.second())
+
+    def ordinal_day(self) -> Series:
+        """
+        Get ordinal day.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> from datetime import datetime
+            >>> import narwhals as nw
+            >>> data = [datetime(2020, 1, 1), datetime(2020, 8, 3)]
+            >>> s_pd = pd.Series(data)
+            >>> s_pl = pl.Series(data)
+
+            We define a library agnostic function:
+
+            >>> def func(s_any):
+            ...     s = nw.from_native(s_any, series_only=True)
+            ...     s = s.dt.ordinal_day()
+            ...     return nw.to_native(s)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(s_pd)
+            0      1
+            1    216
+            dtype: int32
+            >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (2,)
+            Series: '' [i16]
+            [
+               1
+               216
+            ]
+        """
+        return self._series.__class__(self._series._series.dt.ordinal_day())
```

### Comparing `narwhals-0.8.6/narwhals/translate.py` & `narwhals-0.8.7/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/typing.py` & `narwhals-0.8.7/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/utils.py` & `narwhals-0.8.7/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.7/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/expr.py` & `narwhals-0.8.7/narwhals/_pandas_like/expr.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 
 from narwhals._pandas_like.series import PandasSeries
 from narwhals._pandas_like.utils import register_expression_call
-from narwhals._pandas_like.utils import to_datetime
+from narwhals._pandas_like.utils import register_namespace_expression_call
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from narwhals._pandas_like.dataframe import PandasDataFrame
 
 
@@ -260,73 +260,55 @@
 
 
 class PandasExprStringNamespace:
     def __init__(self, expr: PandasExpr) -> None:
         self._expr = expr
 
     def ends_with(self, suffix: str) -> PandasExpr:
-        # TODO make a register_expression_call for namespaces
-
-        return PandasExpr(
-            lambda df: [
-                PandasSeries(
-                    series._series.str.endswith(suffix),
-                    implementation=df._implementation,
-                )
-                for series in self._expr._call(df)
-            ],
-            depth=self._expr._depth + 1,
-            function_name=f"{self._expr._function_name}->str.ends_with",
-            root_names=self._expr._root_names,
-            output_names=self._expr._output_names,
-            implementation=self._expr._implementation,
+        return register_namespace_expression_call(
+            self._expr,
+            "str",
+            "ends_with",
+            suffix,
         )
 
     def head(self, n: int = 5) -> PandasExpr:
-        return PandasExpr(
-            lambda df: [series.str.head(n) for series in self._expr._call(df)],
-            depth=self._expr._depth + 1,
-            function_name=f"{self._expr._function_name}->str.head",
-            root_names=self._expr._root_names,
-            output_names=self._expr._output_names,
-            implementation=self._expr._implementation,
+        return register_namespace_expression_call(
+            self._expr,
+            "str",
+            "head",
+            n,
         )
 
     def to_datetime(self, format: str | None = None) -> PandasExpr:  # noqa: A002
-        # TODO make a register_expression_call for namespaces
-        return PandasExpr(
-            lambda df: [
-                PandasSeries(
-                    to_datetime(df._implementation)(series._series, format=format),
-                    implementation=df._implementation,
-                )
-                for series in self._expr._call(df)
-            ],
-            depth=self._expr._depth + 1,
-            function_name=f"{self._expr._function_name}->str.to_datetime",
-            root_names=self._expr._root_names,
-            output_names=self._expr._output_names,
-            implementation=self._expr._implementation,
+        return register_namespace_expression_call(
+            self._expr,
+            "str",
+            "to_datetime",
+            format,
         )
 
 
 class PandasExprDateTimeNamespace:
     def __init__(self, expr: PandasExpr) -> None:
         self._expr = expr
 
     def year(self) -> PandasExpr:
-        # TODO make a register_expression_call for namespaces
+        return register_namespace_expression_call(self._expr, "dt", "year")
 
-        return PandasExpr(
-            lambda df: [
-                PandasSeries(
-                    series._series.dt.year,
-                    implementation=df._implementation,
-                )
-                for series in self._expr._call(df)
-            ],
-            depth=self._expr._depth + 1,
-            function_name=f"{self._expr._function_name}->dt.year",
-            root_names=self._expr._root_names,
-            output_names=self._expr._output_names,
-            implementation=self._expr._implementation,
-        )
+    def month(self) -> PandasExpr:
+        return register_namespace_expression_call(self._expr, "dt", "month")
+
+    def day(self) -> PandasExpr:
+        return register_namespace_expression_call(self._expr, "dt", "day")
+
+    def hour(self) -> PandasExpr:
+        return register_namespace_expression_call(self._expr, "dt", "hour")
+
+    def minute(self) -> PandasExpr:
+        return register_namespace_expression_call(self._expr, "dt", "minute")
+
+    def second(self) -> PandasExpr:
+        return register_namespace_expression_call(self._expr, "dt", "second")
+
+    def ordinal_day(self) -> PandasExpr:
+        return register_namespace_expression_call(self._expr, "dt", "ordinal_day")
```

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.7/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.7/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/series.py` & `narwhals-0.8.7/narwhals/_pandas_like/series.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Sequence
 
 from narwhals._pandas_like.utils import item
 from narwhals._pandas_like.utils import reverse_translate_dtype
+from narwhals._pandas_like.utils import to_datetime
 from narwhals._pandas_like.utils import translate_dtype
 from narwhals._pandas_like.utils import validate_column_comparand
 from narwhals.utils import parse_version
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
@@ -433,16 +434,58 @@
         )
 
     def head(self, n: int = 5) -> PandasSeries:
         return self._series._from_series(
             self._series._series.str[:n],
         )
 
+    def to_datetime(self, format: str | None = None) -> PandasSeries:  # noqa: A002
+        return self._series._from_series(
+            to_datetime(self._series._implementation)(self._series._series, format=format)
+        )
+
 
 class PandasSeriesDateTimeNamespace:
     def __init__(self, series: PandasSeries) -> None:
         self._series = series
 
     def year(self) -> PandasSeries:
         return self._series._from_series(
             self._series._series.dt.year,
         )
+
+    def month(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.month,
+        )
+
+    def day(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.day,
+        )
+
+    def hour(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.hour,
+        )
+
+    def minute(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.minute,
+        )
+
+    def second(self) -> PandasSeries:
+        return self._series._from_series(
+            self._series._series.dt.second,
+        )
+
+    def ordinal_day(self) -> PandasSeries:
+        ser = self._series._series
+        year_start = ser.dt.year
+        result = (
+            ser.to_numpy().astype("datetime64[D]")
+            - (year_start.to_numpy() - 1970).astype("datetime64[Y]")
+        ).astype("int32") + 1
+        dtype = "Int64[pyarrow]" if "pyarrow" in str(ser.dtype) else "int32"
+        return self._series._from_series(
+            self._series._series.__class__(result, dtype=dtype, name=year_start.name)
+        )
```

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/typing.py` & `narwhals-0.8.7/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/narwhals/_pandas_like/utils.py` & `narwhals-0.8.7/narwhals/_pandas_like/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -186,14 +186,32 @@
         depth=expr._depth + 1,
         function_name=f"{expr._function_name}->{attr}",
         root_names=root_names,
         output_names=expr._output_names,
     )
 
 
+def register_namespace_expression_call(
+    expr: ExprT, namespace: str, attr: str, *args: Any, **kwargs: Any
+) -> PandasExpr:
+    from narwhals._pandas_like.expr import PandasExpr
+
+    return PandasExpr(
+        lambda df: [
+            getattr(getattr(series, namespace), attr)(*args, **kwargs)
+            for series in expr._call(df)
+        ],
+        depth=expr._depth + 1,
+        function_name=f"{expr._function_name}->{namespace}.{attr}",
+        root_names=expr._root_names,
+        output_names=expr._output_names,
+        implementation=expr._implementation,
+    )
+
+
 def item(s: Any) -> Any:
     # cuDF doesn't have Series.item().
     if len(s) != 1:
         msg = "Can only convert a Series of length 1 to a scalar"  # pragma: no cover
         raise AssertionError(msg)
     return s.iloc[0]
```

### Comparing `narwhals-0.8.6/tests/conftest.py` & `narwhals-0.8.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/test_common.py` & `narwhals-0.8.7/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/test_group_by.py` & `narwhals-0.8.7/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/test_series.py` & `narwhals-0.8.7/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/test_str.py` & `narwhals-0.8.7/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/tpch_q1_test.py` & `narwhals-0.8.7/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/utils.py` & `narwhals-0.8.7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/customer.parquet` & `narwhals-0.8.7/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/lineitem.parquet` & `narwhals-0.8.7/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/nation.parquet` & `narwhals-0.8.7/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/orders.parquet` & `narwhals-0.8.7/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/part.parquet` & `narwhals-0.8.7/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/partsupp.parquet` & `narwhals-0.8.7/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/region.parquet` & `narwhals-0.8.7/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/data/supplier.parquet` & `narwhals-0.8.7/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/expr/cum_sum_test.py` & `narwhals-0.8.7/tests/expr/cum_sum_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/expr/diff_test.py` & `narwhals-0.8.7/tests/expr/diff_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/expr/fill_null_test.py` & `narwhals-0.8.7/tests/expr/fill_null_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/expr/over_test.py` & `narwhals-0.8.7/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/expr/str/head_test.py` & `narwhals-0.8.7/tests/expr/str/head_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/expr/str/to_datetime_test.py` & `narwhals-0.8.7/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/frame/pipe_test.py` & `narwhals-0.8.7/tests/frame/pipe_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.7/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/hypothesis/test_concat.py` & `narwhals-0.8.7/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tests/hypothesis/test_join.py` & `narwhals-0.8.7/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/q1.py` & `narwhals-0.8.7/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/q2.py` & `narwhals-0.8.7/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/q3.py` & `narwhals-0.8.7/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/q4.py` & `narwhals-0.8.7/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/q5.py` & `narwhals-0.8.7/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.7/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/utils/bump_version.py` & `narwhals-0.8.7/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/utils/check_api_reference.py` & `narwhals-0.8.7/utils/check_api_reference.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/LICENSE.md` & `narwhals-0.8.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/README.md` & `narwhals-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.6/pyproject.toml` & `narwhals-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.6"
+version = "0.8.7"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.6/PKG-INFO` & `narwhals-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.6
+Version: 0.8.7
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


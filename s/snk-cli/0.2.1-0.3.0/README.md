# Comparing `tmp/snk_cli-0.2.1.tar.gz` & `tmp/snk_cli-0.3.0.tar.gz`

## Comparing `snk_cli-0.2.1.tar` & `snk_cli-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snk_cli-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk_cli-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 snk_cli-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/index.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/cli.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/config.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/dynamic_typer.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/options.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/subcommands.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/testing.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/utils.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/validate.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/workflow.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/__about__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/__init__.py
--rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/cli.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/conda.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/dynamic_typer.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/testing.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/utils.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/validate.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/workflow.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/config/__init__.py
--rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/config/config.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/config/utils.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/options/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/options/option.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/options/utils.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/config.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/env.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/profile.py
--rw-r--r--   0        0        0    18481 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/run.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/script.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_conda_env.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_dynamic_typer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/cov.fasta
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/Snakefile
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/cli.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/config.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/snk.yaml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/cli.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/config.yaml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/snk.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/resources/data.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/things/__about__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/Snakefile
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/envs/python.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/profiles/slurm/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/scripts/hello.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_dynamic_options.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_run.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_snk_config.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_subcommands.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_validate.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_workflow_cli.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snk_cli-0.2.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk_cli-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 snk_cli-0.2.1/README.md
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 snk_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 snk_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snk_cli-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk_cli-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 snk_cli-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/cli.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/config.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/dynamic_typer.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/options.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/subcommands.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/testing.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/utils.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/validate.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.3.0/docs/reference/workflow.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/__about__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/__init__.py
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/cli.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/conda.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/dynamic_typer.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/testing.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/utils.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/validate.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/workflow.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/config/__init__.py
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/config/config.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/config/utils.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/options/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/options/option.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/options/utils.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/subcommands/__init__.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/subcommands/config.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/subcommands/env.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/subcommands/profile.py
+-rw-r--r--   0        0        0    18481 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/subcommands/run.py
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 snk_cli-0.3.0/src/snk_cli/subcommands/script.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_conda_env.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_dynamic_typer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/cov.fasta
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/print_config/Snakefile
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/print_config/cli.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/print_config/config.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/print_config/snk.yaml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/cli.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/config.yaml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/snk.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/resources/data.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/things/__about__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/workflow/Snakefile
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/workflow/envs/wget.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/workflow/profiles/slurm/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/data/workflow/workflow/scripts/hello.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/test_dynamic_options.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/test_run.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/test_snk_config.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/test_subcommands.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/test_validate.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 snk_cli-0.3.0/tests/test_cli/test_workflow_cli.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snk_cli-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk_cli-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 snk_cli-0.3.0/README.md
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 snk_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 snk_cli-0.3.0/PKG-INFO
```

### Comparing `snk_cli-0.2.1/mkdocs.yml` & `snk_cli-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/.github/workflows/publish.yml` & `snk_cli-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/.github/workflows/tests.yml` & `snk_cli-0.3.0/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,28 @@
       - main
 permissions:
   contents: write
 jobs:
   test:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: "conda-incubator/setup-miniconda@v2"
         with:
           python-version: 3.11
           auto-activate-base: false
           miniforge-variant: Mambaforge
           channels: conda-forge,bioconda,defaults
           channel-priority: strict
           auto-update-conda: true
+      - uses: actions/setup-python@v5
+        with:
+          python-version: '3.11' 
       - uses: actions/cache@v2
         with:
           key: ${{ github.ref }}
           path: .cache
       - run: pip install hatch
       - run: sudo apt-get update && sudo apt-get install -y llvm
       - run: sudo apt-get -y install graphviz
```

### Comparing `snk_cli-0.2.1/src/snk_cli/cli.py` & `snk_cli-0.3.0/src/snk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/conda.py` & `snk_cli-0.3.0/src/snk_cli/conda.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/dynamic_typer.py` & `snk_cli-0.3.0/src/snk_cli/dynamic_typer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 
 
 class DynamicTyper:
     app: typer.Typer
 
     def __init__(self):
-        self.app = typer.Typer()
+        self.app = typer.Typer(add_completion=False)
 
     def __call__(self):
         """
         Invoke the CLI.
 
         Side Effects:
           Invokes the CLI.
@@ -29,15 +29,15 @@
         """
         Set the app attribute.
 
         Side Effects:
           Sets the app attribute to a Typer object.
         """
         if not hasattr(self, "app"):
-          self.app = typer.Typer()
+          self.app = typer.Typer(add_completion=False)
 
     def register_default_command(self, command: Callable, **command_kwargs) -> None:
         """
         Register a default command to the CLI.
 
         Args:
           command (Callable): The command to register.
```

### Comparing `snk_cli-0.2.1/src/snk_cli/testing.py` & `snk_cli-0.3.0/src/snk_cli/testing.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/utils.py` & `snk_cli-0.3.0/src/snk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/validate.py` & `snk_cli-0.3.0/src/snk_cli/validate.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/workflow.py` & `snk_cli-0.3.0/src/snk_cli/workflow.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/config/config.py` & `snk_cli-0.3.0/src/snk_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/config/utils.py` & `snk_cli-0.3.0/src/snk_cli/config/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/options/utils.py` & `snk_cli-0.3.0/src/snk_cli/options/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/subcommands/config.py` & `snk_cli-0.3.0/src/snk_cli/subcommands/config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/subcommands/env.py` & `snk_cli-0.3.0/src/snk_cli/subcommands/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             # address relative to cwd
             address = Path(conda.address)
             if address.exists():
                 address = str(address) if verbose else f"[green]{address.name}[/green]"
                 cmd = f"{self.workflow.name} env activate {env.stem}"
             else:
                 address = ""
-                cmd = f"{self.workflow.name} env show {env.stem}"
+                cmd = f"{self.workflow.name} env create {env.stem}"
             table.add_row(
                 env.stem, cmd, address
             )
         console = Console()
         console.print(table)
 
     def _get_conda_env_path(self, name: str) -> Path:
@@ -149,15 +149,15 @@
         if force or input(f"Delete {path}? [y/N] ").lower() == "y":
             shutil.rmtree(path)
             self.success(f"Deleted {path}!")
 
     def create(
             self, 
             names: Optional[List[str]] = typer.Argument(None, help="The names of the environments to create. If not provided, all environments will be created."),
-            max_workers: int = typer.Option(get_num_cores(), "--workers", "-w", help="Max number of envs to create in parallel.")
+            max_workers: int = typer.Option(1, "--workers", "-w", help="Max number of envs to create in parallel.")
         ):
         if names:
             env_paths = [self._get_conda_env_path(name) for name in names]
         else:
             env_paths = self.workflow.environments
         env_args = [
             (
```

### Comparing `snk_cli-0.2.1/src/snk_cli/subcommands/profile.py` & `snk_cli-0.3.0/src/snk_cli/subcommands/profile.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/subcommands/run.py` & `snk_cli-0.3.0/src/snk_cli/subcommands/run.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/src/snk_cli/subcommands/script.py` & `snk_cli-0.3.0/src/snk_cli/subcommands/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             verbose: bool = typer.Option(False, "--verbose", "-v", help="Show script as paths."), 
         ):
         from rich.console import Console
         from rich.table import Table
         table = Table("Name", "CMD", "File", show_header=True, show_lines=True)
         for script in self.workflow.scripts:
             # address relative to cwd
-            table.add_row(script.stem, f"{self.workflow.name} script show {script.stem}", str(script.resolve()) if verbose else script.name)
+            table.add_row(script.stem, f"{self.workflow.name} script run {script.stem} --env ...", str(script.resolve()) if verbose else script.name)
         console = Console()
         console.print(table)
 
     def _get_script_path(self, name: str) -> Path:
         script = [e for e in self.workflow.scripts if e.name == name or e.stem == name]
         if not script:
             self.error(f"Script {name} not found!")
```

### Comparing `snk_cli-0.2.1/tests/test_dynamic_typer.py` & `snk_cli-0.3.0/tests/test_dynamic_typer.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/utils.py` & `snk_cli-0.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/data/artic_v4.1.bed` & `snk_cli-0.3.0/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/data/config.yaml` & `snk_cli-0.3.0/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/data/cov.fasta` & `snk_cli-0.3.0/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/data/workflow/snk.yaml` & `snk_cli-0.3.0/tests/data/workflow/snk.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/data/workflow/workflow/Snakefile` & `snk_cli-0.3.0/tests/data/workflow/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/data/workflow/workflow/envs/python.yml` & `snk_cli-0.3.0/tests/data/workflow/workflow/envs/wget.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,5 +1,5 @@
 channels:                                                                                                                                                                   
   - bioconda                                                                                                                                                                
   - conda-forge                                                                                                                                                             
 dependencies:                                                                                                                                                               
-  - python=3.9
+  - wget
```

### Comparing `snk_cli-0.2.1/tests/data/workflow/workflow/profiles/slurm/config.yaml` & `snk_cli-0.3.0/tests/data/workflow/workflow/profiles/slurm/config.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/test_cli/test_dynamic_options.py` & `snk_cli-0.3.0/tests/test_cli/test_dynamic_options.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/test_cli/test_run.py` & `snk_cli-0.3.0/tests/test_cli/test_run.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/test_cli/test_snk_config.py` & `snk_cli-0.3.0/tests/test_cli/test_snk_config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/test_cli/test_subcommands.py` & `snk_cli-0.3.0/tests/test_cli/test_subcommands.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 @pytest.mark.parametrize("cmd,expected_in_stdout,expected_in_stderr", [
     (["script", "run", "hello.py"], ["hello world"], []),
     (["script", "list"], ["hello.py"], []),
     (["script", "show", "hello.py"], ["print('hello world')"], []),
     (["profile", "list"], ["slurm"], []),
     (["profile", "show", "slurm"], ["cluster"], []),
-    (["env", "list"], ["python"], []),
-    (["env", "show", "python"], ["python"], []),
+    (["env", "list"], ["wget"], []),
+    (["env", "show", "wget"], ["wget"], []),
     (["env", "create"], ["All conda environments created!"], []),
-    (["env", "create", "python"], ["Created environment python!"], []),
-    (["env", "run", "python", "which python"], ["bin/python"], []),
-    (["env", "activate", "python"], [], ["Activating python environment...", "Exiting python environment..."]),
+    (["env", "create", "wget"], ["Created environment wget!"], []),
+    (["env", "run", "wget", "which wget"], [".conda"], []),
+    (["env", "activate", "wget"], [], ["Activating wget environment...", "Exiting wget environment..."]),
     (["env", "remove", "-f"], ["Deleted"], []),
     (["info"], ["name", "version", "snakefile", "conda_prefix_dir", "singularity_prefix_dir", "workflow_dir_path"], []),
 ])
 def test_snk_cli_command(capfd, local_runner, cmd, expected_in_stdout, expected_in_stderr):
     res = local_runner(cmd)
     captured = capfd.readouterr()  # Capture stdout and stderr of subprocess e.g. env and script commands
     assert res.exit_code == 0, res.stderr
```

### Comparing `snk_cli-0.2.1/tests/test_cli/test_validate.py` & `snk_cli-0.3.0/tests/test_cli/test_validate.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/tests/test_cli/test_workflow_cli.py` & `snk_cli-0.3.0/tests/test_cli/test_workflow_cli.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/LICENSE.txt` & `snk_cli-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/README.md` & `snk_cli-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/pyproject.toml` & `snk_cli-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.1/PKG-INFO` & `snk_cli-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snk-cli
-Version: 0.2.1
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/unknown/snk-cli#readme
 Project-URL: Issues, https://github.com/unknown/snk-cli/issues
 Project-URL: Source, https://github.com/unknown/snk-cli
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/argufy-0.1.2b3.tar.gz` & `tmp/argufy-0.1.2b4.tar.gz`

## Comparing `argufy-0.1.2b3.tar` & `argufy-0.1.2b4.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.docstr.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.flake8
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 argufy-0.1.2b3/mkdocs.yml
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.github/workflows/docs.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/commands.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/docstrings.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/getting-started.md
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/index.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/roadmap.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/subcommands.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/type-hints.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/development/argument.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/development/parser.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/bool.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/complete.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/group.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/kwargs.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/simple.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/__main__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/cmd1.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/cmd2.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/__main__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/cmd.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/config.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/__init__.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/__main__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/cmd1.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/cmd2.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/config.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/parents/parents.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/__main__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/cmd1.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/cmd2.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/config.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/__init__.py
--rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/argument.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/exceptions.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/formatter.py
--rw-r--r--   0        0        0    19275 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/py.typed
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/test_argument_type_hints.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/test_version.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/commands/command_parser.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/commands/test_command_parser.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/docstrings/test_google.py
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/docstrings/test_numpy.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/docstrings/test_restructured.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/subcommands/subcommands_parser.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/subcommands/test_subcommands_parser.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 argufy-0.1.2b3/LICENSE
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 argufy-0.1.2b3/README.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 argufy-0.1.2b3/pyproject.toml
--rw-r--r--   0        0        0    17162 2020-02-02 00:00:00.000000 argufy-0.1.2b3/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 argufy-0.1.2b4/.docstr.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 argufy-0.1.2b4/.flake8
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 argufy-0.1.2b4/CODEOWNERS
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 argufy-0.1.2b4/mkdocs.yml
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 argufy-0.1.2b4/versioning.tar.gz
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 argufy-0.1.2b4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 argufy-0.1.2b4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/commands.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/docstrings.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/getting-started.md
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/index.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/roadmap.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/subcommands.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/type-hints.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/development/argument.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 argufy-0.1.2b4/docs/development/parser.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/bool.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/complete.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/group.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/kwargs.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/simple.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/commands/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/commands/__main__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/commands/cmd1.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/commands/cmd2.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/dataclass/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/dataclass/__main__.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/dataclass/cmd.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/dataclass/config.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/multiparse/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/multiparse/__main__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/multiparse/cmd1.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/multiparse/cmd2.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/multiparse/config.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/parents/parents.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/subcommands/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/subcommands/__main__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/subcommands/cmd1.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/subcommands/cmd2.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 argufy-0.1.2b4/examples/subcommands/config.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 argufy-0.1.2b4/src/argufy/__init__.py
+-rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 argufy-0.1.2b4/src/argufy/argument.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 argufy-0.1.2b4/src/argufy/exceptions.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 argufy-0.1.2b4/src/argufy/formatter.py
+-rw-r--r--   0        0        0    19275 2020-02-02 00:00:00.000000 argufy-0.1.2b4/src/argufy/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b4/src/argufy/py.typed
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/test_argument_type_hints.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/test_version.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/commands/command_parser.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/commands/test_command_parser.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/docstrings/test_google.py
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/docstrings/test_numpy.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/docstrings/test_restructured.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/subcommands/subcommands_parser.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 argufy-0.1.2b4/tests/subcommands/test_subcommands_parser.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 argufy-0.1.2b4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 argufy-0.1.2b4/LICENSE
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 argufy-0.1.2b4/README.md
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 argufy-0.1.2b4/pyproject.toml
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 argufy-0.1.2b4/PKG-INFO
```

### Comparing `argufy-0.1.2b3/mkdocs.yml` & `argufy-0.1.2b4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/.github/workflows/ci.yml` & `argufy-0.1.2b4/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ---
 name: CI Build
 on:
   push:
-    # branches: [main]
-    paths:
-      - 'src/**/*.py'
+    branches: [main]
+    # paths:
+    #   - 'src/**/*.py'
   pull_request:
     branches: [main]
 jobs:
   sca:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: 'Set up Python 3.11'
         uses: actions/setup-python@v5
         with:
           python-version: '3.11'
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install .[dev]
+          pip install '.[dev]'
       - name: Lint
         run: |
           isort --check-only **/*.py
           black --check **/*.py
           pylint src
       - name: Type checking
         run: mypy src
@@ -44,15 +44,15 @@
       - name: Setup gitconfig
         run: |
           git config user.name 'autonomous-bot'
           git config user.email 'an.autonomous.bot@gmail.com'
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install .[build]
+          pip install '.[build]'
       - name: Bump version
         run: |
           version info
           if [ "${GITHUB_REF##*/}" == "main" ]; then
             version bump --commit --tag
             version push --password "${{ secrets.GITHUB_TOKEN }}"
           else
@@ -104,15 +104,15 @@
     needs: build
     strategy:
       matrix:
         python-version:
           - '3.7'
           - '3.8'
           - '3.9'
-          - '3.11'
+          - '3.10'
           - '3.11'
           - '3.12'
     steps:
       - uses: actions/checkout@v4
         with:
           ref: "${{ github.event.pull_request.head.sha }}"
           fetch-depth: 0
@@ -126,15 +126,15 @@
         uses: actions/download-artifact@v4
         with:
           name: dist
           path: dist
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install .[dev]
+          pip install '.[dev]'
           pip install ./dist/*whl
       - name: Perform tests
         run: pytest --cov=argufy --cov-report=xml tests
   publish:
     if: github.ref == 'refs/heads/main'
     runs-on: ubuntu-latest
     needs: ['build', 'test']
```

### Comparing `argufy-0.1.2b3/.github/workflows/docs.yml` & `argufy-0.1.2b4/.github/workflows/docs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -13,38 +13,50 @@
       - name: 'Set up Python 3.11'
         uses: actions/setup-python@v5
         with:
           python-version: '3.11'
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install .[docs]
+          pip install '.[docs]'
       - name: Lint documentation
-        run: |
-          pydocstyle **/*.py --verbose
-          docstr-coverage **/*.py
+        run: pydocstyle **/*.py --verbose
   build:
     runs-on: ubuntu-latest
     needs: lint
     steps:
       - uses: actions/checkout@v4
       - name: 'Set up Python 3.11'
         uses: actions/setup-python@v5
         with:
           python-version: '3.11'
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install .[docs]
+          pip install '.[docs]'
       - name: Perform documentation tests
         run: mkdocs build
   test:
     runs-on: ubuntu-latest
+    needs: build
     steps:
       - uses: actions/checkout@v4
       - name: 'Set up Python 3.11'
         uses: actions/setup-python@v5
         with:
           python-version: '3.11'
-      - name: Lint documentation
-        run: |
-          python -m doctest README.md
+      - name: Test readme examples
+        run: python -m doctest README.md
+      - name: Check documentation coverage
+        run: docstr-coverage **/*.py
+  publish:
+    if: github.ref == 'refs/heads/main'
+    runs-on: ubuntu-latest
+    needs: test
+    steps:
+      - uses: actions/checkout@v4
+      - name: 'Set up Python 3.11'
+        uses: actions/setup-python@v5
+        with:
+          python-version: '3.11'
+      - name: Publish documentation
+        run: mkdocs gh-deploy
```

### Comparing `argufy-0.1.2b3/docs/commands.md` & `argufy-0.1.2b4/docs/commands.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/docs/getting-started.md` & `argufy-0.1.2b4/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/docs/index.md` & `argufy-0.1.2b4/docs/index.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/docs/roadmap.md` & `argufy-0.1.2b4/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/bool.py` & `argufy-0.1.2b4/examples/bool.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/complete.py` & `argufy-0.1.2b4/examples/complete.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/group.py` & `argufy-0.1.2b4/examples/group.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/kwargs.py` & `argufy-0.1.2b4/examples/kwargs.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/simple.py` & `argufy-0.1.2b4/examples/simple.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/commands/cmd1.py` & `argufy-0.1.2b4/examples/commands/cmd1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
 """Test parser.
 
 Attributes
 ----------
 example_variable: str
```

### Comparing `argufy-0.1.2b3/examples/commands/cmd2.py` & `argufy-0.1.2b4/examples/commands/cmd2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
 """Test parser.
 
 Attributes
 ----------
 example_variable: str
```

### Comparing `argufy-0.1.2b3/examples/dataclass/cmd.py` & `argufy-0.1.2b4/examples/dataclass/cmd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
 """Test parser.
 
 Attributes
 ----------
 variable: str
```

### Comparing `argufy-0.1.2b3/examples/multiparse/__main__.py` & `argufy-0.1.2b4/examples/multiparse/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
 """Provide CLI for example."""
 
 import sys
 
 from argufy import Parser
```

### Comparing `argufy-0.1.2b3/examples/multiparse/cmd1.py` & `argufy-0.1.2b4/examples/subcommands/cmd2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,38 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
-"""Test parser.
+"""Test parser two.
 
 Attributes
 ----------
 example_variable: str
     Example variable for testing
 
 """
 
-import json  # noqa
-from typing import Optional
+from typing import List, Tuple
 
-example_variable = 'ex_var'
-optional_variable: Optional[str] = None
+example_variable2 = 'test2'
 
 
-def print_variable() -> None:
-    """Print example variable."""
-    print('example_varible', example_variable)
-    print('optional_varible', optional_variable)
-
-
-def example_bool(bool_check: bool = False) -> None:
+def example_list(list_check: List[str]) -> None:
     """Demonstrate example bool.
 
     Parameters
     ----------
-    bool_check: bool, optional
+    list_check: list, optional
         example boolean
 
     """
-    print(bool_check)
+    print(list_check or [])
 
 
-def example_choice(choice_check: str = 'A') -> None:
+def example_tuple(tuple_check: Tuple[str, ...] = ('A', 'B', 'C')) -> None:
     """Demonstrate example choice.
 
     Parameters
     ----------
-    choice_check: str, {'A', 'B', 'C'}
+    tuple_check: tuple, ('A', 'B', 'C')
         example choice
 
     """
-    print(choice_check)
+    print(tuple_check)
```

### Comparing `argufy-0.1.2b3/examples/multiparse/cmd2.py` & `argufy-0.1.2b4/examples/multiparse/cmd2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
 """Test parser."""
 
 from . import builder
 
 _settings = builder()
```

### Comparing `argufy-0.1.2b3/examples/parents/parents.py` & `argufy-0.1.2b4/examples/parents/parents.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/examples/subcommands/cmd1.py` & `argufy-0.1.2b4/examples/subcommands/cmd1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
 """Test parser one.
 
 Attributes
 ----------
 example_variable1: str
```

### Comparing `argufy-0.1.2b3/examples/subcommands/cmd2.py` & `argufy-0.1.2b4/examples/multiparse/cmd1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-# -*- coding: utf-8 -*-
 # :copyright: (c) 2020 by Jesse Johnson.
 # :license: Apache 2.0, see LICENSE for more details.
-"""Test parser two.
+"""Test parser.
 
 Attributes
 ----------
 example_variable: str
     Example variable for testing
 
 """
 
-from typing import List, Tuple
+from typing import Optional
 
-example_variable2 = 'test2'
+example_variable = 'ex_var'
+optional_variable: Optional[str] = None
 
 
-def example_list(list_check: List[str] = []) -> None:
+def print_variable() -> None:
+    """Print example variable."""
+    print('example_varible', example_variable)
+    print('optional_varible', optional_variable)
+
+
+def example_bool(bool_check: bool = False) -> None:
     """Demonstrate example bool.
 
     Parameters
     ----------
-    list_check: list, optional
+    bool_check: bool, optional
         example boolean
 
     """
-    print(list_check)
+    print(bool_check)
 
 
-def example_tuple(tuple_check: Tuple[str, ...] = ('A', 'B', 'C')) -> None:
+def example_choice(choice_check: str = 'A') -> None:
     """Demonstrate example choice.
 
     Parameters
     ----------
-    tuple_check: tuple, ('A', 'B', 'C')
+    choice_check: str, {'A', 'B', 'C'}
         example choice
 
     """
-    print(tuple_check)
+    print(choice_check)
```

### Comparing `argufy-0.1.2b3/src/argufy/__init__.py` & `argufy-0.1.2b4/src/argufy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 from argufy.formatter import ArgufyHelpFormatter  # noqa
 from argufy.parser import Parser  # noqa
 
 __author__ = 'Jesse P. Johnson'
 __author_email__ = 'jpj6652@gmail.com'
 __title__ = 'argufy'
 __description__ = 'Inspection based parser built on argparse.'
-__version__ = '0.1.2b3'
+__version__ = '0.1.2b4'
 __license__ = 'Apache-2.0'
 __copyright__ = 'Copyright 2020 Jesse Johnson.'
 __all__: List[str] = ['Argument', 'ArgufyHelpFormatter', 'Parser']
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `argufy-0.1.2b3/src/argufy/argument.py` & `argufy-0.1.2b4/src/argufy/argument.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/src/argufy/formatter.py` & `argufy-0.1.2b4/src/argufy/formatter.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/src/argufy/parser.py` & `argufy-0.1.2b4/src/argufy/parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/test_argument_type_hints.py` & `argufy-0.1.2b4/tests/test_argument_type_hints.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/commands/command_parser.py` & `argufy-0.1.2b4/tests/commands/command_parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/commands/test_command_parser.py` & `argufy-0.1.2b4/tests/commands/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/docstrings/test_google.py` & `argufy-0.1.2b4/tests/docstrings/test_google.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/docstrings/test_numpy.py` & `argufy-0.1.2b4/tests/docstrings/test_numpy.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/docstrings/test_restructured.py` & `argufy-0.1.2b4/tests/docstrings/test_restructured.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/subcommands/subcommands_parser.py` & `argufy-0.1.2b4/tests/subcommands/subcommands_parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/tests/subcommands/test_subcommands_parser.py` & `argufy-0.1.2b4/tests/subcommands/test_subcommands_parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/.gitignore` & `argufy-0.1.2b4/.gitignore`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/LICENSE` & `argufy-0.1.2b4/LICENSE`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b3/README.md` & `argufy-0.1.2b4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # python-argufy
 
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Build Status](https://travis-ci.org/kuwv/python-argufy.svg?branch=master)](https://travis-ci.org/kuwv/python-argufy)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![build](https://github.com/kuwv/python-argufy/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kuwv/python-argufy/actions/workflows/ci.yml?branch=main)
 [![codecov](https://codecov.io/gh/kuwv/python-argufy/branch/master/graph/badge.svg)](https://codecov.io/gh/kuwv/python-argufy)
 
 ## Overview
 
 Inspection based parser built on argparse. Build complex CLI interfaces by
 writing more code-complete applications.
 
@@ -16,39 +16,17 @@
 without drawbacks. This parser easilly allows a CLI to be created with minimal
 effort while enabling inspection.
 
 ## Install
 
 `pip install argufy`
 
-## Create a parser
+## Create CLI module with a command and an argument.
 
 ```
-from argufy import Parser
-from . import cli
-
-def main():
-    """Do main function for CLI."""
-    parser = Parser()
-    parser.add_commands(cli)
-    parser.dispatch()
-
-if __name__ == '__main__':
-    main()
-```
-
-## Create the command line subcommands and arguments.
-
-```
-"""Example module named CLI."""
-
-def _ignored():
-    """This function is ignored."""
-    pass
-
 def example(argument: bool = False):
     """Provide an example command.
 
     Parameters
     ----------
     argument: bool, optional
         Provide an example argument.
@@ -56,14 +34,30 @@
     """
     if argument:
         print('This is a true argument')
     else:
         print('This is a false argument')
 ```
 
+## Create a parser
+
+```
+from argufy import Parser
+from . import cli
+
+def main():
+    """Do main function for CLI."""
+    parser = Parser()
+    parser.add_commands(cli)
+    parser.dispatch()
+
+if __name__ == '__main__':
+    main()
+```
+
 ## Example help message.
 
 ```
 $ command --help
 usage: command [-h] {example} ...
 
 positional arguments:
```

### Comparing `argufy-0.1.2b3/pyproject.toml` & `argufy-0.1.2b4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "argufy"
-version = "0.1.2b3"
+version = "0.1.2b4"
 description = "Inspection based parser based on argparse."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["parser"]
 requires-python = ">=3.6.2"
 authors = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
 maintainers = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `argufy-0.1.2b3/PKG-INFO` & `argufy-0.1.2b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: argufy
-Version: 0.1.2b3
+Version: 0.1.2b4
 Summary: Inspection based parser based on argparse.
 Project-URL: homepage, https://github.com/kuwv/python-argufy
 Project-URL: repository, https://github.com/kuwv/python-argufy
 Project-URL: documentation, https://kuwv.github.io/python-argufy/
 Author-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 Maintainer-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 License:                                  Apache License
@@ -206,20 +206,19 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 License-File: LICENSE
 Keywords: parser
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -248,16 +247,16 @@
 Requires-Dist: mkdocs>=1.2.2; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.16.2; extra == 'docs'
 Requires-Dist: pydocstyle[toml]>=6.1.1; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # python-argufy
 
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Build Status](https://travis-ci.org/kuwv/python-argufy.svg?branch=master)](https://travis-ci.org/kuwv/python-argufy)
+[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![build](https://github.com/kuwv/python-argufy/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/kuwv/python-argufy/actions/workflows/ci.yml?branch=main)
 [![codecov](https://codecov.io/gh/kuwv/python-argufy/branch/master/graph/badge.svg)](https://codecov.io/gh/kuwv/python-argufy)
 
 ## Overview
 
 Inspection based parser built on argparse. Build complex CLI interfaces by
 writing more code-complete applications.
 
@@ -268,39 +267,17 @@
 without drawbacks. This parser easilly allows a CLI to be created with minimal
 effort while enabling inspection.
 
 ## Install
 
 `pip install argufy`
 
-## Create a parser
+## Create CLI module with a command and an argument.
 
 ```
-from argufy import Parser
-from . import cli
-
-def main():
-    """Do main function for CLI."""
-    parser = Parser()
-    parser.add_commands(cli)
-    parser.dispatch()
-
-if __name__ == '__main__':
-    main()
-```
-
-## Create the command line subcommands and arguments.
-
-```
-"""Example module named CLI."""
-
-def _ignored():
-    """This function is ignored."""
-    pass
-
 def example(argument: bool = False):
     """Provide an example command.
 
     Parameters
     ----------
     argument: bool, optional
         Provide an example argument.
@@ -308,14 +285,30 @@
     """
     if argument:
         print('This is a true argument')
     else:
         print('This is a false argument')
 ```
 
+## Create a parser
+
+```
+from argufy import Parser
+from . import cli
+
+def main():
+    """Do main function for CLI."""
+    parser = Parser()
+    parser.add_commands(cli)
+    parser.dispatch()
+
+if __name__ == '__main__':
+    main()
+```
+
 ## Example help message.
 
 ```
 $ command --help
 usage: command [-h] {example} ...
 
 positional arguments:
```


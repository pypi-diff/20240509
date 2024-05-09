# Comparing `tmp/xwrf-0.0.3.tar.gz` & `tmp/xwrf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xwrf-0.0.3.tar", last modified: Fri Mar 15 15:46:18 2024, max compression
+gzip compressed data, was "xwrf-0.0.4.tar", last modified: Thu May  9 12:50:52 2024, max compression
```

## Comparing `xwrf-0.0.3.tar` & `xwrf-0.0.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.121595 xwrf-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.109595 xwrf-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.109595 xwrf-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/workflows/pypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-15 15:46:04.000000 xwrf-0.0.3/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-15 15:46:04.000000 xwrf-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-15 15:46:04.000000 xwrf-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-15 15:46:04.000000 xwrf-0.0.3/.prettierrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-15 15:46:04.000000 xwrf-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-15 15:46:04.000000 xwrf-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-03-15 15:46:04.000000 xwrf-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-15 15:46:04.000000 xwrf-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-15 15:46:18.121595 xwrf-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-15 15:46:04.000000 xwrf-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-15 15:46:04.000000 xwrf-0.0.3/ci/environment-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-15 15:46:04.000000 xwrf-0.0.3/ci/environment-upstream-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-15 15:46:04.000000 xwrf-0.0.3/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-15 15:46:04.000000 xwrf-0.0.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/_static/custom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/_static/xwrf_favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/_static/xwrf_logo_bg_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/_static/xwrf_logo_bg_light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/source/branding/
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/branding/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/source/explanation/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/explanation/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/source/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/how-to/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/how-to/install-xwrf.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/how-to/load-wrf-data.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.113595 xwrf-0.0.3/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/reference/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.117596 xwrf-0.0.3/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/tutorials/Overview.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/tutorials/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/tutorials/metpy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-15 15:46:04.000000 xwrf-0.0.3/docs/source/tutorials/xgcm.md
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-15 15:46:04.000000 xwrf-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 15:46:04.000000 xwrf-0.0.3/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-15 15:46:04.000000 xwrf-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-15 15:46:18.121595 xwrf-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-15 15:46:04.000000 xwrf-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.117596 xwrf-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_destagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_metpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_udunits.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-15 15:46:04.000000 xwrf-0.0.3/tests/test_version_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.117596 xwrf-0.0.3/xwrf/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/destagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/unit_harmonization_map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-15 15:46:04.000000 xwrf-0.0.3/xwrf/version_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:46:18.121595 xwrf-0.0.3/xwrf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-03-15 15:46:18.000000 xwrf-0.0.3/xwrf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-15 15:46:18.000000 xwrf-0.0.3/xwrf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:46:18.000000 xwrf-0.0.3/xwrf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:46:17.000000 xwrf-0.0.3/xwrf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-15 15:46:18.000000 xwrf-0.0.3/xwrf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 15:46:18.000000 xwrf-0.0.3/xwrf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.384934 xwrf-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.376934 xwrf-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.376934 xwrf-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.376934 xwrf-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-09 12:50:38.000000 xwrf-0.0.4/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-09 12:50:38.000000 xwrf-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-09 12:50:38.000000 xwrf-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 12:50:38.000000 xwrf-0.0.4/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 12:50:38.000000 xwrf-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 12:50:38.000000 xwrf-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-09 12:50:38.000000 xwrf-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 12:50:38.000000 xwrf-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-09 12:50:52.384934 xwrf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-09 12:50:38.000000 xwrf-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.376934 xwrf-0.0.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:50:38.000000 xwrf-0.0.4/ci/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 12:50:38.000000 xwrf-0.0.4/ci/environment-upstream-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-09 12:50:38.000000 xwrf-0.0.4/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 12:50:38.000000 xwrf-0.0.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.376934 xwrf-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.376934 xwrf-0.0.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/_static/custom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/_static/xwrf_favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/_static/xwrf_logo_bg_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/_static/xwrf_logo_bg_light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/docs/source/branding/
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/branding/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/docs/source/explanation/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/explanation/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/docs/source/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/how-to/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/how-to/install-xwrf.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/how-to/load-wrf-data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/reference/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/tutorials/Overview.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/tutorials/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/tutorials/metpy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-09 12:50:38.000000 xwrf-0.0.4/docs/source/tutorials/xgcm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 12:50:38.000000 xwrf-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 12:50:38.000000 xwrf-0.0.4/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 12:50:38.000000 xwrf-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 12:50:52.384934 xwrf-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-09 12:50:38.000000 xwrf-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.380934 xwrf-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_destagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_metpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_udunits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 12:50:38.000000 xwrf-0.0.4/tests/test_version_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.384934 xwrf-0.0.4/xwrf/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/destagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/unit_harmonization_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-09 12:50:38.000000 xwrf-0.0.4/xwrf/version_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:50:52.384934 xwrf-0.0.4/xwrf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-09 12:50:52.000000 xwrf-0.0.4/xwrf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-09 12:50:52.000000 xwrf-0.0.4/xwrf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:50:52.000000 xwrf-0.0.4/xwrf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:50:52.000000 xwrf-0.0.4/xwrf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 12:50:52.000000 xwrf-0.0.4/xwrf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 12:50:52.000000 xwrf-0.0.4/xwrf.egg-info/top_level.txt
```

### Comparing `xwrf-0.0.3/.github/ISSUE_TEMPLATE/bugreport.yml` & `xwrf-0.0.4/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/.github/ISSUE_TEMPLATE/newfeature.yml` & `xwrf-0.0.4/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/.github/pull_request_template.md` & `xwrf-0.0.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/.github/workflows/ci.yaml` & `xwrf-0.0.4/.github/workflows/ci.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,14 @@
 
       - name: Run Tests
         id: test
         run: |
           python -m pytest
 
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.3.1
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `xwrf-0.0.3/.github/workflows/pypi-release.yaml` & `xwrf-0.0.4/.github/workflows/pypi-release.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -74,12 +74,12 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.12
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
           verbose: true
```

### Comparing `xwrf-0.0.3/.github/workflows/upstream-dev-ci.yaml` & `xwrf-0.0.4/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/.gitignore` & `xwrf-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/.pre-commit-config.yaml` & `xwrf-0.0.4/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 ci:
   autoupdate_schedule: monthly
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: double-quote-string-fixer
       - id: debug-statements
       - id: mixed-line-ending
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args:
           - "--py38-plus"
 
   - repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.4.2
     hooks:
       - id: black
       - id: black-jupyter
 
   - repo: https://github.com/keewis/blackdoc
     rev: v0.3.9
     hooks:
```

### Comparing `xwrf-0.0.3/LICENSE` & `xwrf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/PKG-INFO` & `xwrf-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xwrf
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight interface for working with the Weather Research and Forecasting (WRF) model output in Xarray.
 Home-page: https://xwrf.readthedocs.io
 Maintainer: xWRF Developers
 License: Apache 2.0
 Project-URL: Documentation, https://xwrf.readthedocs.io
 Project-URL: Source, https://github.com/xarray-contrib/xwrf
 Project-URL: Tracker, https://github.com/xarray-contrib/xwrf/issues
```

### Comparing `xwrf-0.0.3/README.md` & `xwrf-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/Makefile` & `xwrf-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/make.bat` & `xwrf-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/_static/custom.js` & `xwrf-0.0.4/docs/source/_static/custom.js`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/_static/xwrf_favicon.ico` & `xwrf-0.0.4/docs/source/_static/xwrf_favicon.ico`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/_static/xwrf_logo_bg_dark.svg` & `xwrf-0.0.4/docs/source/_static/xwrf_logo_bg_dark.svg`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/_static/xwrf_logo_bg_light.svg` & `xwrf-0.0.4/docs/source/_static/xwrf_logo_bg_light.svg`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/branding/index.md` & `xwrf-0.0.4/docs/source/branding/index.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/conf.py` & `xwrf-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/how-to/install-xwrf.md` & `xwrf-0.0.4/docs/source/how-to/install-xwrf.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/how-to/load-wrf-data.md` & `xwrf-0.0.4/docs/source/how-to/load-wrf-data.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/index.md` & `xwrf-0.0.4/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/reference/api.md` & `xwrf-0.0.4/docs/source/reference/api.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/tutorials/Overview.md` & `xwrf-0.0.4/docs/source/tutorials/Overview.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/tutorials/metpy.md` & `xwrf-0.0.4/docs/source/tutorials/metpy.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/docs/source/tutorials/xgcm.md` & `xwrf-0.0.4/docs/source/tutorials/xgcm.md`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/setup.py` & `xwrf-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/tests/__init__.py` & `xwrf-0.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/tests/test_accessors.py` & `xwrf-0.0.4/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/tests/test_destagger.py` & `xwrf-0.0.4/tests/test_destagger.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/tests/test_grid.py` & `xwrf-0.0.4/tests/test_grid.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,20 @@
     )
     np.testing.assert_array_almost_equal(grid_params['west_east'], dummy_salem['west_east'].values)
 
     # Projection CRS
     assert grid_params['crs'] == pyproj.CRS(dummy_salem['Q2'].attrs['pyproj_srs'])
 
 
+def test_raise_notimplemented_error(dummy_dataset):
+    dummy_dataset.attrs['MAP_PROJ'] = 'invalid'
+    with pytest.raises(NotImplementedError):
+        _wrf_grid_from_dataset(dummy_dataset)
+
+
 @pytest.mark.parametrize(
     'test_grid, cf_grid_mapping_name',
     [
         ('polar_stereographic_1', 'polar_stereographic'),
         ('polar_stereographic_2', 'polar_stereographic'),
         ('lambert_conformal', 'lambert_conformal_conic'),
         ('mercator', 'mercator'),
@@ -76,7 +82,19 @@
         elif '_' not in varname and varname + '_M' in test_grid.data_vars:
             np.testing.assert_array_almost_equal(
                 recalculated_values,
                 test_grid[varname + '_M'].values[0],
                 decimal=2,
                 err_msg=f"Computed {varname + '_M'} does not match with raw output",
             )
+
+
+@pytest.mark.parametrize(
+    'test_grid',
+    [
+        'ideal',
+    ],
+    indirect=True,
+)
+def test_ideal_grid(test_grid):
+    grid_params = _wrf_grid_from_dataset(test_grid)
+    assert grid_params['crs'] is None
```

### Comparing `xwrf-0.0.3/tests/test_metpy.py` & `xwrf-0.0.4/tests/test_metpy.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/tests/test_postprocess.py` & `xwrf-0.0.4/tests/test_postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     assert dataset['south_north'].attrs['axis'] == 'Y'
     assert dataset['west_east'].attrs['axis'] == 'X'
     assert isinstance(dataset['wrf_projection'].item(), pyproj.CRS)
     assert dataset['Q2'].attrs['grid_mapping'] == 'wrf_projection'
 
 
 @pytest.mark.parametrize(
-    'sample_dataset', set(xwrf.tutorial.sample_datasets.keys()) - {'tiny'}, indirect=True
+    'sample_dataset', set(xwrf.tutorial.sample_datasets.keys()) - {'tiny', 'ideal'}, indirect=True
 )
 def test_grid_mapping_is_in_all_vars(sample_dataset):
     dataset = xwrf.postprocess._include_projection_coordinates(sample_dataset)
     horizontal_dims = set(xwrf.config.get('horizontal_dims')).intersection(set(dataset.dims))
     for var in dataset.data_vars:
         if any(dim in dataset[var].dims for dim in horizontal_dims):
             assert dataset[var].attrs['grid_mapping'] == 'wrf_projection'
@@ -117,14 +117,32 @@
     indirect=['sample_dataset_with_kwargs'],
 )
 def test_xtime_handling(sample_dataset_with_kwargs, xtime_dtype):
     dataset = xwrf.postprocess._decode_times(sample_dataset_with_kwargs)
     assert np.issubdtype(dataset.XTIME.dtype, xtime_dtype)
 
 
+@pytest.mark.parametrize(
+    'sample_dataset_with_kwargs,xtime_dtype',
+    [
+        (('wrfout', {'decode_times': True}), np.datetime64),
+        pytest.param(
+            ('wrfout', {'decode_times': False}),
+            np.datetime64,
+            marks=pytest.mark.xfail(raises=ValueError, strict=True),
+        ),
+    ],
+    indirect=['sample_dataset_with_kwargs'],
+)
+def test_xtime_fallback(sample_dataset_with_kwargs, xtime_dtype):
+    dataset_fallback = xwrf.postprocess._decode_times(sample_dataset_with_kwargs.drop_vars('Times'))
+    dataset = xwrf.postprocess._decode_times(sample_dataset_with_kwargs)
+    assert dataset_fallback.Time.equals(dataset.Time)
+
+
 @pytest.mark.parametrize('sample_dataset', ['lambert_conformal'], indirect=True)
 def test_assign_coord_to_dim_of_different_name(sample_dataset):
     dataset = sample_dataset.pipe(xwrf.postprocess._collapse_time_dim).pipe(
         xwrf.postprocess._assign_coord_to_dim_of_different_name
     )
     assert 'ZNU' not in dataset.dims
     assert 'ZNW' not in dataset.dims
```

### Comparing `xwrf-0.0.3/tests/test_tutorial.py` & `xwrf-0.0.4/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/tests/test_udunits.py` & `xwrf-0.0.4/tests/test_udunits.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/xwrf/accessors.py` & `xwrf-0.0.4/xwrf/accessors.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/xwrf/config.yaml` & `xwrf-0.0.4/xwrf/config.yaml`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/xwrf/destagger.py` & `xwrf-0.0.4/xwrf/destagger.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/xwrf/grid.py` & `xwrf-0.0.4/xwrf/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,18 @@
         'lat_1': ds.TRUELAT1,
         'lat_2': getattr(ds, 'TRUELAT2', ds.TRUELAT1),
         'lat_0': ds.MOAD_CEN_LAT,
         'lon_0': ds.STAND_LON,
         'center_lon': cen_lon,
     }
 
-    if proj_id == 1:
+    if proj_id == 0:
+        # Idealized Run, Cartesian grid
+        pass
+    elif proj_id == 1:
         # Lambert
         pargs['proj'] = 'lcc'
         del pargs['center_lon']
     elif proj_id == 2:
         # Polar stereo
         pargs['proj'] = 'stere'
         pargs['lat_ts'] = pargs['lat_1']
@@ -53,22 +56,28 @@
         pargs['proj'] = 'merc'
         pargs['lat_ts'] = pargs['lat_1']
         pargs['lon_0'] = pargs['center_lon']
         del pargs['lat_0'], pargs['lat_1'], pargs['lat_2'], pargs['center_lon']
     else:
         raise NotImplementedError(f'WRF proj not implemented yet: {proj_id}')
 
-    # Construct the pyproj CRS (letting errors fail through)
-    crs = pyproj.CRS(pargs)
+    if proj_id == 0:
+        # As this is an idealized run, there is no physical CRS
+        crs = None
+        e, n = cen_lon, cen_lat
+    else:
+        # Construct the pyproj CRS (letting errors fail through)
+        crs = pyproj.CRS(pargs)
+
+        # Get grid specifications
+        trf = pyproj.Transformer.from_crs(wgs84, crs, always_xy=True)
+        e, n = trf.transform(cen_lon, cen_lat)
 
-    # Get grid specifications
-    trf = pyproj.Transformer.from_crs(wgs84, crs, always_xy=True)
     nx = ds.sizes['west_east']
     ny = ds.sizes['south_north']
-    e, n = trf.transform(cen_lon, cen_lat)
     x0 = -(nx - 1) / 2.0 * dx + e  # DL corner
     y0 = -(ny - 1) / 2.0 * dy + n  # DL corner
 
     return {
         'crs': crs,
         'south_north': y0 + np.arange(ny) * dy,
         'west_east': x0 + np.arange(nx) * dx,
```

### Comparing `xwrf-0.0.3/xwrf/postprocess.py` & `xwrf-0.0.4/xwrf/postprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,32 @@
 from .grid import _wrf_grid_from_dataset
 
 
 def _decode_times(ds: xr.Dataset) -> xr.Dataset:
     """
     Decode the time variable to datetime64.
     """
-    try:
-        _time = pd.to_datetime(
-            ds.Times.data.astype('str'), errors='raise', format='%Y-%m-%d_%H:%M:%S'
-        )
-    except ValueError:
-        _time = pd.to_datetime(
-            ds.Times.data.astype('str'), errors='raise', format='%Y-%m-%dT%H:%M:%S'
-        )
+    if 'Times' in ds:
+        try:
+            _time = pd.to_datetime(
+                ds.Times.data.astype('str'), errors='raise', format='%Y-%m-%d_%H:%M:%S'
+            )
+        except ValueError:
+            _time = pd.to_datetime(
+                ds.Times.data.astype('str'), errors='raise', format='%Y-%m-%dT%H:%M:%S'
+            )
+    elif 'XTIME' in ds:
+        if ds.XTIME.dtype == 'datetime64[ns]':
+            _time = ds.XTIME.data
+        else:
+            raise ValueError(
+                'XTIME is not in datetime64 format, please use `xr.open_dataset(..., decode_times=True)`.'
+            )
+    else:
+        raise ValueError('No time variable found in the dataset.')
     ds = ds.assign_coords({'Time': _time})
     ds.Time.attrs = {'long_name': 'Time', 'standard_name': 'time'}
     return ds
 
 
 def _make_units_pint_friendly(ds: xr.Dataset) -> xr.Dataset:
     """
@@ -101,19 +111,20 @@
         return ds
     horizontal_dims = set(config.get('horizontal_dims')).intersection(set(ds.dims))
 
     # Include dimension coordinates
     for dim in horizontal_dims:
         ds[dim] = (dim, grid_components[dim], config.get(f'cf_attribute_map.{dim}'))
 
-    # Include CRS
-    ds['wrf_projection'] = (tuple(), grid_components['crs'], grid_components['crs'].to_cf())
-    for varname in ds.data_vars:
-        if any(dim in ds[varname].dims for dim in horizontal_dims):
-            ds[varname].attrs['grid_mapping'] = 'wrf_projection'
+    # Include CRS if we don't have idealized coords
+    if grid_components['crs'] is not None:
+        ds['wrf_projection'] = (tuple(), grid_components['crs'], grid_components['crs'].to_cf())
+        for varname in ds.data_vars:
+            if any(dim in ds[varname].dims for dim in horizontal_dims):
+                ds[varname].attrs['grid_mapping'] = 'wrf_projection'
 
     return ds
 
 
 def _assign_coord_to_dim_of_different_name(ds: xr.Dataset) -> xr.Dataset:
     for varname, dim in config.get('assign_coord_to_dim_map').items():
         try:
```

### Comparing `xwrf-0.0.3/xwrf/tutorial.py` & `xwrf-0.0.4/xwrf/tutorial.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     'polar_stereographic_1': 'data/geo_em_d01_polarstereo.nc',
     'polar_stereographic_2': 'data/geo_em_d02_polarstereo.nc',
     'lambert_conformal': 'data/lambert_conformal_sample.nc',
     'mercator': 'data/mercator_sample.nc',
     'tiny': 'data/tiny.nc',
     'met_em_sample': 'data/met_em.d01.2005-08-28_12:00:00.nc',
     'wrfout': 'data/wrfout_d01_2099-10-01_00:00:00.nc',
+    'ideal': 'data/ideal.nc',
 }
 
 
 # idea borrowed from Seaborn and Xarray
 def open_dataset(
     name: str,
     cache: bool = True,
@@ -61,14 +62,15 @@
     * ``"dummy_salem_parsed"``
     * ``"polar_stereographic_1"``
     * ``"polar_stereographic_2"``
     * ``"lambert_conformal"``
     * ``"mercator"``
     * ``"met_em_sample"``
     * ``"wrfout"``
+    * ``"ideal"``
 
     Parameters
     ----------
     name : str
         Name of the dataset.
         e.g. 'mercator'
     cache : bool, optional
```

### Comparing `xwrf-0.0.3/xwrf/unit_harmonization_map.yaml` & `xwrf-0.0.4/xwrf/unit_harmonization_map.yaml`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/xwrf/version_report.py` & `xwrf-0.0.4/xwrf/version_report.py`

 * *Files identical despite different names*

### Comparing `xwrf-0.0.3/xwrf.egg-info/PKG-INFO` & `xwrf-0.0.4/xwrf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xwrf
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight interface for working with the Weather Research and Forecasting (WRF) model output in Xarray.
 Home-page: https://xwrf.readthedocs.io
 Maintainer: xWRF Developers
 License: Apache 2.0
 Project-URL: Documentation, https://xwrf.readthedocs.io
 Project-URL: Source, https://github.com/xarray-contrib/xwrf
 Project-URL: Tracker, https://github.com/xarray-contrib/xwrf/issues
```

### Comparing `xwrf-0.0.3/xwrf.egg-info/SOURCES.txt` & `xwrf-0.0.4/xwrf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


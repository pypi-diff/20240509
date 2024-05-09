# Comparing `tmp/nexgen-0.9.1.tar.gz` & `tmp/nexgen-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexgen-0.9.1.tar", last modified: Mon Apr 22 16:39:35 2024, max compression
+gzip compressed data, was "nexgen-0.9.2.tar", last modified: Thu May  9 14:47:21 2024, max compression
```

## Comparing `nexgen-0.9.1.tar` & `nexgen-0.9.2.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.659085 nexgen-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-22 16:39:32.000000 nexgen-0.9.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 16:39:32.000000 nexgen-0.9.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-22 16:39:32.000000 nexgen-0.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.643085 nexgen-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.639085 nexgen-0.9.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.643085 nexgen-0.9.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-22 16:39:32.000000 nexgen-0.9.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 16:39:32.000000 nexgen-0.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.643085 nexgen-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-22 16:39:32.000000 nexgen-0.9.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-22 16:39:32.000000 nexgen-0.9.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-22 16:39:32.000000 nexgen-0.9.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-22 16:39:32.000000 nexgen-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-22 16:39:32.000000 nexgen-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-22 16:39:32.000000 nexgen-0.9.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-22 16:39:32.000000 nexgen-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-22 16:39:32.000000 nexgen-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-22 16:39:32.000000 nexgen-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-22 16:39:32.000000 nexgen-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-22 16:39:35.659085 nexgen-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-22 16:39:32.000000 nexgen-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.643085 nexgen-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/api_beamlines.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/beamlines.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5119 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-22 16:39:32.000000 nexgen-0.9.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-22 16:39:32.000000 nexgen-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-22 16:39:32.000000 nexgen-0.9.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-22 16:39:32.000000 nexgen-0.9.1/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:39:35.659085 nexgen-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.639085 nexgen-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.643085 nexgen-0.9.1/src/nexgen/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.647085 nexgen-0.9.1/src/nexgen/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/ED_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/ED_singla_nxs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.647085 nexgen-0.9.1/src/nexgen/beamlines/GDAtools/
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/GDAtools/ExtendedRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/GDAtools/GDAjson2params.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/GDAtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/I19_2_gda_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19350 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/I19_2_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/I19_2_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/I24_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/SSX_Eiger_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/SSX_Tristan_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/SSX_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/SSX_expt.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/beamlines/beamline_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.647085 nexgen-0.9.1/src/nexgen/command_line/
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/ED_mrc_to_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/ED_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/I19_2_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/SSX_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/copy_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/nexus_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/nxs_phil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/command_line/phil_files_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.651085 nexgen-0.9.1/src/nexgen/nxs_copy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_copy/copy_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_copy/copy_tristan_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_copy/copy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.651085 nexgen-0.9.1/src/nexgen/nxs_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/axes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/goniometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/scan_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.651085 nexgen-0.9.1/src/nexgen/nxs_write/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_write/nxclass_writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22162 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_write/nxmx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/nxs_write/write_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.651085 nexgen-0.9.1/src/nexgen/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/DLS_Template.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/ED_Singla.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/I03_Eiger.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/I19-2_Eiger.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/I19-2_Tristan.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/I24_Eiger.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/VMXi.phil
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.655085 nexgen-0.9.1/src/nexgen/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/data_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/ed_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/meta_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/metafile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/mrc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/tools/vds_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-22 16:39:32.000000 nexgen-0.9.1/src/nexgen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.659085 nexgen-0.9.1/src/nexgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-22 16:39:35.000000 nexgen-0.9.1/src/nexgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-22 16:39:35.000000 nexgen-0.9.1/src/nexgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:39:35.000000 nexgen-0.9.1/src/nexgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-22 16:39:35.000000 nexgen-0.9.1/src/nexgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-22 16:39:35.000000 nexgen-0.9.1/src/nexgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 16:39:35.000000 nexgen-0.9.1/src/nexgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.655085 nexgen-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.655085 nexgen-0.9.1/tests/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/test_GDA_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/test_SSX_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/test_SSX_expt.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/test_SSXwriters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/test_beamline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/beamlines/test_i19nxs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.655085 nexgen-0.9.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/cli/test_cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.655085 nexgen-0.9.1/tests/nxs_copy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_copy/test_copy_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.655085 nexgen-0.9.1/tests/nxs_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_utils/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_utils/test_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_utils/test_goniometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_utils/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_utils/test_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.659085 nexgen-0.9.1/tests/nxs_write/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_write/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17441 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_write/test_NXclassWriters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_write/test_NXmxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/nxs_write/test_write_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:35.659085 nexgen-0.9.1/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/tools/test_VDS_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/tools/test_meta_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-22 16:39:32.000000 nexgen-0.9.1/tests/tools/test_tools_for_ED.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.595804 nexgen-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 14:47:15.000000 nexgen-0.9.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 14:47:15.000000 nexgen-0.9.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 14:47:15.000000 nexgen-0.9.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.571804 nexgen-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.567804 nexgen-0.9.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.571804 nexgen-0.9.2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.575804 nexgen-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-09 14:47:15.000000 nexgen-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 14:47:15.000000 nexgen-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 14:47:15.000000 nexgen-0.9.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-09 14:47:15.000000 nexgen-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-09 14:47:15.000000 nexgen-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-09 14:47:15.000000 nexgen-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-09 14:47:15.000000 nexgen-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-09 14:47:21.595804 nexgen-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 14:47:15.000000 nexgen-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.575804 nexgen-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/api_beamlines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/beamlines.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5119 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-09 14:47:15.000000 nexgen-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 14:47:15.000000 nexgen-0.9.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 14:47:15.000000 nexgen-0.9.2/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:47:21.595804 nexgen-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.567804 nexgen-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.575804 nexgen-0.9.2/src/nexgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.579804 nexgen-0.9.2/src/nexgen/beamlines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/ED_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/ED_singla_nxs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.579804 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/ExtendedRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/GDAjson2params.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I19_2_gda_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19350 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I19_2_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I19_2_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I24_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_Eiger_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_Tristan_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/beamline_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/command_line/
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/ED_mrc_to_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/ED_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/I19_2_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/SSX_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/copy_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/nexus_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/nxs_phil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/phil_files_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/nxs_copy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/copy_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/copy_tristan_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/copy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/nxs_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12330 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/goniometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/scan_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/nxs_write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36768 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/nxclass_writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22235 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/nxmx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/write_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/src/nexgen/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/DLS_Template.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/ED_Singla.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I03_Eiger.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I19-2_Eiger.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I19-2_Tristan.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I24_Eiger.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/VMXi.phil
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/src/nexgen/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/data_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/ed_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/meta_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/metafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/mrc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/vds_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/src/nexgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/tests/beamlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_GDA_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_SSX_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_SSX_expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_SSXwriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_beamline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_i19nxs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/cli/test_cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/nxs_copy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_copy/test_copy_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/nxs_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_goniometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/nxs_write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17441 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/test_NXclassWriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/test_NXmxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/test_write_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/test_VDS_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/test_meta_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/test_tools_for_ED.py
```

### Comparing `nexgen-0.9.1/.github/actions/install_requirements/action.yml` & `nexgen-0.9.2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/.github/dependabot.yml` & `nexgen-0.9.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/.github/workflows/code.yml` & `nexgen-0.9.2/.github/workflows/code.yml`

 * *Files 5% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 jobs:
   lint:
     # pull requests are a duplicate of a branch push if within the same repo.
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     runs-on: ubuntu-latest
 
     steps:
+      - name: Checkout nexgen
+        uses: actions/checkout@v4
+      
       - name: Setup Python
         uses: actions/setup-python@v5
         with:
           python-version: '3.10'
           architecture: x64
 
-      - name: Checkout nexgen
-        uses: actions/checkout@v4
-
       - name: Install python packages
         uses: ./.github/actions/install_requirements
         with:
           requirements_file: requirements-dev-3.x.txt
           install_options: -e .[dev]
           python_version: '3.10'
+          artifact_name: lint
 
       - name: Install ruff
         run: pip install ruff
 
       - name: Run ruff
         run: ruff check .
 
@@ -64,23 +65,24 @@
 
       - name: Install python packages
         uses: ./.github/actions/install_requirements
         with:
           python_version: ${{ matrix.python }}
           requirements_file: requirements-test-${{ matrix.os }}-${{ matrix.python }}.txt
           install_options: ${{ matrix.install }}
+          artifact_name: tests
 
       - name: List dependency tree
         run: pipdeptree
 
       - name: Run tests
         run: pytest
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v4
+        uses: codecov/codecov-action@v3
         # env:
         #   CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
         with:
           name: ${{ matrix.python }}/${{ matrix.os }}
           files: cov.xml
 
   dist:
@@ -96,15 +98,15 @@
 
       - name: Build sdist and wheel
         run: |
           export SOURCE_DATE_EPOCH=$(git log -1 --pretty=%ct) && \
           pipx run build
 
       - name: Upload sdist and wheel as artifacts
-        uses: actions/upload-artifact@v4.3.1
+        uses: actions/upload-artifact@v4.3.3
         with:
           name: ${{ env.DIST_WHEEL_PATH }}
           path: dist
 
       - name: Check for packaging errors
         run: pipx run twine check --strict dist/*
 
@@ -130,15 +132,15 @@
 
     environment:
       name: pypi
       url: https://pypi.org/p/nexgen
 
     steps:
       - name: Download wheel and lockfiles
-        uses: actions/download-artifact@v4.1.0
+        uses: actions/download-artifact@v4.1.7
         with:
           pattern: "*dist*"
 
       - name: Rename lockfiles and dist
         run: |
           mv lockfiles-${{ env.CONTAINER_PYTHON }}-dist-${{ github.sha }} lockfiles
           mv ${{ env.DIST_WHEEL_PATH }} dist
```

### Comparing `nexgen-0.9.1/.github/workflows/codeql.yml` & `nexgen-0.9.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/.gitignore` & `nexgen-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/.pre-commit-config.yaml` & `nexgen-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/.readthedocs.yaml` & `nexgen-0.9.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/CHANGELOG.md` & `nexgen-0.9.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # CHANGELOG
 
 
 
+## 0.9.2
+
+### Changed
+- Temporarily disabled external links in NXdetector and detectorSpecific groups which may have wrong data type in meta file.
+Currently unavailable fields: `serial_number`, `data_collection_date`, `eiger_fw_version`.
+- More CI fixes
+
+
 ## 0.9.1
 
 ### Changed
 - Small CI updates
 
 ### Removed
 - Dropped Python 3.9 support
@@ -13,15 +21,15 @@
 
 ## 0.9.0
 
 ### Changed
 - Module names refactored to follow python conventions
 
 ### Added
-- Added missing NXdetector fields for Eiger
+- Added missing NXdetector fields for Eiger.
 - Command line tool to convert mrc files from Ceta detector for Electron Diffraction.
 - Detector definition for Ceta detector.
 
 
 ## 0.8.7
 
 ## Fixed
```

### Comparing `nexgen-0.9.1/CONTRIBUTING.rst` & `nexgen-0.9.2/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 
 Because the `bump2version` package has not been updated to support newer versions of python (last one currently listed is 3.8), it might be best to only use it to
 automatically update all the version strings but without pushing the tags. This can be done by adding the `--no-tag` flag to the previous command.
 
 
 .. code-block:: console
+    
     bump2version {major,minor,patch} --no-tag --verbose
     git push
 
 
 Note that this should not create a release but simply update the version in all the files.
```

### Comparing `nexgen-0.9.1/LICENSE` & `nexgen-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/PKG-INFO` & `nexgen-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexgen
-Version: 0.9.1
+Version: 0.9.2
 Summary: Next Generation Nexus Generator
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Diamond Light Source
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `nexgen-0.9.1/README.rst` & `nexgen-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/Makefile` & `nexgen-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/api.rst` & `nexgen-0.9.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/api_beamlines.rst` & `nexgen-0.9.2/docs/api_beamlines.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/beamlines.rst` & `nexgen-0.9.2/docs/beamlines.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/conf.py` & `nexgen-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/make.bat` & `nexgen-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/docs/usage.rst` & `nexgen-0.9.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/pyproject.toml` & `nexgen-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8.0.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nexgen"
-version = "0.9.1"
+version = "0.9.2"
 description = "Next Generation Nexus Generator"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.10",
```

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/ED_params.py` & `nexgen-0.9.2/src/nexgen/beamlines/ED_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/ED_singla_nxs.py` & `nexgen-0.9.2/src/nexgen/beamlines/ED_singla_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/GDAtools/ExtendedRequest.py` & `nexgen-0.9.2/src/nexgen/beamlines/GDAtools/ExtendedRequest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/GDAtools/GDAjson2params.py` & `nexgen-0.9.2/src/nexgen/beamlines/GDAtools/GDAjson2params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/I19_2_gda_nxs.py` & `nexgen-0.9.2/src/nexgen/beamlines/I19_2_gda_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/I19_2_nxs.py` & `nexgen-0.9.2/src/nexgen/beamlines/I19_2_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/I19_2_params.py` & `nexgen-0.9.2/src/nexgen/beamlines/I19_2_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/I24_params.py` & `nexgen-0.9.2/src/nexgen/beamlines/I24_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/SSX_Eiger_nxs.py` & `nexgen-0.9.2/src/nexgen/beamlines/SSX_Eiger_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/SSX_Tristan_nxs.py` & `nexgen-0.9.2/src/nexgen/beamlines/SSX_Tristan_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/SSX_chip.py` & `nexgen-0.9.2/src/nexgen/beamlines/SSX_chip.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/SSX_expt.py` & `nexgen-0.9.2/src/nexgen/beamlines/SSX_expt.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/beamlines/beamline_utils.py` & `nexgen-0.9.2/src/nexgen/beamlines/beamline_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/ED_mrc_to_nexus.py` & `nexgen-0.9.2/src/nexgen/command_line/ED_mrc_to_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/ED_nexus.py` & `nexgen-0.9.2/src/nexgen/command_line/ED_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/I19_2_cli.py` & `nexgen-0.9.2/src/nexgen/command_line/I19_2_cli.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/SSX_cli.py` & `nexgen-0.9.2/src/nexgen/command_line/SSX_cli.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/__init__.py` & `nexgen-0.9.2/src/nexgen/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/cli_utils.py` & `nexgen-0.9.2/src/nexgen/command_line/cli_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/copy_nexus.py` & `nexgen-0.9.2/src/nexgen/command_line/copy_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/nexus_generator.py` & `nexgen-0.9.2/src/nexgen/command_line/nexus_generator.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/nxs_phil.py` & `nexgen-0.9.2/src/nexgen/command_line/nxs_phil.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/command_line/phil_files_cli.py` & `nexgen-0.9.2/src/nexgen/command_line/phil_files_cli.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/log.py` & `nexgen-0.9.2/src/nexgen/log.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_copy/copy_nexus.py` & `nexgen-0.9.2/src/nexgen/nxs_copy/copy_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_copy/copy_tristan_nexus.py` & `nexgen-0.9.2/src/nexgen/nxs_copy/copy_tristan_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_copy/copy_utils.py` & `nexgen-0.9.2/src/nexgen/nxs_copy/copy_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_utils/__init__.py` & `nexgen-0.9.2/src/nexgen/nxs_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_utils/axes.py` & `nexgen-0.9.2/src/nexgen/nxs_utils/axes.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_utils/detector.py` & `nexgen-0.9.2/src/nexgen/nxs_utils/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,22 @@
     "flatfield_applied": "_dectris/flatfield_correction_applied",
     "pixel_mask": "mask",
     "pixel_mask_applied": "_dectris/pixel_mask_applied",
     "bit_depth_readout": "_dectris/bit_depth_image",  # Gorilla to be consistent with NeXus format (and make DIALS work)
     "bit_depth_image": "_dectris/bit_depth_image",
     "detector_readout_time": "_dectris/detector_readout_time",
     "threshold_energy": "_dectris/threshold_energy",
+    "photon_energy": "_dectris/photon_energy",
     "software_version": "_dectris/software_version",
-    "serial_number": "_dectris/detector_number",
+    "ntrigger": "/_dectris/ntrigger",
+    # "serial_number": "/_dectris/detector_number",
+    # "eiger_fw_version": "/_dectris/eiger_fw_version",
+    # "data_collection_date": "/_dectris/data_collection_date",
 }
+# TODO see https://github.com/DiamondLightSource/nexgen/issues/236
 
 TRISTAN_CONST = {
     "flatfield": "Tristan10M_flat_field_coeff_with_Mo_17.479keV.h5",
     "flatfield_applied": False,
     "pixel_mask": "Tristan10M_mask_with_spec.h5",
     "pixel_mask_applied": False,
     "software_version": "1.1.3",
```

### Comparing `nexgen-0.9.1/src/nexgen/nxs_utils/goniometer.py` & `nexgen-0.9.2/src/nexgen/nxs_utils/goniometer.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_utils/scan_utils.py` & `nexgen-0.9.2/src/nexgen/nxs_utils/scan_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_utils/source.py` & `nexgen-0.9.2/src/nexgen/nxs_utils/source.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/nxs_write/nxclass_writers.py` & `nexgen-0.9.2/src/nexgen/nxs_write/nxclass_writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,17 +484,26 @@
             NXclass_logger.info(f"Found metadata in {meta.as_posix()} file.")
             meta_link = (
                 meta.name
                 if meta.parent == Path(nxsfile.filename).parent
                 else meta.as_posix()
             )
             for k, v in detector.detector_params.constants.items():
-                if k == "software_version":
-                    # Software version should go in detectorSpecific (NXcollection)
-                    break
+                if k in [
+                    "software_version",
+                    "ntrigger",
+                    "data_collection_date",
+                    "eiger_fw_version",
+                    "serial_number",
+                ]:
+                    # NOTE: Software version, eiger_fw_version ntrigger & date should
+                    # go in detectorSpecific (NXcollection)
+                    # TODO re-enable eiger_fw_version, date & serial_number
+                    # see https://github.com/DiamondLightSource/nexgen/issues/236
+                    continue
                 nxdetector[k] = h5py.ExternalLink(meta_link, v)
         else:
             NXclass_logger.warning(
                 """
                 Meta file for Eiger detector hasn't been specified.
                 No links will be written. Pixel mask and flatfield information missing.
                 """
@@ -645,39 +654,14 @@
 
     # Detector distance
     nxdetector.create_dataset("distance", data=dist.to("m").magnitude)
     create_attributes(
         nxdetector["distance"], ("units",), (format(dist.to("m").units, "~"))
     )
 
-    # Check if there are any remaining datasets to be written (usually from the meta file but not always)
-    others_with_units = {"detector_readout_time": "s", "threshold_energy": "eV"}
-    others = [
-        "bit_depth_image",
-        "serial_number",
-        "photon_energy",
-        *others_with_units.keys(),
-    ]
-    for dset in others:
-        if (
-            nxdetector.__contains__(dset) is False
-            and dset in detector.detector_params.constants.keys()
-        ):
-            val = (
-                np.string_(detector.detector_params.constants[dset])
-                if isinstance(detector.detector_params.constants[dset], str)
-                else detector.detector_params.constants[dset]
-            )
-            if val is not None:
-                nxdetector.create_dataset(dset, data=val)
-                if dset in others_with_units.keys():
-                    create_attributes(
-                        nxdetector[dset], ("units",), (others_with_units[dset],)
-                    )
-
 
 # NXdetector_module writer
 def write_NXdetector_module(
     nxsfile: h5py.File,
     module: Dict,
     image_size: List | Tuple,
     pixel_size: List | Tuple,
@@ -855,20 +839,17 @@
             )
         else:
             grp.create_dataset(
                 "software_version",
                 data=np.string_(detector_params.constants["software_version"]),
             )
     if "EIGER" in detector_params.description.upper() and meta:
-        for k, v in {
-            "data_collection_date": "/_dectris/data_collection_date",
-            "eiger_fw_version": "/_dectris/eiger_fw_version",
-            "ntrigger": "/_dectris/ntrigger",
-        }.items():
-            grp[k] = h5py.ExternalLink(meta.name, v)
+        for field in ["ntrigger"]:  # "data_collection_date", "eiger_fw_version"]
+            # TODO See https://github.com/DiamondLightSource/nexgen/issues/236
+            grp[field] = h5py.ExternalLink(meta.name, detector_params.constants[field])
     elif "TRISTAN" in detector_params.description.upper():
         tick = ureg.Quantity(detector_params.constants["detector_tick"])
         grp.create_dataset("detector_tick", data=tick.magnitude)
         grp["detector_tick"].attrs["units"] = np.string_(format(tick.units, "~"))
         freq = ureg.Quantity(detector_params.constants["detector_frequency"])
         grp.create_dataset("detector_frequency", data=freq.magnitude)
         grp["detector_frequency"].attrs["units"] = np.string_(format(freq.units, "~"))
```

### Comparing `nexgen-0.9.1/src/nexgen/nxs_write/nxmx_writer.py` & `nexgen-0.9.2/src/nexgen/nxs_write/nxmx_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,18 @@
             write_NXdatetime(nxs, timestamp, dset_name)
         nxmx_logger.info(f"{dset_name} timestamp for collection updated.")
 
     def add_NXnote(self, notes: Dict, loc: str = "/entry/notes"):
         """Save any additional information as NXnote at the end of the collection.
 
         Args:
-            notes (Dict): Dictionary of (key, value) pairs where key represents the dataset name and value its data.
-            loc (str, optional): Location in the NeXus file to save metadata. Defaults to "/entry/notes".
+            notes (Dict): Dictionary of (key, value) pairs where key represents the \
+                dataset name and value its data.
+            loc (str, optional): Location in the NeXus file to save metadata. \
+                Defaults to "/entry/notes".
         """
         with h5py.File(self.filename, "r+") as nxs:
             write_NXnote(nxs, loc, notes)
         nxmx_logger.info(f"Notes saved in {loc}.")
 
     def write(
         self,
@@ -141,24 +143,26 @@
         write_mode: str = "x",
     ):
         """Write the NXmx format NeXus file.
 
         This function calls the writers for the main NXclass objects.
 
         Args:
-            image_datafiles (List | None, optional): List of image data files. If not passed, the program will look for \
-                files with the stem_######.h5 in the target directory. Defaults to None.
-            image_filename (str | None, optional): Filename stem to use to look for image files. Needed in case it doesn't match \
-                the NeXus file name. Format: filename_runnumber. Defaults to None.
-            start_time (datetime | str, optional): Collection start time if available, in the format "%Y-%m-%dT%H:%M:%SZ".\
+            image_datafiles (List | None, optional): List of image data files. If not passed, \
+                the program will look for files with the stem_######.h5 in the target directory. \
                 Defaults to None.
-            est_end_time (datetime | str, optional): Collection estimated end time if available, in the format "%Y-%m-%dT%H:%M:%SZ".\
+            image_filename (str | None, optional): Filename stem to use to look for image files. \
+                Needed in case it doesn't match the NeXus file name. Format: filename_runnumber. \
                 Defaults to None.
-            write_mode (str, optional): String indicating writing mode for the output NeXus file. Accepts any valid \
-                h5py file opening mode. Defaults to "x".
+            start_time (datetime | str, optional): Collection start time if available, in the \
+                format "%Y-%m-%dT%H:%M:%SZ".Defaults to None.
+            est_end_time (datetime | str, optional): Collection estimated end time if available, \
+                in the format "%Y-%m-%dT%H:%M:%SZ". Defaults to None.
+            write_mode (str, optional): String indicating writing mode for the output NeXus file. \
+                Accepts any valid h5py file opening mode. Defaults to "x".
         """
         metafile = self._get_meta_file(image_filename)
         if metafile:
             nxmx_logger.debug(f"Metafile name: {metafile.as_posix()}.")
 
         datafiles = (
             image_datafiles
```

### Comparing `nexgen-0.9.1/src/nexgen/nxs_write/write_utils.py` & `nexgen-0.9.2/src/nexgen/nxs_write/write_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/DLS_Template.phil` & `nexgen-0.9.2/src/nexgen/templates/DLS_Template.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/ED_Singla.phil` & `nexgen-0.9.2/src/nexgen/templates/ED_Singla.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/I03_Eiger.phil` & `nexgen-0.9.2/src/nexgen/templates/I03_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/I19-2_Eiger.phil` & `nexgen-0.9.2/src/nexgen/templates/I19-2_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/I19-2_Tristan.phil` & `nexgen-0.9.2/src/nexgen/templates/I19-2_Tristan.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/I24_Eiger.phil` & `nexgen-0.9.2/src/nexgen/templates/I24_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/templates/VMXi.phil` & `nexgen-0.9.2/src/nexgen/templates/VMXi.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/tools/constants.py` & `nexgen-0.9.2/src/nexgen/tools/constants.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/tools/data_writer.py` & `nexgen-0.9.2/src/nexgen/tools/data_writer.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/tools/ed_tools.py` & `nexgen-0.9.2/src/nexgen/tools/ed_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/tools/meta_reader.py` & `nexgen-0.9.2/src/nexgen/tools/meta_reader.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/tools/metafile.py` & `nexgen-0.9.2/src/nexgen/tools/metafile.py`

 * *Files 18% similar despite different names*

```diff
@@ -155,20 +155,57 @@
         _loc_material = [obj for obj in self.walk if "sensor_material" in obj]
         _loc_thickness = [obj for obj in self.walk if "sensor_thickness" in obj]
         return (
             self.__getitem__(_loc_material[0])[0],
             self.__getitem__(_loc_thickness[0])[0],
         )
 
-    def get_bit_depth_image(self):
+    def get_bit_depth_image(self) -> int:
         _loc = [obj for obj in self.walk if "bit_depth_image" in obj]
         if len(_loc) == 0:
             return None
         return self.__getitem__(_loc[0])[0]
 
+    def get_data_collection_date(self) -> str:
+        if self.hasDectrisGroup:
+            config = self.read_dectris_config()
+            return config["data_collection_date"]
+        if self.hasConfig:
+            config = self.read_config_dset()
+            return config["data_collection_date"]
+        _loc = [obj for obj in self.walk if "data_collection_date" in obj]
+        if len(_loc) == 0:
+            return None
+        return self.__getitem__(_loc[0])[0]
+
+    def get_fw_version(self) -> str:
+        if self.hasDectrisGroup:
+            config = self.read_dectris_config()
+            return config["eiger_fw_version"]
+        if self.hasConfig:
+            config = self.read_config_dset()
+            return config["eiger_fw_version"]
+        _loc = [obj for obj in self.walk if "eiger_fw_version" in obj]
+        if len(_loc) == 0:
+            return None
+        return self.__getitem__(_loc[0])[0]
+
+    def get_serial_number(self) -> str:
+        # Stored in meta file as "detector_number"
+        if self.hasDectrisGroup:
+            config = self.read_dectris_config()
+            return config["detector_number"]
+        if self.hasConfig:
+            config = self.read_config_dset()
+            return config["detector_number"]
+        _loc = [obj for obj in self.walk if "detector_number" in obj]
+        if len(_loc) == 0:
+            return None
+        return self.__getitem__(_loc[0])[0]
+
     def find_mask(self) -> Tuple[str, str]:
         if self.hasMask:
             mask_path = [obj for obj in self.walk if obj.lower() == "mask"]
             mask_applied_path = [obj for obj in self.walk if "mask_applied" in obj]
             if len(mask_applied_path) == 0:
                 return (mask_path[0], None)
             return (mask_path[0], mask_applied_path[0])
```

### Comparing `nexgen-0.9.1/src/nexgen/tools/mrc_tools.py` & `nexgen-0.9.2/src/nexgen/tools/mrc_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/tools/vds_tools.py` & `nexgen-0.9.2/src/nexgen/tools/vds_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen/utils.py` & `nexgen-0.9.2/src/nexgen/utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/src/nexgen.egg-info/PKG-INFO` & `nexgen-0.9.2/src/nexgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexgen
-Version: 0.9.1
+Version: 0.9.2
 Summary: Next Generation Nexus Generator
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Diamond Light Source
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `nexgen-0.9.1/src/nexgen.egg-info/SOURCES.txt` & `nexgen-0.9.2/src/nexgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/conftest.py` & `nexgen-0.9.2/tests/beamlines/conftest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/test_GDA_tools.py` & `nexgen-0.9.2/tests/beamlines/test_GDA_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/test_SSX_chip.py` & `nexgen-0.9.2/tests/beamlines/test_SSX_chip.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/test_SSX_expt.py` & `nexgen-0.9.2/tests/beamlines/test_SSX_expt.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/test_SSXwriters.py` & `nexgen-0.9.2/tests/beamlines/test_SSXwriters.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/test_beamline_utils.py` & `nexgen-0.9.2/tests/beamlines/test_beamline_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/beamlines/test_i19nxs.py` & `nexgen-0.9.2/tests/beamlines/test_i19nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/cli/test_cli_utils.py` & `nexgen-0.9.2/tests/cli/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_copy/test_copy_tools.py` & `nexgen-0.9.2/tests/nxs_copy/test_copy_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_utils/test_axes.py` & `nexgen-0.9.2/tests/nxs_utils/test_axes.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_utils/test_detector.py` & `nexgen-0.9.2/tests/nxs_utils/test_detector.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_utils/test_goniometer.py` & `nexgen-0.9.2/tests/nxs_utils/test_goniometer.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_utils/test_scan.py` & `nexgen-0.9.2/tests/nxs_utils/test_scan.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_utils/test_source.py` & `nexgen-0.9.2/tests/nxs_utils/test_source.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_write/conftest.py` & `nexgen-0.9.2/tests/nxs_write/conftest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_write/test_NXclassWriters.py` & `nexgen-0.9.2/tests/nxs_write/test_NXclassWriters.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_write/test_NXmxWriter.py` & `nexgen-0.9.2/tests/nxs_write/test_NXmxWriter.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/nxs_write/test_write_utils.py` & `nexgen-0.9.2/tests/nxs_write/test_write_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/test_log.py` & `nexgen-0.9.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/test_utils.py` & `nexgen-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/test_version.py` & `nexgen-0.9.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/tools/test_VDS_tools.py` & `nexgen-0.9.2/tests/tools/test_VDS_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/tools/test_meta_tools.py` & `nexgen-0.9.2/tests/tools/test_meta_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.1/tests/tools/test_tools_for_ED.py` & `nexgen-0.9.2/tests/tools/test_tools_for_ED.py`

 * *Files identical despite different names*


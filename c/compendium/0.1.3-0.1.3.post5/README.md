# Comparing `tmp/compendium-0.1.3.tar.gz` & `tmp/compendium-0.1.3.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compendium-0.1.3.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `compendium-0.1.3.tar` & `compendium-0.1.3.post5.tar`

### file list

```diff
@@ -1,18 +1,123 @@
--rw-r--r--   0        0        0    11357 2022-10-02 17:06:05.714151 compendium-0.1.3/LICENSE
--rw-r--r--   0        0        0     4199 2022-10-02 22:26:25.380512 compendium-0.1.3/README.md
--rw-r--r--   0        0        0     2515 2022-10-04 01:32:42.979838 compendium-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      864 2022-10-04 01:34:35.715677 compendium-0.1.3/src/compendium/__init__.py
--rw-r--r--   0        0        0    11676 2022-10-04 01:03:24.927770 compendium-0.1.3/src/compendium/config_manager.py
--rw-r--r--   0        0        0      606 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/exceptions.py
--rw-r--r--   0        0        0     5252 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filepaths.py
--rw-r--r--   0        0        0      715 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filetypes/__init__.py
--rw-r--r--   0        0        0     1897 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filetypes/ini.py
--rw-r--r--   0        0        0     2055 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filetypes/json.py
--rw-r--r--   0        0        0     2584 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filetypes/toml.py
--rw-r--r--   0        0        0     2053 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filetypes/xml.py
--rw-r--r--   0        0        0     2197 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/filetypes/yaml.py
--rw-r--r--   0        0        0     5827 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/loader.py
--rw-r--r--   0        0        0        0 2022-10-02 17:06:05.717151 compendium-0.1.3/src/compendium/py.typed
--rw-r--r--   0        0        0    12110 2022-10-04 01:31:14.451179 compendium-0.1.3/src/compendium/settings.py
--rw-r--r--   0        0        0     5309 1970-01-01 00:00:00.000000 compendium-0.1.3/setup.py
--rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 compendium-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.flake8
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/mkdocs.yml
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/versioning.tar.gz
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/configuration.md
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/index.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/schema.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/settings.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/config_manager.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes_base.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/loader.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/paths.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/settings.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/json.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/toml.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/xml.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/yaml.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config.toml
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested_env.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/settings.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/settings.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/check.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/config_file.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/example-out.yaml
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/example.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/in.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/in.toml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/in.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/out.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/out.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/out.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/config1.toml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/config2.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/config_manager.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/config1.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/config2.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/example.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/multiconfig.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/prototype.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/read_write.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/hierarchial/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/hierarchial/config.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/hierarchial/config_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/marshmallow/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/pydantic/.keep
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/simple/example-out.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/simple/example.yaml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/simple/example_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/hidden/.example
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/hidden/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/hidden/config.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/__init__.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman.py
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/proman-lock.json
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/proman-lock.json
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule1/proman-lock.json
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule2/proman-lock.json
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule2/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module2/proman-lock.json
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module2/pyproject.toml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/node.toml
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/tree.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/dry/node.toml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/dry/dehiscent/node.toml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/dry/indehiscent/node.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/node.toml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/berry/node.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/berry/hesperidium/node.toml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/drupe/node.toml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/pome/node.toml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/__init__.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/config_manager.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/exceptions.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filepaths.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/py.typed
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/settings.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/__init__.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/ini.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/json.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/toml.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/xml.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/yaml.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/__init__.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/build.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/doc.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/qa.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/config.toml
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/test_config_manager.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/test_settings.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/test_version.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/test_filepaths.py.bak
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/settings1.toml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/settings2.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/settings3.toml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/test_hierarchy.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/fruit.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/fruit1.toml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/fruit2.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/test_tree.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/ini/config.ini
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/ini/test_ini.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/json/config.json
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/json/test_json.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/module/config.toml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/toml/config.toml
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/toml/test_toml.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/xml/config.xml
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/xml/test_xml.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/yaml/config.yaml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/yaml/test_yaml.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/LICENSE
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/README.md
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/pyproject.toml
+-rw-r--r--   0        0        0    19600 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/PKG-INFO
```

### Comparing `compendium-0.1.3/LICENSE` & `compendium-0.1.3.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3/README.md` & `compendium-0.1.3.post5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -166,11 +166,11 @@
 #
 # ```
 -->
 
 ### Development
 
 ```
-poetry shell
-poetry install
+python -m venv .vev
+pip install -e .[dev]
 python -m doctest README.md
 ```
```

### Comparing `compendium-0.1.3/pyproject.toml` & `compendium-0.1.3.post5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["hatchling>=1.11.0"]
+build-backend = "hatchling.build"
 
-[tool.poetry]
+[project]
 name = "compendium"
-version = "0.1.3"
+version = "0.1.3.post5"
 description = "Simple layered configuraion tool"
-authors = ["Jesse P. Johnson <jpj6652@gmail.com>"]
-homepage = "https://github.com/kuwv/python-compendium"
-documentation = "https://kuwv.github.io/python-compendium"
-license = "Apache-2.0"
+authors = [{name="Jesse P. Johnson", email="jpj6652@gmail.com"}]
+maintainers = [{name="Jesse P. Johnson", email="jpj6652@gmail.com"}]
+requires-python = ">=3.6.2"
+license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["configuration", "configuration management"]
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Software Development :: Libraries"
 ]
-packages = [
-    { include = "compendium", from = "src" },
+dependencies = [
+    "ruamel.yaml>=0.16.10,<1",
+    "anytree>=2.8.0",
+    # "dataclasses>=0.8;python_version<3.7",
+    "dpath>=2.0.1",
+    "tomlkit>=0.7.0,<1",
+    # "jsonschema>=3.2.0",
+    # "xmlschema>=1.2.3",
+    # "yamale>=3.0.2"
 ]
 
-[tool.poetry.dependencies]
-python = "^3.6.2"
-"ruamel.yaml" = "^0.16.10"
-anytree = "^2.8.0"
-# dataclasses = {version = "^0.8", python = "~3.6", optional = true}
-dpath = "^2.0.1"
-tomlkit = "^0.7.0"
-xmltodict = {version = "^0.12.0", optional = true}
-# jsonschema = "^3.2.0"
-# xmlschema = "^1.2.3"
-# yamale = "^3.0.2"
-
-[tool.poetry.extras]
-xml = ["xmltodict"]
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^6.2"
-flake8 = "^3.8.2"
-black = "^19.10b0"
-invoke = "^1.4.1"
-pyfakefs = "^4.0.2"
-pytest-cov = "^2.9.0"
-safety = "^1.9.0"
-isort = {extras = ["pyproject"], version = "^4.3.21"}
-mkdocs = "^1.1.2"
-pydocstyle = {extras = ["toml"], version = "^6.1.1"}
-mkdocstrings = "^0.12.1"
-bandit = "^1.6.2"
-docstr-coverage = "^1.2.0"
-mkdocs-material = "^7.1.2"
-proman-versioning = "^0.1.1-beta.4"
-mypy = ">=0.910"
-mypy-extensions = ">=0.4.3"
+[project.optional-dependencies]
+xml = ["xmltodict>=0.12.0,<1"]
+build = [
+    "build",
+    "proman-versioning>=0.1.1-beta.4,<1",
+    "proman-workflows>=0.1.0a8,<1",
+    "invoke>=1.4.1"
+]
+dev = [
+    "pytest>=6.2.5",
+    "pyfakefs>=5.4.1",
+    "pytest-cov>=2.9.0",
+    "isort[pyproject]>=4.3.21",
+    "black>=24.1.0",
+    "flake8>=3.8.2",
+    "pylint>=2.9.5",
+    "bandit>=1.6.2",
+    "safety>=2.2.0",
+    "mypy>=1",
+    "mypy-extensions>=0.4.3"
+]
+docs = [
+    "mkdocs>=1.1.2,<2",
+    "pydocstyle[toml]>=6.1.1,<7",
+    "mkdocstrings>=0.12.1,<1",
+    "mkdocs-material>=7.1.2,<8",
+    "docstr-coverage>=1.2.0,<2"
+]
 
-[tool.proman.versioning]
+[project.urls]
+homepage = "https://github.com/kuwv/python-compendium"
+documentation = "https://kuwv.github.io/python-compendium"
 
 [[tool.proman.versioning.files]]
 filepath = "pyproject.toml"
 pattern = "version = \"${version}\""
 
 [[tool.proman.versioning.files]]
 filepath = "src/compendium/__init__.py"
@@ -74,37 +83,61 @@
 filepath = "tests/test_version.py"
 pattern = "__version__ == '${version}'"
 
 [tool.pydocstyle]
 ignore = [
     "D203",
     "D213",
-    "D300"
+    "D300",
 ]
 
+[tool.pylint]
+fail-under = 9.0
+
+[tool.pylint."MESSAGES CONTROL"]
+disable = [
+    "R0903",
+    "C0103",
+    "W0715"
+]
+
+[tool.pylint."FORMAT"]
+max-line-length = 79
+
+[tool.pylint."MISCELLANEOUS"]
+notes = []
+
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.black]
 line-length = 79
 skip-string-normalization = true
 include = '\.pyi?$'
 exclude = '''
-
 (
   /(
     | \.git
+    | \.github
     | \.mypy_cache
     | \.pytest_cache
-    | _build
     | build
     | dist
+    | docs
+    | site
   )
 )
 '''
 
 [tool.mypy]
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_untyped_defs = true
 ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+testpaths = [
+    # "examples",
+    "tests",
+]
+addopts = "--doctest-modules"
```

### Comparing `compendium-0.1.3/src/compendium/__init__.py` & `compendium-0.1.3.post5/src/compendium/__init__.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3/src/compendium/config_manager.py` & `compendium-0.1.3.post5/src/compendium/config_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             log.addHandler(logging.StreamHandler(log_handler))
 
         self.separator = kwargs.get('separator', '/')
 
         # Setup filepaths
         self.name = kwargs.pop('name', 'compendium')
         self._filepaths: List[ConfigFile] = [
-            (ConfigFile(f, factory_kwargs=kwargs) if type(f) == str else f)
+            (ConfigFile(f, factory_kwargs=kwargs) if isinstance(f, str) else f)
             for f in kwargs.pop('filepaths', [])
         ]
 
         # Load defaults
         defaults = kwargs.pop('defaults', {})
 
         # Populate settings
@@ -86,36 +86,35 @@
     @property
     def filepaths(self) -> Tuple[ConfigFile, ...]:
         """Retrieve filepaths."""
         return tuple(self._filepaths)
 
     def add_filepath(self, filepath: str) -> None:
         """Load settings from configuration in filepath."""
-        logging.debug(f"searching for {filepath}")
+        logging.debug('searching for %s', filepath)
         self._filepaths.append(ConfigFile(filepath))
 
     # def dump_config(self, config_file: ConfigFile) -> None:
     #     """Dump settings to configuration."""
     #     if os.path.exists(config_file.filepath):
     #         config_file.dump(self.data)
     #         if update:
     #             self.data.push(config_file)
 
     def load_config(
         self,
         config_file: ConfigFile,
-        update: bool = True,
-        *args: str,
+        # *args: str,
         **kwargs: Any,
     ) -> Optional[Dict[str, Any]]:
         """Load settings from configuration."""
         if os.path.exists(config_file.filepath):
             # config_file = ConfigFile(filepath=filepath, **kwargs)
             settings = config_file.load()
-            if update:
+            if kwargs.pop('update', True):
                 self.push(settings)
             return settings
         return None
 
     def load_configs(self, **kwargs: Any) -> None:
         """Load configuration files from filepaths."""
         for filepath in self._filepaths:
@@ -212,35 +211,33 @@
             super().load_config(self.filepaths[0])
         if load_children:
             self.load_configs()
 
     @property
     def namepaths(self) -> Tuple[str, ...]:
         """Return list of namepaths."""
-        return tuple([self.get_namepath(x.filepath) for x in self.filepaths])
+        return tuple(self.get_namepath(x.filepath) for x in self.filepaths)
 
     def get_name(self, filepath: str) -> str:
         """Get name from tree path."""
         name = os.path.dirname(os.path.relpath(filepath, self.basedir)).split(
             os.sep
         )[-1]
         if name != '':
             return name
-        else:
-            return self.name
+        return self.name
 
     def get_namepath(self, filepath: str) -> str:
         """Get name from tree path."""
         name = os.path.dirname(
             os.path.relpath(filepath, self.basedir),
         ).replace(os.sep, self.separator)
         if name != '':
             return f"{self.separator}{self.name}{self.separator}{name}"
-        else:
-            return f"{self.separator}{self.name}"
+        return f"{self.separator}{self.name}"
 
     def get_filepath(self, name: str) -> Optional[str]:
         """Get filepath from namepath."""
         for config in self.filepaths:
             if name == self.get_namepath(config.filepath):
                 return config.filepath
         return None
@@ -271,21 +268,20 @@
         ):
             if filepath not in self.filepaths:
                 self.add_filepath(filepath)
 
     def load_config(
         self,
         config_file: ConfigFile,
-        update: bool = False,
         *args: str,
         **kwargs: Any,
     ) -> Optional[Dict[str, Any]]:
         """Load config."""
         # TODO: need to separate chainmap of defaults from namespace config
-        settings = super().load_config(config_file, update)
+        settings = super().load_config(config_file, **kwargs)
         return self.new_child(
             settings, name=self.get_name(config_file.filepath), *args, **kwargs
         )
 
     def load_configs(self, **kwargs: Any) -> None:
         """Load configuration files from filepaths."""
```

### Comparing `compendium-0.1.3/src/compendium/exceptions.py` & `compendium-0.1.3.post5/src/compendium/exceptions.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3/src/compendium/filepaths.py` & `compendium-0.1.3.post5/src/compendium/filepaths.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 from typing import List, Optional, Tuple
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class File:
+    """Provide file info."""
+
     path: str
     name: str = field(init=False)
     extension: Optional[str] = field(init=False)
 
     def __post_init__(self) -> None:
         """Intialize filepath."""
-        self.name = os.path.basename(self.filepath) or 'config.toml'
+        self.name = os.path.basename(self.path) or 'config.toml'
 
         if '.' in self.name and not self.name.startswith('.'):
             self.extension = os.path.splitext(self.name)[-1].strip('.')
         else:
             self.extension = 'toml'
 
 
 @dataclass
-class ConfigPaths:
+class ConfigPaths:  # pylint: disable=too-many-instance-attributes
     r"""Load config paths based on priority.
 
     First(lowest) to last(highest):
       1. Load config.<FILETYPE> from /etc/<APP>
         - /etc/<FILENAME>
         - /etc/<APP>/config.<FILETYPE>
         - /etc/<APP>/<FILENAME>
@@ -48,16 +50,14 @@
       4. Runtime configs:
         - /etc/sysconfig/<APP>
         - .env
         - <CLI>
 
     """
 
-    # TODO: Implement pathlib
-
     name: str
     filename: str
     filetype: Optional[str] = field(init=False)
     basedir: str = os.sep
 
     enable_system_filepaths: bool = False
     enable_global_filepaths: bool = False
@@ -102,15 +102,16 @@
 
         if self.enable_global_filepaths:
             if platform.system() == 'Windows':
                 __global_app_filepath = os.path.join('AppData', 'Local')
 
             if platform.system() == 'Darwin':
                 __global_app_filepath = os.path.join(
-                    'Library', 'Application Support',
+                    'Library',
+                    'Application Support',
                 )
 
             if platform.system() == 'Linux':
                 __global_app_filepath = '.config'
 
             self.global_filepaths.append(
                 os.path.join(
```

### Comparing `compendium-0.1.3/src/compendium/filetypes/__init__.py` & `compendium-0.1.3.post5/src/compendium/filetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3/src/compendium/filetypes/ini.py` & `compendium-0.1.3.post5/src/compendium/filetypes/ini.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             data[k] = v
         return data
 
     def dump_config(self, content: Dict[str, Any], filepath: str) -> None:
         """Save settings to toml configuration."""
         logging.info('TomlConfig: saving configuration file')
         try:
-            with open(filepath, 'w') as f:
-                self.__config_parser.write(f)
+            with open(filepath, 'w', encoding=self.encoding) as file:
+                self.__config_parser.write(file)
         except IOError as err:
             if err.errno == errno.EACCES:
                 logging.error(
                     'You do not have permission to write to this file'
                 )
                 raise
```

### Comparing `compendium-0.1.3/src/compendium/filetypes/json.py` & `compendium-0.1.3.post5/src/compendium/filetypes/json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
 """Control JSON module."""
 
 # import datetime
 import errno
 import json
+
 # import jsonschema
 import logging
 import os
 from typing import Any, Dict, Tuple
 
 from compendium.filetypes import FiletypesBase
 
@@ -27,26 +28,29 @@
         """Return support JSON file extensions."""
         return ('json',)
 
     def load_config(self, filepath: str) -> Dict[str, Any]:
         """Load settings from JSON configuration."""
         logging.info('loading JSON configuration file')
         if os.path.isfile(filepath):
-            with open(filepath, 'r', encoding=self.encoding) as f:
-                content = json.load(f)
+            with open(filepath, 'r', encoding=self.encoding) as file:
+                content = json.load(file)
         else:
             content = {}
         return content
 
     def dump_config(self, content: Dict[str, Any], filepath: str) -> None:
         """Save settings to JSON configuration."""
         try:
-            with open(filepath, 'w') as f:
+            with open(filepath, 'w', encoding=self.encoding) as file:
                 json.dump(
-                    content, f, indent=2, sort_keys=False
+                    content,
+                    file,
+                    indent=2,
+                    sort_keys=False
                     # , default=self.encoder
                 )
         except IOError as err:
             if err.errno == errno.EACCES:
                 logging.error(
                     'You do not have permission to write to this file'
                 )
```

### Comparing `compendium-0.1.3/src/compendium/filetypes/toml.py` & `compendium-0.1.3.post5/src/compendium/filetypes/toml.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
         See: https://github.com/sdispater/tomlkit/issues/43
 
         """
         # convert associative array
         if isinstance(content, dict):
             content = {
-                str(k): TomlConfig._convert(v)
-                for k, v in content.items()
+                str(k): TomlConfig._convert(v) for k, v in content.items()
             }
 
         # convert list
         elif isinstance(content, list):
             content = [TomlConfig._convert(x) for x in content]
 
         # convert scalars
@@ -55,26 +54,26 @@
 
         return content
 
     def load_config(self, filepath: str) -> Dict[str, Any]:
         """Load settings from toml configuration."""
         logging.info('loading TOML configuration file')
         if os.path.isfile(filepath):
-            with open(filepath, 'r', encoding=self.encoding) as f:
-                content = self._convert(tomlkit.parse(f.read()))
+            with open(filepath, 'r', encoding=self.encoding) as file:
+                content = self._convert(tomlkit.parse(file.read()))
         else:
             content = {}
         return content
 
     def dump_config(self, content: Dict[str, Any], filepath: str) -> None:
         """Save settings to toml configuration."""
         logging.info('TomlConfig: saving configuration file')
         try:
-            with open(filepath, 'w') as f:
+            with open(filepath, 'w', encoding=self.encoding) as file:
                 # XXX: tomlkit is missing union of tomldocument and dict
-                f.write(tomlkit.dumps(content))  # type: ignore
+                file.write(tomlkit.dumps(content))
         except IOError as err:
             if err.errno == errno.EACCES:
                 logging.error(
                     'You do not have permission to write to this file'
                 )
                 raise
```

### Comparing `compendium-0.1.3/src/compendium/filetypes/xml.py` & `compendium-0.1.3.post5/src/compendium/filetypes/xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
 """Control XML module."""
+
 # import datetime
 import errno
 import logging
 import os
 from typing import Any, Dict, Tuple
 
 import xmltodict
@@ -28,34 +29,32 @@
         """Return supported XML configuration file extensions."""
         return ('xml',)
 
     def load_config(self, filepath: str) -> Dict[str, Any]:
         """Load settings from XML configuration."""
         logging.info('loading XML configuration file')
         if os.path.isfile(filepath):
-            with open(filepath, 'r') as f:
+            with open(filepath, 'r', encoding=self.encoding) as file:
                 content = xmltodict.parse(
-                    f.read(),
+                    file.read(),
                     encoding=self.encoding,
                     process_namespaces=self.process_namespaces,
-                    namespaces=self.namespaces
+                    namespaces=self.namespaces,
                 )
         else:
             content = {}
         return content
 
     def dump_config(self, content: Dict[str, Any], filepath: str) -> None:
         """Save settings to XML configuration."""
         try:
-            with open(filepath, 'w') as f:
-                f.write(
+            with open(filepath, 'w', encoding=self.encoding) as file:
+                file.write(
                     xmltodict.unparse(
-                        content,
-                        encoding=self.encoding,
-                        pretty=True
+                        content, encoding=self.encoding, pretty=True
                     )
                 )
         except IOError as err:
             if err.errno == errno.EACCES:
                 logging.error(
                     'You do not have permission to write to this file'
                 )
```

### Comparing `compendium-0.1.3/src/compendium/filetypes/yaml.py` & `compendium-0.1.3.post5/src/compendium/filetypes/yaml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
 """Control YAML configuration module."""
 
 import errno
 import logging
 import os
+
 # import textwrap
 from typing import Any, Dict, Tuple
 
 from ruamel.yaml import YAML
+
 # from ruamel.yaml.scalarstring import LiteralScalarString
 
 from compendium.filetypes import FiletypesBase
 
 # TODO consider strictyaml or poyo
 # def literal_scalar_string(content):
 #     """Prepare multiline string as yaml scalar."""
@@ -27,39 +29,39 @@
         logging.info('Inializing YamlConfig')
         self.encoding = kwargs.get('encoding', 'utf-8')
         self.kind = kwargs.get('kind', None)
 
     def __yaml_parser(self, kind: str) -> YAML:
         """Get yaml parser."""
         yaml = YAML(typ=kind)
-        yaml.explicit_start = True  # type: ignore
-        yaml.preserve_quotes = True  # type: ignore
+        yaml.explicit_start = True
+        yaml.preserve_quotes = True
         return yaml
 
     @staticmethod
     def extensions() -> Tuple[str, ...]:
         """Return support YAML file extensions."""
         return ('yaml', 'yml')
 
     def load_config(self, filepath: str) -> Dict[str, Any]:
         """Load settings from YAML configuration."""
-        logging.info(f"loading YAML configuration file {filepath}")
+        logging.info('loading YAML configuration file %s', filepath)
         if os.path.isfile(filepath):
-            with open(filepath, 'r', encoding=self.encoding) as f:
+            with open(filepath, 'r', encoding=self.encoding) as file:
                 yaml = self.__yaml_parser(self.kind or 'safe')
-                content = yaml.load(f)
+                content = yaml.load(file)
         else:
             content = {}
         return content
 
     def dump_config(self, content: Dict[str, Any], filepath: str) -> None:
         """Save settings to YAML configuration."""
         try:
-            with open(filepath, 'w') as f:
+            with open(filepath, 'w', encoding=self.encoding) as file:
                 yaml = self.__yaml_parser(self.kind or 'rt')
-                yaml.dump(content, f)
+                yaml.dump(content, file)
         except IOError as err:
             if err.errno == errno.EACCES:
                 logging.error(
                     'You do not have permission to write to this file'
                 )
                 raise
```

### Comparing `compendium-0.1.3/src/compendium/loader.py` & `compendium-0.1.3.post5/src/compendium/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
+# pylint: disable=unused-import
 """Control configuration files."""
 
 # from weakref import ref
 import importlib
 import logging
 import os
 from typing import Any, Dict, Optional, Type
 
 from compendium import exceptions
 from compendium.filetypes import FiletypesBase
-from compendium.filetypes.ini import IniConfig  # noqa
-from compendium.filetypes.json import JsonConfig  # noqa
-from compendium.filetypes.toml import TomlConfig  # noqa
-from compendium.filetypes.yaml import YamlConfig  # noqa
+from compendium.filetypes.ini import IniConfig
+from compendium.filetypes.json import JsonConfig
+from compendium.filetypes.toml import TomlConfig
+from compendium.filetypes.yaml import YamlConfig
 from compendium.settings import Settings
 
 if importlib.util.find_spec('xmltodict'):  # type: ignore
-    from compendium.filetypes.xml import XmlConfig  # noqa
+    from compendium.filetypes.xml import XmlConfig
 
 log = logging.getLogger(__name__)
 
 
-class ConfigFile:
+class ConfigFile:  # pylint: disable=too-many-instance-attributes
     """Manage settings loaded from confiugrations using dpath."""
 
     # TODO: switch to dependency injection for filetypes
     def __init__(self, filepath: Optional[str] = None, **kwargs: Any) -> None:
         """Initialize single configuration file."""
         self.default_filetype = kwargs.pop('default_filetype', 'toml')
         self.default_filename = kwargs.pop(
             'default_filename', f"config.{self.default_filetype}"
         )
         if filepath:
             self.filepath = filepath
         self.writable = bool(kwargs.pop('writable', False))
-        self.autosave = bool(
-            kwargs.pop('autosave', True if self.writable else False)
-        )
+        self.autosave = bool(kwargs.pop('autosave', self.writable))
         self.factory: dict = kwargs.pop('factory', Settings)
         self.factory_kwargs: Dict[str, Any] = kwargs.pop('factory_kwargs', {})
 
+    def __eq__(self, other: object) -> bool:
+        """Check if path is equal to config file path."""
+        if isinstance(other, str):
+            return self.filepath == other
+        if isinstance(other, self.__class__):
+            return self == other
+        return False
+
     def __repr__(self) -> str:
         """Get filepath."""
         return repr(self.filepath)
 
     def __str__(self) -> str:
         """Return filepath."""
         return self.filepath
 
-    def __eq__(self, other: Any) -> bool:
-        """Check if path is equal to config file path."""
-        if type(other) == str:
-            return self.filepath == other
-        if type(other) == type(self):
-            return self == other
-        return False
-
     # def enter(self) -> None:
     #     ...
 
     # def exit(self, exc_type, exc_value, exc_tb)) -> None:
     #     ...
 
     # async def aenter(self) -> None:
@@ -69,15 +68,15 @@
     # async def aexit(self, exc_type, exc_value, exc_tb)) -> None:
     #     await ...
 
     def __get_class(
         self, filetype: Optional[str] = 'toml'
     ) -> Optional[Type[FiletypesBase]]:
         """Get class object from filetype module."""
-        for module in [m for m in FiletypesBase.__subclasses__()]:
+        for module in list(FiletypesBase.__subclasses__()):
             if filetype in module.extensions():
                 return module
         return None
 
     @property
     def filename(self) -> str:
         """Get filename from filepath."""
@@ -103,54 +102,49 @@
 
     @filepath.setter
     def filepath(self, filepath: str) -> None:
         """Set filepath."""
         self._filepath = filepath
         if not hasattr(self, '_strategy'):
             self._strategy: Dict[str, FiletypesBase] = {}
-        if filepath not in self._strategy.keys():
+        if filepath not in self._strategy:
             Class = self.__get_class(self.filetype)
             if Class:
                 self._strategy[filepath] = Class()
 
     def load(self, filepath: Optional[str] = None) -> Dict[str, Any]:
         """Load settings from configuration file."""
         self.filepath = filepath or self.filepath
         if self.filepath:
             # Use discovered module to load configuration.
             if os.path.exists(self.filepath):
-                logging.info(f"Retrieving configuration: '{filepath}'")
+                logging.info('Retrieving configuration: %s', filepath)
                 if self.strategy:
                     # TODO: combine factory and load_config
                     data = self.strategy.load_config(filepath=self.filepath)
                     return self.factory(
                         data, **self.factory_kwargs
                     )  # type: ignore
-                else:
-                    raise exceptions.DriverError(
-                        f"Error: No class found for: '{filepath}'"
-                    )
-            else:
-                raise exceptions.ConfigFileError(
-                    f"Skipping: No configuration found at: '{filepath}'"
+                raise exceptions.DriverError(
+                    f"Error: No class found for: '{filepath}'"
                 )
-        else:
-            raise exceptions.ConfigFileError('Error: no config file provided')
+            raise exceptions.ConfigFileError(
+                f"Skipping: No configuration found at: '{filepath}'"
+            )
+        raise exceptions.ConfigFileError('Error: no config file provided')
 
     def dump(
-        self,
-        data: Dict[str, Any],
-        filepath: Optional[str] = None
+        self, data: Dict[str, Any], filepath: Optional[str] = None
     ) -> None:
         """Save settings to configuraiton."""
         if self.writable:
             self.filepath = filepath or self.filepath
             if self.filepath:
                 # Use discovered module to save configuration
-                logging.info(f"Saving configuration: '{filepath}'")
+                logging.info('Saving configuration: %s', filepath)
                 if self.strategy:
                     # TODO: refactor to use respective dict from chainmap
                     self.strategy.dump_config(data, self.filepath)
                 else:
                     raise exceptions.DriverError(
                         f"Skipping: No class found for: '{filepath}'"
                     )
```

### Comparing `compendium-0.1.3/src/compendium/settings.py` & `compendium-0.1.3.post5/src/compendium/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,28 +3,33 @@
 """Provide settings modules."""
 
 import logging
 import os
 from ast import literal_eval
 from collections import ChainMap
 from collections.abc import MutableMapping
+from string import Template
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
+    Iterable,
     Iterator,
     Mapping,
     Optional,
+    Tuple,
+    Union,
 )
 
-from dpath import util as dpath
+import dpath
 from dpath.exceptions import PathNotFound
 
 if TYPE_CHECKING:
+    from _typeshed import SupportsKeysAndGetItem
     from mypy_extensions import KwArg, VarArg
 
 log = logging.getLogger(__name__)
 
 
 class Settings(MutableMapping):
     """Manage settings loaded from confiugrations using dpath."""
@@ -37,96 +42,109 @@
             Settings.separator = kwargs.pop('separator')
         self.data: Dict[str, Any] = {}
         if data is not None:
             self.update(data)
         if kwargs:
             self.update(kwargs)
 
-    def __delitem__(self, keypath: str) -> Any:
-        """Delete item at keypath."""
-        return dpath.delete(self.data, keypath, Settings.separator)
+    def __delitem__(self, key: str) -> Any:
+        """Delete item at key."""
+        return dpath.delete(self.data, key, Settings.separator)
 
     def __iter__(self) -> Iterator[Any]:
         """Iterate settings dictionary."""
         return iter(self.data)
 
     def __len__(self) -> int:
         """Return number of settings items."""
         return len(self.data)
 
-    def __getitem__(self, keypath: str) -> Any:
+    def __getitem__(self, key: str) -> Any:
         """Get item."""
-        return dpath.get(self.data, keypath, Settings.separator)
+        return dpath.get(self.data, key, Settings.separator)
 
-    def __setitem__(self, keypath: str, value: Any) -> Any:
+    def __setitem__(self, key: str, value: Any) -> Any:
         """Set item to new value or create it."""
         try:
-            self.__getitem__(keypath)
-            dpath.set(self.data, keypath, value, Settings.separator)
+            self[key]  # pylint: disable=pointless-statement
+            dpath.set(self.data, key, value, Settings.separator)
         except KeyError:
-            dpath.new(self.data, keypath, value, Settings.separator)
+            dpath.new(self.data, key, value, Settings.separator)
 
     def __repr__(self) -> str:
         """Retrun readable representation of settings."""
-        return f"{type(self).__name__}({repr(self.data)})"
+        template = Template('<$name: $data>')
+        return repr(
+            template.substitute(name=type(self).__name__, data=self.data)
+        )
 
-    def get(self, keypath: str, default: Optional[Any] = None) -> Any:
+    def get(self, key: str, default: Optional[Any] = None) -> Any:
         """Get item or return default."""
         try:
-            value = self.__getitem__(keypath)
+            value = self[key]
             return value
         except KeyError:
             return default
 
-    def pop(self, keypath: str, default: Optional[Any] = None) -> Any:
+    def pop(self, key: str, *default: Any) -> Any:
         """Get item and remove it from settings or return default."""
         try:
             # TODO: need to determine how dpath will handle list element here
-            value = self.__getitem__(keypath)
-            self.__delitem__(keypath)
+            value = self[key]
+            del self[key]
             return value
         except (KeyError, PathNotFound):
-            return default
+            return default[0]
 
     def lookup(
-        self, *args: str, default: Optional[Any] = None,
+        self,
+        *args: str,
+        default: Optional[Any] = None,
     ) -> Optional[Any]:
-        """Get value from settings from multiple keypaths."""
-        for keypath in args:
+        """Get value from settings from multiple keys."""
+        for key in args:
             try:
-                value = self.__getitem__(keypath)
+                value = self[key]
                 if value is not None:
-                    log.info(f"lookup found: {value} for {keypath}")
+                    log.info('lookup found: %s for %s', value, key)
                     return value
             except KeyError:
-                log.debug(f"lookup was unable to query: {keypath}")
-        log.debug(f"returning default for: {keypath}")
+                log.debug('lookup was unable to query: %s', key)
+            log.debug('returning default for: %s', key)
         return default
 
     def values(self, query: Optional[str] = None) -> Any:
         """Search settings matching query."""
         if query is None:
-            query = f"{Settings.separator}*"
+            template = Template('${separator}*')
+            query = template.substitute(separator=Settings.separator)
         return dpath.values(self.data, query, Settings.separator)
 
     # XXX: not sure if this should stay for dictionary
-    def append(self, keypath: str, value: Any) -> None:
-        """Append to a list located at keypath."""
+    def append(self, key: str, value: Any) -> None:
+        """Append to a list located at key."""
         store = [value]
-        for x in reversed(keypath.split(Settings.separator)):
-            if x != '':
-                store = {x: store}  # type: ignore
-        dpath.merge(self.data, store)
+        for subkey in reversed(key.split(Settings.separator)):
+            if subkey != '':
+                store = {subkey: store}  # type: ignore
+        dpath.merge(self.data, store)  # type: ignore
 
     # def update(self, other=(), /, **kwds: Any) -> None:
-    def update(  # type: ignore
-        self, other: Dict[str, Any], **kwargs: Any
+    def update(
+        self,
+        other: Union['SupportsKeysAndGetItem', Iterable[Tuple[Any, Any]]] = (),
+        /,
+        **kwargs: Any,
     ) -> None:
         """Update settings."""
-        dpath.merge(self.data, other, afilter=None, flags=2)
+        dpath.merge(
+            self.data,
+            other or kwargs,  # type: ignore
+            flags=2,
+        )
 
 
 class SettingsMap(ChainMap):
     """Manage layered settings loaded from confiugrations using dpath."""
 
     separator: str = '/'
 
@@ -139,86 +157,97 @@
     def push(self, data: Dict[str, Any]) -> None:
         """Push settings untop store."""
         logging.debug(data)
         self.maps.insert(0, data)
 
     # TODO: add capability to recursive search settings
 
-    def __delitem__(self, keypath: str) -> Any:
-        """Delete item at keypath."""
-        return dpath.delete(self.maps[0], keypath, SettingsMap.separator)
+    def __delitem__(self, key: str) -> Any:
+        """Delete item at key."""
+        return dpath.delete(self.maps[0], key, SettingsMap.separator)
 
-    def __getitem__(self, keypath: str) -> Any:
+    def __getitem__(self, key: str) -> Any:
         """Get item."""
         for mapping in self.maps:
             try:
-                return dpath.get(mapping, keypath, SettingsMap.separator)
+                return dpath.get(mapping, key, SettingsMap.separator)
             except KeyError:
                 pass
-        return self.__missing__(keypath)
+        return self.__missing__(key)
 
-    def __setitem__(self, keypath: str, value: Any) -> Any:
+    def __setitem__(self, key: str, value: Any) -> Any:
         """Set item to new value or create it."""
         try:
-            self.__getitem__(keypath)
-            dpath.set(self.maps[0], keypath, value, SettingsMap.separator)
+            self[key]  # pylint: disable=pointless-statement
+            dpath.set(self.maps[0], key, value, SettingsMap.separator)
         except KeyError:
-            dpath.new(self.maps[0], keypath, value, SettingsMap.separator)
+            dpath.new(self.maps[0], key, value, SettingsMap.separator)
 
-    def get(self, keypath: str, default: Optional[Any] = None) -> Any:
+    def get(self, key: str, default: Optional[Any] = None) -> Any:
         """Get item or return default."""
         try:
-            value = self.__getitem__(keypath)
+            value = self[key]
             return value
         except KeyError:
             return default
 
-    def pop(self, keypath: str, default: Optional[Any] = None) -> Any:
+    def pop(self, key: str, *default: Any) -> Any:
         """Get item and remove it from settings or return default."""
         try:
             # TODO: need to determine how dpath will handle list element here
-            value = self.__getitem__(keypath)
-            self.__delitem__(keypath)
+            value = self[key]
+            del self[key]
             return value
         except (KeyError, PathNotFound):
-            return default
+            # self.maps[0].pop(key, *args)
+            return default[0]
 
     def lookup(
-        self, *args: str, default: Optional[Any] = None,
+        self,
+        *args: str,
+        default: Optional[Any] = None,
     ) -> Optional[Any]:
-        """Get value from settings from multiple keypaths."""
-        for keypath in args:
+        """Get value from settings from multiple keys."""
+        for key in args:
             try:
-                value = self.__getitem__(keypath)
-                log.info(f"lookup found: {value} for {keypath}")
+                value = self[key]
+                log.info('lookup found: %s for %s', value, key)
                 return value
             except KeyError:
-                log.debug(f"lookup was unable to query: {keypath}")
-        log.debug(f"returning default for: {keypath}")
+                log.debug('lookup was unable to query: %s', key)
+            log.debug('returning default for: %s', key)
         return default
 
     # def values(self, query: Optional[str] = None) -> Dict[str, Any]:
     #     """Search settings matching query."""
     #     if query is None:
     #         query = f"{SettingsMap.separator}*"
     #     return dpath.values(self.maps[0], query, SettingsMap.separator)
 
-    # def append(self, keypath: str, value: Any) -> None:
-    #     """Append to a list located at keypath."""
+    # def append(self, key: str, value: Any) -> None:
+    #     """Append to a list located at key."""
     #     store = [value]
-    #     for x in reversed(keypath.split(SettingsMap.separator)):
+    #     for x in reversed(key.split(SettingsMap.separator)):
     #         if x != '':
     #             store = {x: store}  # type: ignore
     #     dpath.merge(self.maps[0], store)
 
-    def update(  # type: ignore
-        self, other: Dict[str, Any], **kwargs: Any
+    def update(
+        self,
+        other: Union['SupportsKeysAndGetItem', Iterable[Tuple[Any, Any]]] = (),
+        /,
+        **kwargs: Any,
     ) -> None:
         """Update settings."""
-        dpath.merge(self.maps[0], other, afilter=None, flags=2)
+        dpath.merge(
+            self.maps[0],
+            other or kwargs,  # type: ignore
+            afilter=None,  # type: ignore
+            flags=2,
+        )
 
 
 class SettingsProxy(MutableMapping):
     """Proxy to manage settings with environment variables."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initialize settings store."""
@@ -234,78 +263,80 @@
         self.data = SettingsMap(*args, **kwargs)
 
     @property
     def environs(self) -> Dict[str, Any]:
         """Get environs."""
         return self.__environs
 
-    def __delitem__(self, keypath: str) -> Any:
-        """Delete item at keypath."""
-        self.data.__delitem__(keypath)
+    def __delitem__(self, key: str) -> Any:
+        """Delete item at key."""
+        del self.data[key]
 
     def __getattr__(
         self, attr: str
     ) -> 'Callable[[VarArg(Any), KwArg(Any)], Any]':
         """Proxy calls to settings store."""
         if hasattr(self.__dict__.get('data'), attr):
 
             def wrapper(*args: Any, **kwargs: Any) -> Any:
                 """Call query for data store."""
                 return getattr(self.data, attr)(*args, **kwargs)
 
             return wrapper
         raise AttributeError(attr)
 
-    def __getitem__(self, keypath: str) -> Any:
+    def __getitem__(self, key: str) -> Any:
         """Get environment variable then mapped item."""
         try:
-            value = dpath.get(self.environs, keypath, Settings.separator)
+            value = dpath.get(self.environs, key, Settings.separator)
             return value
         except KeyError:
             pass
 
-        value = self.data.__getitem__(keypath)
+        value = self.data[key]
         return value
 
     def __iter__(self) -> Iterator[Any]:
         """Iterate settings dictionary."""
         return self.data.__iter__()
 
     def __len__(self) -> int:
         """Return number of settings items."""
         return self.data.__len__()
 
-    def __setitem__(self, keypath: str, value: Any) -> Any:
+    def __setitem__(self, key: str, value: Any) -> Any:
         """Set item to new value or create it."""
-        self.data.__setitem__(keypath, value)
+        self.data[key] = value
 
     def __repr__(self) -> str:
         """Retrun readable representation of settings."""
-        return self.data.__repr__()
+        return repr(self.data)
 
-    def get(self, keypath: str, default: Optional[Any] = None) -> Any:
+    def get(self, key: str, default: Optional[Any] = None) -> Any:
         """Get item or return default."""
         try:
-            value = self.__getitem__(keypath)
+            value = self[key]
             return value
         except KeyError:
             return default
 
     def lookup(
-        self, *args: str, default: Optional[Any] = None,
+        self,
+        *args: str,
+        default: Optional[Any] = None,
     ) -> Optional[Any]:
-        """Get value from settings from multiple keypaths."""
-        for keypath in args:
+        """Get value from settings from multiple keys."""
+        for key in args:
             try:
-                value = self.__getitem__(keypath)
-                log.info(f"lookup found: {value} for {keypath}")
+                value = self[key]
+                log.info('lookup found: %s for %s', value, key)
                 return value
             except KeyError:
-                log.debug(f"lookup was unable to query: {keypath}")
-        log.debug(f"returning default for: {keypath}")
+                log.debug('lookup was unable to query: %s', key)
+            log.debug('returning default for: %s', key)
         return default
 
     @classmethod
     def combine(
         cls, source: Dict[str, Any], update: Mapping[str, Any]
     ) -> Dict[str, Any]:
         """Perform recursive merge."""
@@ -314,32 +345,32 @@
                 source[k] = cls.combine(source.get(k, {}), v)
             else:
                 source[k] = v
         return source
 
     @staticmethod
     def to_dict(key: str, value: Any) -> Dict[str, Any]:
-        """Convert environment keypath to nested dictionary."""
+        """Convert environment key to nested dictionary."""
 
-        def expand(x: str) -> Dict[str, Any]:
+        def expand(keypath: str) -> Dict[str, Any]:
             """Convert key part to dictionary key."""
-            if '_' not in x:
-                return {x: value}
-            k, v = x.split('_', 1)
+            if '_' not in keypath:
+                return {keypath: value}
+            k, v = keypath.split('_', 1)
             return {k: expand(v)}
 
         return expand(key.lower())
 
     @staticmethod
     def load_dotenv() -> None:
         """Load environs from '.env' file."""
         # TODO: key/value should be added from dotenv regardless of prefix
         env_file = os.path.join(os.getcwd(), '.env')
         if os.path.exists(env_file):
-            with open(env_file) as env:
+            with open(env_file, encoding='utf-8') as env:
                 for line in env:
                     k, v = line.partition('=')[::2]
                     os.environ[k.strip().upper()] = str(v)
 
     def load_environs(self) -> Dict[str, Any]:
         """Load environment variables."""
         prefix = str(
```


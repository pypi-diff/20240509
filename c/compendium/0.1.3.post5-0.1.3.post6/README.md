# Comparing `tmp/compendium-0.1.3.post5.tar.gz` & `tmp/compendium-0.1.3.post6.tar.gz`

## Comparing `compendium-0.1.3.post5.tar` & `compendium-0.1.3.post6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.flake8
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/mkdocs.yml
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/versioning.tar.gz
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.github/workflows/docs.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/configuration.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/index.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/schema.md
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/settings.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/config_manager.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes_base.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/loader.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/paths.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/settings.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/json.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/toml.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/xml.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/docs/development/filetypes/yaml.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config.toml
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested_env.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/settings.md
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/settings.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/check.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/config_file.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/example-out.yaml
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/example.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/in.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/in.toml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/in.yaml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/out.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/out.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_file/out.yaml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/config1.toml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/config2.toml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/config_manager.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/config1.toml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/config2.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/example.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/multiconfig.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/prototype.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/read_write.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/config_manager/prototyping/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/hierarchial/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/hierarchial/config.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/hierarchial/config_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/marshmallow/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/pydantic/.keep
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/simple/example-out.yaml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/simple/example.yaml
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/dataclass/simple/example_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/hidden/.example
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/hidden/__init__.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/hidden/config.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/__init__.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman.py
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/proman-lock.json
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/proman-lock.json
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule1/proman-lock.json
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule1/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule2/proman-lock.json
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module1/submodule2/pyproject.toml
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module2/proman-lock.json
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/nested/proman/module2/pyproject.toml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/node.toml
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/tree.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/dry/node.toml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/dry/dehiscent/node.toml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/dry/indehiscent/node.toml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/node.toml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/berry/node.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/berry/hesperidium/node.toml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/drupe/node.toml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/examples/tree/succulant/pome/node.toml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/__init__.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/config_manager.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/exceptions.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filepaths.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/py.typed
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/settings.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/__init__.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/ini.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/json.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/toml.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/xml.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/src/compendium/filetypes/yaml.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/__init__.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/build.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/doc.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tasks/qa.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/__init__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/config.toml
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/test_config_manager.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/test_settings.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/test_version.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/test_filepaths.py.bak
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/settings1.toml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/settings2.toml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/settings3.toml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/hierarchy/test_hierarchy.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/fruit.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/fruit1.toml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/fruit2.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/filepaths/tree/test_tree.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/ini/config.ini
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/ini/test_ini.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/json/config.json
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/json/test_json.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/module/config.toml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/toml/config.toml
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/toml/test_toml.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/xml/config.xml
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/xml/test_xml.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/yaml/config.yaml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/tests/yaml/test_yaml.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/LICENSE
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/README.md
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/pyproject.toml
--rw-r--r--   0        0        0    19600 2020-02-02 00:00:00.000000 compendium-0.1.3.post5/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/.flake8
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/mkdocs.yml
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/versioning.tar.gz
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/configuration.md
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/index.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/schema.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/settings.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/config_manager.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/filetypes.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/loader.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/paths.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/settings.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/filetypes/json.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/filetypes/toml.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/filetypes/xml.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/docs/development/filetypes/yaml.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config.toml
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested_env.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/settings.md
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/settings.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/check.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/config_file.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/example-out.yaml
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/example.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/in.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/in.toml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/in.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/out.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/out.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_file/out.yaml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/config1.toml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/config2.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/config_manager.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/config1.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/config2.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/example.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/multiconfig.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/prototype.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/read_write.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/config_manager/prototyping/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/hierarchial/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/hierarchial/config.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/hierarchial/config_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/marshmallow/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/pydantic/.keep
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/simple/example-out.yaml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/simple/example.yaml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/dataclass/simple/example_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/hidden/.example
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/hidden/__init__.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/hidden/config.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/__init__.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman.py
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/proman-lock.json
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module1/proman-lock.json
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module1/submodule1/proman-lock.json
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module1/submodule1/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module1/submodule2/proman-lock.json
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module1/submodule2/pyproject.toml
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module2/proman-lock.json
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/nested/proman/module2/pyproject.toml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/node.toml
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/tree.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/dry/node.toml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/dry/dehiscent/node.toml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/dry/indehiscent/node.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/succulant/node.toml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/succulant/berry/node.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/succulant/berry/hesperidium/node.toml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/succulant/drupe/node.toml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/examples/tree/succulant/pome/node.toml
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/__init__.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/config_manager.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/exceptions.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filepaths.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/py.typed
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/settings.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filetypes/__init__.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filetypes/ini.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filetypes/json.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filetypes/toml.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filetypes/xml.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/src/compendium/filetypes/yaml.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tasks/__init__.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tasks/build.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tasks/doc.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tasks/qa.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/config.toml
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/test_config_manager.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/test_settings.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/test_version.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/test_filepaths.py.bak
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/hierarchy/settings1.toml
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/hierarchy/settings2.toml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/hierarchy/settings3.toml
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/hierarchy/test_hierarchy.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/tree/fruit.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/tree/fruit1.toml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/tree/fruit2.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/filepaths/tree/test_tree.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/ini/config.ini
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/ini/test_ini.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/json/config.json
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/json/test_json.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/module/config.toml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/toml/config.toml
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/toml/test_toml.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/xml/config.xml
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/xml/test_xml.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/yaml/config.yaml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/tests/yaml/test_yaml.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/LICENSE
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/README.md
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/pyproject.toml
+-rw-r--r--   0        0        0    19597 2020-02-02 00:00:00.000000 compendium-0.1.3.post6/PKG-INFO
```

### Comparing `compendium-0.1.3.post5/mkdocs.yml` & `compendium-0.1.3.post6/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
   - Schema: schema.md
   - Settings: settings.md
   - Development:
     - Config Manager: development/config_manager.md
     - Paths: development/paths.md
     - Settings: development/settings.md
     - Loader: development/loader.md
-    - Filetypes Base: development/filetypes_base.md
+    - Filetypes Base: development/filetypes.md
     - Filetypes:
       - Json: development/filetypes/json.md
       - Toml: development/filetypes/toml.md
       - Xml: development/filetypes/xml.md
       - Yaml: development/filetypes/yaml.md
```

### Comparing `compendium-0.1.3.post5/.github/workflows/ci.yml` & `compendium-0.1.3.post6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/.github/workflows/docs.yml` & `compendium-0.1.3.post6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/docs/configuration.md` & `compendium-0.1.3.post6/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/docs/settings.md` & `compendium-0.1.3.post6/docs/settings.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config.toml` & `compendium-0.1.3.post6/examples/config.toml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/nested_env.py` & `compendium-0.1.3.post6/examples/nested_env.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/settings.md` & `compendium-0.1.3.post6/examples/settings.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/settings.py` & `compendium-0.1.3.post6/examples/settings.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config_file/config_file.py` & `compendium-0.1.3.post6/examples/config_file/config_file.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config_manager/config_manager.py` & `compendium-0.1.3.post6/examples/config_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config_manager/prototyping/multiconfig.py` & `compendium-0.1.3.post6/examples/config_manager/prototyping/multiconfig.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config_manager/prototyping/prototype.py` & `compendium-0.1.3.post6/examples/config_manager/prototyping/prototype.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config_manager/prototyping/read_write.py` & `compendium-0.1.3.post6/examples/config_manager/prototyping/read_write.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/config_manager/prototyping/simple.py` & `compendium-0.1.3.post6/examples/config_manager/prototyping/simple.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/dataclass/hierarchial/config_file.py` & `compendium-0.1.3.post6/examples/dataclass/hierarchial/config_file.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/dataclass/simple/example_config.py` & `compendium-0.1.3.post6/examples/dataclass/simple/example_config.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/hidden/config.py` & `compendium-0.1.3.post6/examples/hidden/config.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/nested/proman.py` & `compendium-0.1.3.post6/examples/nested/proman.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/examples/tree/tree.py` & `compendium-0.1.3.post6/examples/tree/tree.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/__init__.py` & `compendium-0.1.3.post6/src/compendium/__init__.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/config_manager.py` & `compendium-0.1.3.post6/src/compendium/config_manager.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/exceptions.py` & `compendium-0.1.3.post6/src/compendium/exceptions.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filepaths.py` & `compendium-0.1.3.post6/src/compendium/filepaths.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/loader.py` & `compendium-0.1.3.post6/src/compendium/loader.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/settings.py` & `compendium-0.1.3.post6/src/compendium/settings.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filetypes/__init__.py` & `compendium-0.1.3.post6/src/compendium/filetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filetypes/ini.py` & `compendium-0.1.3.post6/src/compendium/filetypes/ini.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filetypes/json.py` & `compendium-0.1.3.post6/src/compendium/filetypes/json.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filetypes/toml.py` & `compendium-0.1.3.post6/src/compendium/filetypes/toml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filetypes/xml.py` & `compendium-0.1.3.post6/src/compendium/filetypes/xml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/src/compendium/filetypes/yaml.py` & `compendium-0.1.3.post6/src/compendium/filetypes/yaml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tasks/build.py` & `compendium-0.1.3.post6/tasks/build.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tasks/doc.py` & `compendium-0.1.3.post6/tasks/doc.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tasks/qa.py` & `compendium-0.1.3.post6/tasks/qa.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/config.toml` & `compendium-0.1.3.post6/tests/config.toml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/test_config_manager.py` & `compendium-0.1.3.post6/tests/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/test_settings.py` & `compendium-0.1.3.post6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/filepaths/test_filepaths.py.bak` & `compendium-0.1.3.post6/tests/filepaths/test_filepaths.py.bak`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/filepaths/hierarchy/test_hierarchy.py` & `compendium-0.1.3.post6/tests/filepaths/hierarchy/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/filepaths/tree/test_tree.py` & `compendium-0.1.3.post6/tests/filepaths/tree/test_tree.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/ini/test_ini.py` & `compendium-0.1.3.post6/tests/ini/test_ini.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/json/test_json.py` & `compendium-0.1.3.post6/tests/json/test_json.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/module/config.toml` & `compendium-0.1.3.post6/tests/module/config.toml`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/toml/test_toml.py` & `compendium-0.1.3.post6/tests/toml/test_toml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/xml/test_xml.py` & `compendium-0.1.3.post6/tests/xml/test_xml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/tests/yaml/test_yaml.py` & `compendium-0.1.3.post6/tests/yaml/test_yaml.py`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/.gitignore` & `compendium-0.1.3.post6/.gitignore`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/LICENSE` & `compendium-0.1.3.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/README.md` & `compendium-0.1.3.post6/README.md`

 * *Files identical despite different names*

### Comparing `compendium-0.1.3.post5/pyproject.toml` & `compendium-0.1.3.post6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "compendium"
-version = "0.1.3.post5"
+version = "0.1.3.post6"
 description = "Simple layered configuraion tool"
 authors = [{name="Jesse P. Johnson", email="jpj6652@gmail.com"}]
 maintainers = [{name="Jesse P. Johnson", email="jpj6652@gmail.com"}]
 requires-python = ">=3.6.2"
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["configuration", "configuration management"]
@@ -56,19 +56,19 @@
     "pylint>=2.9.5",
     "bandit>=1.6.2",
     "safety>=2.2.0",
     "mypy>=1",
     "mypy-extensions>=0.4.3"
 ]
 docs = [
-    "mkdocs>=1.1.2,<2",
-    "pydocstyle[toml]>=6.1.1,<7",
-    "mkdocstrings>=0.12.1,<1",
-    "mkdocs-material>=7.1.2,<8",
-    "docstr-coverage>=1.2.0,<2"
+    "docstr-coverage>=1.2.0,<2",
+    "mkdocs>=1.2.2,<2",
+    "mkdocs-material>=9,<10",
+    "mkdocstrings[python]>=1,<2",
+    "pydocstyle[toml]>=6.1.1"
 ]
 
 [project.urls]
 homepage = "https://github.com/kuwv/python-compendium"
 documentation = "https://kuwv.github.io/python-compendium"
 
 [[tool.proman.versioning.files]]
```

### Comparing `compendium-0.1.3.post5/PKG-INFO` & `compendium-0.1.3.post6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: compendium
-Version: 0.1.3.post5
+Version: 0.1.3.post6
 Summary: Simple layered configuraion tool
 Project-URL: homepage, https://github.com/kuwv/python-compendium
 Project-URL: documentation, https://kuwv.github.io/python-compendium
 Author-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 Maintainer-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -242,18 +242,18 @@
 Requires-Dist: pyfakefs>=5.4.1; extra == 'dev'
 Requires-Dist: pylint>=2.9.5; extra == 'dev'
 Requires-Dist: pytest-cov>=2.9.0; extra == 'dev'
 Requires-Dist: pytest>=6.2.5; extra == 'dev'
 Requires-Dist: safety>=2.2.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: docstr-coverage<2,>=1.2.0; extra == 'docs'
-Requires-Dist: mkdocs-material<8,>=7.1.2; extra == 'docs'
-Requires-Dist: mkdocs<2,>=1.1.2; extra == 'docs'
-Requires-Dist: mkdocstrings<1,>=0.12.1; extra == 'docs'
-Requires-Dist: pydocstyle[toml]<7,>=6.1.1; extra == 'docs'
+Requires-Dist: mkdocs-material<10,>=9; extra == 'docs'
+Requires-Dist: mkdocs<2,>=1.2.2; extra == 'docs'
+Requires-Dist: mkdocstrings[python]<2,>=1; extra == 'docs'
+Requires-Dist: pydocstyle[toml]>=6.1.1; extra == 'docs'
 Provides-Extra: xml
 Requires-Dist: xmltodict<1,>=0.12.0; extra == 'xml'
 Description-Content-Type: text/markdown
 
 # Compendium
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```


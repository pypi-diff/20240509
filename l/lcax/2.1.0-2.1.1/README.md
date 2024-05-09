# Comparing `tmp/lcax-2.1.0.tar.gz` & `tmp/lcax-2.1.1.tar.gz`

## Comparing `lcax-2.1.0.tar` & `lcax-2.1.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0     1001      127      589 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/Cargo.toml
--rw-r--r--   0     1001      127    20171 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/country.rs
--rw-r--r--   0     1001      127     1391 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/dates.rs
--rw-r--r--   0     1001      127       47 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/lib.rs
--rw-r--r--   0     1001      127      686 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/utils.rs
--rw-r--r--   0     1001      127     1524 2024-05-09 11:06:46.000000 lcax-2.1.0/README.md
--rw-r--r--   0     1001      127     1135 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/Cargo.toml
--rw-r--r--   0     1001      127      967 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/assembly.rs
--rw-r--r--   0     1001      127     3310 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/epd.rs
--rw-r--r--   0     1001      127      124 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/lib.rs
--rw-r--r--   0     1001      127     5764 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/life_cycle_base.rs
--rw-r--r--   0     1001      127     1967 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/product.rs
--rw-r--r--   0     1001      127     7181 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/project.rs
--rw-r--r--   0     1001      127     1295 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/shared.rs
--rw-r--r--   0     1001      127     1331 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/techflow.rs
--rw-r--r--   0     1001      127      147 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/tests/test_epd.rs
--rw-r--r--   0     1001      127      168 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/tests/test_project.rs
--rw-r--r--   0     1001      127      180 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/tests/test_techflow.rs
--rw-r--r--   0     1001      127      845 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/Cargo.toml
--rw-r--r--   0     1001      127     5582 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/ilcd/ilcd.rs
--rw-r--r--   0     1001      127       29 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/ilcd/mod.rs
--rw-r--r--   0     1001      127    16269 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/ilcd/parse.rs
--rw-r--r--   0     1001      127     4042 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/categories.rs
--rw-r--r--   0     1001      127     2045 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/edges.rs
--rw-r--r--   0     1001      127       70 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/mod.rs
--rw-r--r--   0     1001      127     8325 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/nodes.rs
--rw-r--r--   0     1001      127    13236 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/parse.rs
--rw-r--r--   0     1001      127     1788 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/results.rs
--rw-r--r--   0     1001      127       45 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lib.rs
--rw-r--r--   0     1001      127       30 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/slice/mod.rs
--rw-r--r--   0     1001      127    13484 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/slice/model.rs
--rw-r--r--   0     1001      127     5871 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/slice/parse.rs
--rw-r--r--   0     1001      127      262 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/convert_tests.rs
--rw-r--r--   0     1001      127    64785 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
--rw-r--r--   0     1001      127    68643 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
--rw-r--r--   0     1001      127    81962 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
--rw-r--r--   0     1001      127    70431 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
--rw-r--r--   0     1001      127    70200 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
--rw-r--r--   0     1001      127    84820 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
--rw-r--r--   0     1001      127    50733 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
--rw-r--r--   0     1001      127    80754 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
--rw-r--r--   0     1001      127   102497 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
--rw-r--r--   0     1001      127   111759 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
--rw-r--r--   0     1001      127    87077 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
--rw-r--r--   0     1001      127   100644 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
--rw-r--r--   0     1001      127    52735 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
--rwxr-xr-x   0     1001      127    69619 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
--rwxr-xr-x   0     1001      127    47820 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
--rw-r--r--   0     1001      127     4623 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/test_parse_ilcd.rs
--rw-r--r--   0     1001      127     2779 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
--rw-r--r--   0     1001      127    25028 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
--rw-r--r--   0     1001      127  2051524 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
--rw-r--r--   0     1001      127    13935 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127     1961 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
--rw-r--r--   0     1001      127     2157 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
--rw-r--r--   0     1001      127      133 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
--rw-r--r--   0     1001      127      905 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/slice/test_parse_slice.rs
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.1.0/modules/lcax/Cargo.toml
--rw-r--r--   0     1001      127     1505 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/javascript.rs
--rw-r--r--   0     1001      127      113 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/lib.rs
--rw-r--r--   0     1001      127     1551 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/python.rs
--rw-r--r--   0     1001      127      859 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/rust.rs
--rw-r--r--   0     1001      127      246 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/schemars.rs
--rw-r--r--   0     1001      127    35772 2024-05-09 11:06:48.000000 lcax-2.1.0/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.1.0/Cargo.toml
--rw-r--r--   0     1001      127     1441 2024-05-09 11:06:47.000000 lcax-2.1.0/pyproject.toml
--rw-r--r--   0     1001      127     2825 2024-05-09 11:06:47.000000 lcax-2.1.0/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      127      407 2024-05-09 11:06:47.000000 lcax-2.1.0/packages/python/src/lcax/lcax.pyi
--rw-r--r--   0     1001      127    15323 2024-05-09 11:06:49.000000 lcax-2.1.0/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      127    10173 2024-05-09 11:06:46.000000 lcax-2.1.0/LICENSE
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.1.0/PKG-INFO
+-rw-r--r--   0     1001      127     1135 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/Cargo.toml
+-rw-r--r--   0     1001      127      967 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/assembly.rs
+-rw-r--r--   0     1001      127     3380 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/epd.rs
+-rw-r--r--   0     1001      127      124 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/lib.rs
+-rw-r--r--   0     1001      127     5764 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/life_cycle_base.rs
+-rw-r--r--   0     1001      127     1996 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/product.rs
+-rw-r--r--   0     1001      127     7181 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/project.rs
+-rw-r--r--   0     1001      127     1330 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/shared.rs
+-rw-r--r--   0     1001      127     1331 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/src/techflow.rs
+-rw-r--r--   0     1001      127      147 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/tests/test_epd.rs
+-rw-r--r--   0     1001      127      168 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/tests/test_project.rs
+-rw-r--r--   0     1001      127      180 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/models/tests/test_techflow.rs
+-rw-r--r--   0     1001      127     1524 2024-05-09 11:30:34.000000 lcax-2.1.1/README.md
+-rw-r--r--   0     1001      127      845 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/Cargo.toml
+-rw-r--r--   0     1001      127     5582 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/ilcd/ilcd.rs
+-rw-r--r--   0     1001      127       29 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/ilcd/mod.rs
+-rw-r--r--   0     1001      127    16269 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/ilcd/parse.rs
+-rw-r--r--   0     1001      127     4042 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lcabyg/categories.rs
+-rw-r--r--   0     1001      127     2045 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lcabyg/edges.rs
+-rw-r--r--   0     1001      127       70 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lcabyg/mod.rs
+-rw-r--r--   0     1001      127     8325 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lcabyg/nodes.rs
+-rw-r--r--   0     1001      127    13236 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lcabyg/parse.rs
+-rw-r--r--   0     1001      127     1788 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lcabyg/results.rs
+-rw-r--r--   0     1001      127       45 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/lib.rs
+-rw-r--r--   0     1001      127       30 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/slice/mod.rs
+-rw-r--r--   0     1001      127    13484 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/slice/model.rs
+-rw-r--r--   0     1001      127     5871 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/src/slice/parse.rs
+-rw-r--r--   0     1001      127      262 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/convert_tests.rs
+-rw-r--r--   0     1001      127    64785 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
+-rw-r--r--   0     1001      127    68643 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
+-rw-r--r--   0     1001      127    81962 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
+-rw-r--r--   0     1001      127    70431 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
+-rw-r--r--   0     1001      127    70200 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
+-rw-r--r--   0     1001      127    84820 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
+-rw-r--r--   0     1001      127    50733 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
+-rw-r--r--   0     1001      127    80754 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
+-rw-r--r--   0     1001      127   102497 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
+-rw-r--r--   0     1001      127   111759 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
+-rw-r--r--   0     1001      127    87077 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
+-rw-r--r--   0     1001      127   100644 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
+-rw-r--r--   0     1001      127    52735 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
+-rwxr-xr-x   0     1001      127    69619 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rwxr-xr-x   0     1001      127    47820 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
+-rw-r--r--   0     1001      127     4623 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/ilcd/test_parse_ilcd.rs
+-rw-r--r--   0     1001      127     2779 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
+-rw-r--r--   0     1001      127    25028 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
+-rw-r--r--   0     1001      127  2051524 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
+-rw-r--r--   0     1001      127    13935 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127     1961 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
+-rw-r--r--   0     1001      127     2157 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
+-rw-r--r--   0     1001      127      133 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
+-rw-r--r--   0     1001      127      905 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/convert/tests/slice/test_parse_slice.rs
+-rw-r--r--   0     1001      127      589 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/core/Cargo.toml
+-rw-r--r--   0     1001      127    20171 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/core/src/country.rs
+-rw-r--r--   0     1001      127     1391 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/core/src/dates.rs
+-rw-r--r--   0     1001      127       47 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/core/src/lib.rs
+-rw-r--r--   0     1001      127      686 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/core/src/utils.rs
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.1.1/modules/lcax/Cargo.toml
+-rw-r--r--   0     1001      127     1505 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/lcax/src/javascript.rs
+-rw-r--r--   0     1001      127      113 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/lcax/src/lib.rs
+-rw-r--r--   0     1001      127     1551 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/lcax/src/python.rs
+-rw-r--r--   0     1001      127      859 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/lcax/src/rust.rs
+-rw-r--r--   0     1001      127      246 2024-05-09 11:30:34.000000 lcax-2.1.1/modules/lcax/src/schemars.rs
+-rw-r--r--   0     1001      127    35772 2024-05-09 11:30:35.000000 lcax-2.1.1/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     1441 2024-05-09 11:30:34.000000 lcax-2.1.1/pyproject.toml
+-rw-r--r--   0     1001      127     2825 2024-05-09 11:30:34.000000 lcax-2.1.1/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      127      407 2024-05-09 11:30:34.000000 lcax-2.1.1/packages/python/src/lcax/lcax.pyi
+-rw-r--r--   0     1001      127    15319 2024-05-09 11:30:36.000000 lcax-2.1.1/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      127    10173 2024-05-09 11:30:34.000000 lcax-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.1.1/PKG-INFO
```

### Comparing `lcax-2.1.0/modules/core/Cargo.toml` & `lcax-2.1.1/modules/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/core/src/country.rs` & `lcax-2.1.1/modules/core/src/country.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/core/src/dates.rs` & `lcax-2.1.1/modules/core/src/dates.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/core/src/utils.rs` & `lcax-2.1.1/modules/core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/README.md` & `lcax-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/models/Cargo.toml` & `lcax-2.1.1/modules/models/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/models/src/assembly.rs` & `lcax-2.1.1/modules/models/src/assembly.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/models/src/epd.rs` & `lcax-2.1.1/modules/models/src/epd.rs`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             impacts: Default::default(),
             meta_data: None,
         }
     }
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
+#[serde(rename_all = "lowercase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub enum Standard {
     EN15804A1,
     EN15804A2,
     UNKNOWN,
 }
 
@@ -86,14 +87,15 @@
         } else {
             Standard::UNKNOWN
         }
     }
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
+#[serde(rename_all = "lowercase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub enum SubType {
     Generic,
     Specific,
     Industry,
     Representative,
 }
```

### Comparing `lcax-2.1.0/modules/models/src/life_cycle_base.rs` & `lcax-2.1.1/modules/models/src/life_cycle_base.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/models/src/product.rs` & `lcax-2.1.1/modules/models/src/product.rs`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     pub transport_epd: ImpactDataSource,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub enum ImpactDataSource {
+    #[serde(rename = "EPD")]
     EPD(EPD),
     TechFlow(TechFlow),
     ExternalImpactData(ExternalImpactData),
     InternalImpactData(InternalImpactData),
 }
 
 impl Default for ImpactDataSource {
```

### Comparing `lcax-2.1.0/modules/models/src/project.rs` & `lcax-2.1.1/modules/models/src/project.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/models/src/shared.rs` & `lcax-2.1.1/modules/models/src/shared.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use schemars::JsonSchema;
 use serde::{Deserialize, Serialize};
 
 #[cfg(feature = "jsbindings")]
 use tsify::Tsify;
 
 #[derive(Debug, Deserialize, Serialize, JsonSchema, Clone)]
+#[serde(rename_all = "lowercase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub enum Unit {
     M,
     M2,
     M3,
     KG,
     TONES,
```

### Comparing `lcax-2.1.0/modules/models/src/techflow.rs` & `lcax-2.1.1/modules/models/src/techflow.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/Cargo.toml` & `lcax-2.1.1/modules/convert/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/ilcd/ilcd.rs` & `lcax-2.1.1/modules/convert/src/ilcd/ilcd.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/ilcd/parse.rs` & `lcax-2.1.1/modules/convert/src/ilcd/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/lcabyg/categories.rs` & `lcax-2.1.1/modules/convert/src/lcabyg/categories.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/lcabyg/edges.rs` & `lcax-2.1.1/modules/convert/src/lcabyg/edges.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/lcabyg/nodes.rs` & `lcax-2.1.1/modules/convert/src/lcabyg/nodes.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/lcabyg/parse.rs` & `lcax-2.1.1/modules/convert/src/lcabyg/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/lcabyg/results.rs` & `lcax-2.1.1/modules/convert/src/lcabyg/results.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/slice/model.rs` & `lcax-2.1.1/modules/convert/src/slice/model.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/src/slice/parse.rs` & `lcax-2.1.1/modules/convert/src/slice/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json` & `lcax-2.1.1/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/ilcd/test_parse_ilcd.rs` & `lcax-2.1.1/modules/convert/tests/ilcd/test_parse_ilcd.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json` & `lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json` & `lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json` & `lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json` & `lcax-2.1.1/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg.rs` & `lcax-2.1.1/modules/convert/tests/lcabyg/test_parse_lcabyg.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs` & `lcax-2.1.1/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/convert/tests/slice/test_parse_slice.rs` & `lcax-2.1.1/modules/convert/tests/slice/test_parse_slice.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/lcax/Cargo.toml` & `lcax-2.1.1/modules/lcax/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/lcax/src/javascript.rs` & `lcax-2.1.1/modules/lcax/src/javascript.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/lcax/src/python.rs` & `lcax-2.1.1/modules/lcax/src/python.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/modules/lcax/src/rust.rs` & `lcax-2.1.1/modules/lcax/src/rust.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/Cargo.lock` & `lcax-2.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "lcax"
-version = "2.1.0"
+version = "2.1.1"
 dependencies = [
  "console_error_panic_hook",
  "getrandom",
  "lcax_convert",
  "lcax_core",
  "lcax_models",
  "pyo3",
@@ -380,15 +380,15 @@
  "tsify",
  "wasm-bindgen",
  "wee_alloc",
 ]
 
 [[package]]
 name = "lcax_convert"
-version = "2.1.0"
+version = "2.1.1"
 dependencies = [
  "bytes",
  "chrono",
  "field_access",
  "lcax_core",
  "lcax_models",
  "parquet",
@@ -396,27 +396,27 @@
  "serde",
  "serde_json",
  "uuid",
 ]
 
 [[package]]
 name = "lcax_core"
-version = "2.1.0"
+version = "2.1.1"
 dependencies = [
  "chrono",
  "pkg-version",
  "rust_iso3166",
  "schemars",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "lcax_models"
-version = "2.1.0"
+version = "2.1.1"
 dependencies = [
  "chrono",
  "console_error_panic_hook",
  "lcax_core",
  "pyo3",
  "schemars",
  "serde",
```

### Comparing `lcax-2.1.0/pyproject.toml` & `lcax-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/packages/python/src/lcax/__init__.py` & `lcax-2.1.1/packages/python/src/lcax/__init__.py`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/packages/python/src/lcax/pydantic.py` & `lcax-2.1.1/packages/python/src/lcax/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,38 +442,38 @@
         populate_by_name=True,
     )
     name: str
     url: Optional[str] = None
 
 
 class Standard(Enum):
-    EN15804_A1 = 'EN15804A1'
-    EN15804_A2 = 'EN15804A2'
-    UNKNOWN = 'UNKNOWN'
+    EN15804A1 = 'en15804a1'
+    EN15804A2 = 'en15804a2'
+    UNKNOWN = 'unknown'
 
 
 class SubType(Enum):
-    GENERIC = 'Generic'
-    SPECIFIC = 'Specific'
-    INDUSTRY = 'Industry'
-    REPRESENTATIVE = 'Representative'
+    GENERIC = 'generic'
+    SPECIFIC = 'specific'
+    INDUSTRY = 'industry'
+    REPRESENTATIVE = 'representative'
 
 
 class Unit(Enum):
-    M = 'M'
-    M2 = 'M2'
-    M3 = 'M3'
-    KG = 'KG'
-    TONES = 'TONES'
-    PCS = 'PCS'
-    L = 'L'
-    M2_R1 = 'M2R1'
-    KM = 'KM'
-    TONES_KM = 'TONES_KM'
-    UNKNOWN = 'UNKNOWN'
+    M = 'm'
+    M2 = 'm2'
+    M3 = 'm3'
+    KG = 'kg'
+    TONES = 'tones'
+    PCS = 'pcs'
+    L = 'l'
+    M2R1 = 'm2r1'
+    KM = 'km'
+    TONES_KM = 'tones_km'
+    UNKNOWN = 'unknown'
 
 
 class ValueUnit(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     unit: Unit
@@ -560,15 +560,15 @@
 
 
 class ImpactDataSource1(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    e_pd: EPD = Field(..., alias='ePD')
+    epd: EPD = Field(..., alias='EPD')
 
 
 class ImpactDataSource4(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
```

### Comparing `lcax-2.1.0/LICENSE` & `lcax-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-2.1.0/PKG-INFO` & `lcax-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lcax
-Version: 2.1.0
+Version: 2.1.1
 Requires-Dist: cffi
 Requires-Dist: pydantic >2.0.0
 Requires-Dist: mkdocs-material >=8.1.4, <9.0.0 ; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1, <2.0.0 ; extra == 'doc'
 Requires-Dist: datamodel-code-generator ; extra == 'codegen'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-datafixtures ; extra == 'tests'
```


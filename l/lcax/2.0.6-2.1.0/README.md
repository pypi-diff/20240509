# Comparing `tmp/lcax-2.0.6.tar.gz` & `tmp/lcax-2.1.0.tar.gz`

## Comparing `lcax-2.0.6.tar` & `lcax-2.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0     1001      127      845 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/Cargo.toml
--rw-r--r--   0     1001      127     5582 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/ilcd/ilcd.rs
--rw-r--r--   0     1001      127       29 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/ilcd/mod.rs
--rw-r--r--   0     1001      127    16269 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/ilcd/parse.rs
--rw-r--r--   0     1001      127     4042 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/categories.rs
--rw-r--r--   0     1001      127     2045 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/edges.rs
--rw-r--r--   0     1001      127       70 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/mod.rs
--rw-r--r--   0     1001      127     8325 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/nodes.rs
--rw-r--r--   0     1001      127    13236 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/parse.rs
--rw-r--r--   0     1001      127     1788 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/results.rs
--rw-r--r--   0     1001      127       45 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lib.rs
--rw-r--r--   0     1001      127       30 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/slice/mod.rs
--rw-r--r--   0     1001      127    13484 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/slice/model.rs
--rw-r--r--   0     1001      127     5871 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/slice/parse.rs
--rw-r--r--   0     1001      127      262 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/convert_tests.rs
--rw-r--r--   0     1001      127    64785 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
--rw-r--r--   0     1001      127    68643 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
--rw-r--r--   0     1001      127    81962 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
--rw-r--r--   0     1001      127    70431 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
--rw-r--r--   0     1001      127    70200 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
--rw-r--r--   0     1001      127    84820 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
--rw-r--r--   0     1001      127    50733 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
--rw-r--r--   0     1001      127    80754 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
--rw-r--r--   0     1001      127   102497 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
--rw-r--r--   0     1001      127   111759 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
--rw-r--r--   0     1001      127    87077 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
--rw-r--r--   0     1001      127   100644 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
--rw-r--r--   0     1001      127    52735 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
--rwxr-xr-x   0     1001      127    69619 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
--rwxr-xr-x   0     1001      127    47820 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
--rw-r--r--   0     1001      127     4623 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/test_parse_ilcd.rs
--rw-r--r--   0     1001      127     2779 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
--rw-r--r--   0     1001      127    25028 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
--rw-r--r--   0     1001      127  2051524 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
--rw-r--r--   0     1001      127    13935 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127     1961 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
--rw-r--r--   0     1001      127     2157 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
--rw-r--r--   0     1001      127      133 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
--rw-r--r--   0     1001      127      905 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/convert/tests/slice/test_parse_slice.rs
--rw-r--r--   0     1001      127     1524 2024-05-09 10:05:05.000000 lcax-2.0.6/README.md
--rw-r--r--   0     1001      127     1135 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/Cargo.toml
--rw-r--r--   0     1001      127      967 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/assembly.rs
--rw-r--r--   0     1001      127     4080 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/epd.rs
--rw-r--r--   0     1001      127      124 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/lib.rs
--rw-r--r--   0     1001      127     5764 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/life_cycle_base.rs
--rw-r--r--   0     1001      127     1967 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/product.rs
--rw-r--r--   0     1001      127     7201 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/project.rs
--rw-r--r--   0     1001      127     1295 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/shared.rs
--rw-r--r--   0     1001      127     1296 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/techflow.rs
--rw-r--r--   0     1001      127      147 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/tests/test_epd.rs
--rw-r--r--   0     1001      127      168 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/tests/test_project.rs
--rw-r--r--   0     1001      127      180 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/tests/test_techflow.rs
--rw-r--r--   0     1001      127      589 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/Cargo.toml
--rw-r--r--   0     1001      127    20171 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/country.rs
--rw-r--r--   0     1001      127     1391 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/dates.rs
--rw-r--r--   0     1001      127       47 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/lib.rs
--rw-r--r--   0     1001      127      686 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/utils.rs
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.0.6/modules/lcax/Cargo.toml
--rw-r--r--   0     1001      127     1505 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/javascript.rs
--rw-r--r--   0     1001      127      113 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/lib.rs
--rw-r--r--   0     1001      127     1551 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/python.rs
--rw-r--r--   0     1001      127      859 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/rust.rs
--rw-r--r--   0     1001      127      246 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/schemars.rs
--rw-r--r--   0     1001      127    35772 2024-05-09 10:05:07.000000 lcax-2.0.6/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.0.6/Cargo.toml
--rw-r--r--   0     1001      127     1441 2024-05-09 10:05:06.000000 lcax-2.0.6/pyproject.toml
--rw-r--r--   0     1001      127     2825 2024-05-09 10:05:06.000000 lcax-2.0.6/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      127      407 2024-05-09 10:05:06.000000 lcax-2.0.6/packages/python/src/lcax/lcax.pyi
--rw-r--r--   0     1001      127    14795 2024-05-09 10:05:08.000000 lcax-2.0.6/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      127    10173 2024-05-09 10:05:05.000000 lcax-2.0.6/LICENSE
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.0.6/PKG-INFO
+-rw-r--r--   0     1001      127      589 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/Cargo.toml
+-rw-r--r--   0     1001      127    20171 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/country.rs
+-rw-r--r--   0     1001      127     1391 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/dates.rs
+-rw-r--r--   0     1001      127       47 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/lib.rs
+-rw-r--r--   0     1001      127      686 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/core/src/utils.rs
+-rw-r--r--   0     1001      127     1524 2024-05-09 11:06:46.000000 lcax-2.1.0/README.md
+-rw-r--r--   0     1001      127     1135 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/Cargo.toml
+-rw-r--r--   0     1001      127      967 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/assembly.rs
+-rw-r--r--   0     1001      127     3310 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/epd.rs
+-rw-r--r--   0     1001      127      124 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/lib.rs
+-rw-r--r--   0     1001      127     5764 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/life_cycle_base.rs
+-rw-r--r--   0     1001      127     1967 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/product.rs
+-rw-r--r--   0     1001      127     7181 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/project.rs
+-rw-r--r--   0     1001      127     1295 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/shared.rs
+-rw-r--r--   0     1001      127     1331 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/src/techflow.rs
+-rw-r--r--   0     1001      127      147 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/tests/test_epd.rs
+-rw-r--r--   0     1001      127      168 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/tests/test_project.rs
+-rw-r--r--   0     1001      127      180 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/models/tests/test_techflow.rs
+-rw-r--r--   0     1001      127      845 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/Cargo.toml
+-rw-r--r--   0     1001      127     5582 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/ilcd/ilcd.rs
+-rw-r--r--   0     1001      127       29 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/ilcd/mod.rs
+-rw-r--r--   0     1001      127    16269 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/ilcd/parse.rs
+-rw-r--r--   0     1001      127     4042 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/categories.rs
+-rw-r--r--   0     1001      127     2045 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/edges.rs
+-rw-r--r--   0     1001      127       70 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/mod.rs
+-rw-r--r--   0     1001      127     8325 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/nodes.rs
+-rw-r--r--   0     1001      127    13236 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/parse.rs
+-rw-r--r--   0     1001      127     1788 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lcabyg/results.rs
+-rw-r--r--   0     1001      127       45 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/lib.rs
+-rw-r--r--   0     1001      127       30 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/slice/mod.rs
+-rw-r--r--   0     1001      127    13484 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/slice/model.rs
+-rw-r--r--   0     1001      127     5871 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/src/slice/parse.rs
+-rw-r--r--   0     1001      127      262 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/convert_tests.rs
+-rw-r--r--   0     1001      127    64785 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
+-rw-r--r--   0     1001      127    68643 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
+-rw-r--r--   0     1001      127    81962 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
+-rw-r--r--   0     1001      127    70431 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
+-rw-r--r--   0     1001      127    70200 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
+-rw-r--r--   0     1001      127    84820 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
+-rw-r--r--   0     1001      127    50733 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
+-rw-r--r--   0     1001      127    80754 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
+-rw-r--r--   0     1001      127   102497 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
+-rw-r--r--   0     1001      127   111759 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
+-rw-r--r--   0     1001      127    87077 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
+-rw-r--r--   0     1001      127   100644 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
+-rw-r--r--   0     1001      127    52735 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
+-rwxr-xr-x   0     1001      127    69619 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rwxr-xr-x   0     1001      127    47820 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
+-rw-r--r--   0     1001      127     4623 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/ilcd/test_parse_ilcd.rs
+-rw-r--r--   0     1001      127     2779 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
+-rw-r--r--   0     1001      127    25028 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
+-rw-r--r--   0     1001      127  2051524 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
+-rw-r--r--   0     1001      127    13935 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127     1961 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
+-rw-r--r--   0     1001      127     2157 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
+-rw-r--r--   0     1001      127      133 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
+-rw-r--r--   0     1001      127      905 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/convert/tests/slice/test_parse_slice.rs
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.1.0/modules/lcax/Cargo.toml
+-rw-r--r--   0     1001      127     1505 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/javascript.rs
+-rw-r--r--   0     1001      127      113 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/lib.rs
+-rw-r--r--   0     1001      127     1551 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/python.rs
+-rw-r--r--   0     1001      127      859 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/rust.rs
+-rw-r--r--   0     1001      127      246 2024-05-09 11:06:46.000000 lcax-2.1.0/modules/lcax/src/schemars.rs
+-rw-r--r--   0     1001      127    35772 2024-05-09 11:06:48.000000 lcax-2.1.0/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.1.0/Cargo.toml
+-rw-r--r--   0     1001      127     1441 2024-05-09 11:06:47.000000 lcax-2.1.0/pyproject.toml
+-rw-r--r--   0     1001      127     2825 2024-05-09 11:06:47.000000 lcax-2.1.0/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      127      407 2024-05-09 11:06:47.000000 lcax-2.1.0/packages/python/src/lcax/lcax.pyi
+-rw-r--r--   0     1001      127    15323 2024-05-09 11:06:49.000000 lcax-2.1.0/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      127    10173 2024-05-09 11:06:46.000000 lcax-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.1.0/PKG-INFO
```

### Comparing `lcax-2.0.6/modules/convert/Cargo.toml` & `lcax-2.1.0/modules/convert/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/ilcd/ilcd.rs` & `lcax-2.1.0/modules/convert/src/ilcd/ilcd.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/ilcd/parse.rs` & `lcax-2.1.0/modules/convert/src/ilcd/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/lcabyg/categories.rs` & `lcax-2.1.0/modules/convert/src/lcabyg/categories.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/lcabyg/edges.rs` & `lcax-2.1.0/modules/convert/src/lcabyg/edges.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/lcabyg/nodes.rs` & `lcax-2.1.0/modules/convert/src/lcabyg/nodes.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/lcabyg/parse.rs` & `lcax-2.1.0/modules/convert/src/lcabyg/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/lcabyg/results.rs` & `lcax-2.1.0/modules/convert/src/lcabyg/results.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/slice/model.rs` & `lcax-2.1.0/modules/convert/src/slice/model.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/src/slice/parse.rs` & `lcax-2.1.0/modules/convert/src/slice/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json` & `lcax-2.1.0/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/ilcd/test_parse_ilcd.rs` & `lcax-2.1.0/modules/convert/tests/ilcd/test_parse_ilcd.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json` & `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json` & `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json` & `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json` & `lcax-2.1.0/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg.rs` & `lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs` & `lcax-2.1.0/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/convert/tests/slice/test_parse_slice.rs` & `lcax-2.1.0/modules/convert/tests/slice/test_parse_slice.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/README.md` & `lcax-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/models/Cargo.toml` & `lcax-2.1.0/modules/models/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/models/src/assembly.rs` & `lcax-2.1.0/modules/models/src/assembly.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/models/src/epd.rs` & `lcax-2.1.0/modules/models/src/epd.rs`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 use lcax_core::dates::{deserialize_yyyy_mm_dd, serialize_yyyy_mm_dd};
 use lcax_core::utils::get_version;
 
 use crate::life_cycle_base::{ImpactCategory, ImpactCategoryKey};
 use crate::shared::{Conversion, Source, Unit};
 
 #[derive(Serialize, Deserialize, JsonSchema, Clone)]
+#[serde(rename_all = "camelCase")]
 #[cfg_attr(
     feature = "jsbindings",
     derive(Tsify),
     tsify(into_wasm_abi, from_wasm_abi)
 )]
 pub struct EPD {
     pub id: String,
@@ -105,36 +106,7 @@
             }
             Some(_value) if _value.to_lowercase().contains("specific") => SubType::Specific,
             Some(_value) if _value.to_lowercase().contains("industry") => SubType::Industry,
             _ => SubType::Generic,
         }
     }
 }
-
-// mod my_date_format {
-//     use chrono::{NaiveDate};
-//     use serde::{self, Serializer, Deserializer, Deserialize};
-//
-//     const FORMAT: &'static str = "%Y-%m-%d";
-//
-//     pub fn serialize<S>(
-//         date: &NaiveDate,
-//         serializer: S,
-//     ) -> Result<S::Ok, S::Error>
-//         where
-//             S: Serializer,
-//     {
-//         let s = format!("{}", date.format(FORMAT));
-//         serializer.serialize_str(&s)
-//     }
-//
-//     pub fn deserialize<'de, D>(
-//         deserializer: D,
-//     ) -> Result<NaiveDate, D::Error>
-//         where
-//             D: Deserializer<'de>,
-//     {
-//         let s = String::deserialize(deserializer)?;
-//         let dt = NaiveDate::parse_from_str(&s, FORMAT).map_err(serde::de::Error::custom)?;
-//         Ok(dt)
-//     }
-// }
```

### Comparing `lcax-2.0.6/modules/models/src/life_cycle_base.rs` & `lcax-2.1.0/modules/models/src/life_cycle_base.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/models/src/product.rs` & `lcax-2.1.0/modules/models/src/product.rs`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     pub name: String,
     pub distance: f64,
     pub distance_unit: Unit,
     pub transport_epd: ImpactDataSource,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
-#[serde(rename_all = "lowercase")]
+#[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub enum ImpactDataSource {
     EPD(EPD),
     TechFlow(TechFlow),
     ExternalImpactData(ExternalImpactData),
     InternalImpactData(InternalImpactData),
 }
```

### Comparing `lcax-2.0.6/modules/models/src/project.rs` & `lcax-2.1.0/modules/models/src/project.rs`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,21 @@
     OTHER,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Default, Clone)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub struct Location {
-    pub country: lcax_core::country::Country,
+    pub country: Country,
     pub city: Option<String>,
     pub address: Option<String>,
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
-#[serde(rename_all = "lowercase")]
+#[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub enum ProjectInfo {
     BuildingInfo(BuildingInfo),
     InfrastructureInfo(HashMap<String, String>),
 }
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
```

### Comparing `lcax-2.0.6/modules/models/src/shared.rs` & `lcax-2.1.0/modules/models/src/shared.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/models/src/techflow.rs` & `lcax-2.1.0/modules/models/src/techflow.rs`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 use lcax_core::country::Country;
 use lcax_core::utils::get_version;
 
 use crate::life_cycle_base::{ImpactCategory, ImpactCategoryKey};
 use crate::shared::{Conversion, Source, Unit};
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
+#[serde(rename_all = "camelCase")]
 #[cfg_attr(
     feature = "jsbindings",
     derive(Tsify),
     tsify(into_wasm_abi, from_wasm_abi)
 )]
 pub struct TechFlow {
     pub id: String,
```

### Comparing `lcax-2.0.6/modules/core/Cargo.toml` & `lcax-2.1.0/modules/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/core/src/country.rs` & `lcax-2.1.0/modules/core/src/country.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/core/src/dates.rs` & `lcax-2.1.0/modules/core/src/dates.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/core/src/utils.rs` & `lcax-2.1.0/modules/core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/lcax/Cargo.toml` & `lcax-2.1.0/modules/lcax/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/lcax/src/javascript.rs` & `lcax-2.1.0/modules/lcax/src/javascript.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/lcax/src/python.rs` & `lcax-2.1.0/modules/lcax/src/python.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/modules/lcax/src/rust.rs` & `lcax-2.1.0/modules/lcax/src/rust.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/Cargo.lock` & `lcax-2.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "lcax"
-version = "2.0.6"
+version = "2.1.0"
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
-version = "2.0.6"
+version = "2.1.0"
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
-version = "2.0.6"
+version = "2.1.0"
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
-version = "2.0.6"
+version = "2.1.0"
 dependencies = [
  "chrono",
  "console_error_panic_hook",
  "lcax_core",
  "pyo3",
  "schemars",
  "serde",
```

### Comparing `lcax-2.0.6/pyproject.toml` & `lcax-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/packages/python/src/lcax/__init__.py` & `lcax-2.1.0/packages/python/src/lcax/__init__.py`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/packages/python/src/lcax/pydantic.py` & `lcax-2.1.0/packages/python/src/lcax/pydantic.py`

 * *Files 3% similar despite different names*

```diff
@@ -362,15 +362,15 @@
 
 
 class ImpactDataSource3(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    externalimpactdata: ExternalImpactData
+    external_impact_data: ExternalImpactData = Field(..., alias='externalImpactData')
 
 
 class InternalImpactData(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     path: str
@@ -404,15 +404,15 @@
 
 
 class ProjectInfo2(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    infrastructureinfo: Dict[str, str]
+    infrastructure_info: Dict[str, str] = Field(..., alias='infrastructureInfo')
 
 
 class ProjectPhase(Enum):
     DESIGN = 'design'
     ONGOING = 'ongoing'
     BUILT = 'built'
     OTHER = 'other'
@@ -537,76 +537,78 @@
 
 class EPD(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     comment: Optional[str] = None
     conversions: Optional[List[Conversion]] = None
-    declared_unit: Unit
-    format_version: str
+    declared_unit: Unit = Field(..., alias='declaredUnit')
+    format_version: str = Field(..., alias='formatVersion')
     id: str
     impacts: Dict[str, Dict[str, Optional[float]]]
     location: Country
-    meta_data: Optional[Dict[str, Any]] = None
+    meta_data: Optional[Dict[str, Any]] = Field(None, alias='metaData')
     name: str
-    published_date: date
-    reference_service_life: Optional[int] = Field(None, ge=0)
+    published_date: date = Field(..., alias='publishedDate')
+    reference_service_life: Optional[int] = Field(
+        None, alias='referenceServiceLife', ge=0
+    )
     source: Optional[Source] = None
     standard: Standard
     subtype: SubType
-    valid_until: date
+    valid_until: date = Field(..., alias='validUntil')
     version: str
 
 
 class ImpactDataSource1(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    epd: EPD
+    e_pd: EPD = Field(..., alias='ePD')
 
 
 class ImpactDataSource4(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    internalimpactdata: InternalImpactData
+    internal_impact_data: InternalImpactData = Field(..., alias='internalImpactData')
 
 
 class ProjectInfo1(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    buildinginfo: BuildingInfo
+    building_info: BuildingInfo = Field(..., alias='buildingInfo')
 
 
 class TechFlow(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     comment: Optional[str] = None
     conversions: Optional[List[Conversion]] = None
-    declared_unit: Unit
-    format_version: str
+    declared_unit: Unit = Field(..., alias='declaredUnit')
+    format_version: str = Field(..., alias='formatVersion')
     id: str
     impacts: Dict[str, Dict[str, Optional[float]]]
     location: Country
-    meta_data: Optional[Dict[str, Any]] = None
+    meta_data: Optional[Dict[str, Any]] = Field(None, alias='metaData')
     name: str
     source: Optional[Source] = None
 
 
 class ImpactDataSource2(BaseModel):
     model_config = ConfigDict(
         extra='forbid',
         populate_by_name=True,
     )
-    techflow: TechFlow
+    tech_flow: TechFlow = Field(..., alias='techFlow')
 
 
 class Transport(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     distance: float
```

### Comparing `lcax-2.0.6/LICENSE` & `lcax-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-2.0.6/PKG-INFO` & `lcax-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lcax
-Version: 2.0.6
+Version: 2.1.0
 Requires-Dist: cffi
 Requires-Dist: pydantic >2.0.0
 Requires-Dist: mkdocs-material >=8.1.4, <9.0.0 ; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1, <2.0.0 ; extra == 'doc'
 Requires-Dist: datamodel-code-generator ; extra == 'codegen'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-datafixtures ; extra == 'tests'
```


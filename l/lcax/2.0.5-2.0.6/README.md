# Comparing `tmp/lcax-2.0.5.tar.gz` & `tmp/lcax-2.0.6.tar.gz`

## Comparing `lcax-2.0.5.tar` & `lcax-2.0.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0     1001      127      845 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/Cargo.toml
--rw-r--r--   0     1001      127     5582 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/ilcd/ilcd.rs
--rw-r--r--   0     1001      127       29 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/ilcd/mod.rs
--rw-r--r--   0     1001      127    16269 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/ilcd/parse.rs
--rw-r--r--   0     1001      127     4042 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/categories.rs
--rw-r--r--   0     1001      127     2045 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/edges.rs
--rw-r--r--   0     1001      127       70 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/mod.rs
--rw-r--r--   0     1001      127     8325 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/nodes.rs
--rw-r--r--   0     1001      127    13218 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/parse.rs
--rw-r--r--   0     1001      127     1788 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lcabyg/results.rs
--rw-r--r--   0     1001      127       45 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/lib.rs
--rw-r--r--   0     1001      127       30 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/slice/mod.rs
--rw-r--r--   0     1001      127    13472 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/slice/model.rs
--rw-r--r--   0     1001      127     5871 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/src/slice/parse.rs
--rw-r--r--   0     1001      127      261 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/convert_tests.rs
--rw-r--r--   0     1001      127    64785 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
--rw-r--r--   0     1001      127    68643 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
--rw-r--r--   0     1001      127    81962 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
--rw-r--r--   0     1001      127    70431 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
--rw-r--r--   0     1001      127    70200 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
--rw-r--r--   0     1001      127    84820 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
--rw-r--r--   0     1001      127    50733 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
--rw-r--r--   0     1001      127    80754 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
--rw-r--r--   0     1001      127   102497 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
--rw-r--r--   0     1001      127   111759 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
--rw-r--r--   0     1001      127    87077 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
--rw-r--r--   0     1001      127   100644 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
--rw-r--r--   0     1001      127    52735 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
--rwxr-xr-x   0     1001      127    69619 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
--rwxr-xr-x   0     1001      127    47820 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
--rw-r--r--   0     1001      127     4625 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/ilcd/test_parse_ilcd.rs
--rw-r--r--   0     1001      127     2779 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
--rw-r--r--   0     1001      127    25028 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
--rw-r--r--   0     1001      127  2051524 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
--rw-r--r--   0     1001      127    13935 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
--rw-r--r--   0     1001      127     1961 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
--rw-r--r--   0     1001      127     2158 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
--rw-r--r--   0     1001      127      133 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
--rw-r--r--   0     1001      127      905 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/convert/tests/slice/test_parse_slice.rs
--rw-r--r--   0     1001      127     1524 2024-05-08 11:58:51.000000 lcax-2.0.5/README.md
--rw-r--r--   0     1001      127     1135 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/Cargo.toml
--rw-r--r--   0     1001      127      959 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/assembly.rs
--rw-r--r--   0     1001      127     4080 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/epd.rs
--rw-r--r--   0     1001      127      124 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/lib.rs
--rw-r--r--   0     1001      127     5764 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/life_cycle_base.rs
--rw-r--r--   0     1001      127     1959 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/product.rs
--rw-r--r--   0     1001      127     7201 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/project.rs
--rw-r--r--   0     1001      127     1295 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/shared.rs
--rw-r--r--   0     1001      127     1296 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/src/techflow.rs
--rw-r--r--   0     1001      127      147 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/tests/test_epd.rs
--rw-r--r--   0     1001      127      168 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/tests/test_project.rs
--rw-r--r--   0     1001      127      180 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/models/tests/test_techflow.rs
--rw-r--r--   0     1001      127      589 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/Cargo.toml
--rw-r--r--   0     1001      127    20171 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/country.rs
--rw-r--r--   0     1001      127     1391 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/dates.rs
--rw-r--r--   0     1001      127       47 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/lib.rs
--rw-r--r--   0     1001      127      686 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/core/src/utils.rs
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.0.5/modules/lcax/Cargo.toml
--rw-r--r--   0     1001      127     1521 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/javascript.rs
--rw-r--r--   0     1001      127      113 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/lib.rs
--rw-r--r--   0     1001      127     1551 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/python.rs
--rw-r--r--   0     1001      127      859 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/rust.rs
--rw-r--r--   0     1001      127      246 2024-05-08 11:58:51.000000 lcax-2.0.5/modules/lcax/src/schemars.rs
--rw-r--r--   0     1001      127    35772 2024-05-08 11:58:52.000000 lcax-2.0.5/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.0.5/Cargo.toml
--rw-r--r--   0     1001      127     1441 2024-05-08 11:58:52.000000 lcax-2.0.5/pyproject.toml
--rw-r--r--   0     1001      127     2825 2024-05-08 11:58:51.000000 lcax-2.0.5/packages/python/src/lcax/__init__.py
--rw-r--r--   0     1001      127      407 2024-05-08 11:58:52.000000 lcax-2.0.5/packages/python/src/lcax/lcax.pyi
--rw-r--r--   0     1001      127    14761 2024-05-08 11:58:53.000000 lcax-2.0.5/packages/python/src/lcax/pydantic.py
--rw-r--r--   0     1001      127    10173 2024-05-08 11:58:51.000000 lcax-2.0.5/LICENSE
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.0.5/PKG-INFO
+-rw-r--r--   0     1001      127      845 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/Cargo.toml
+-rw-r--r--   0     1001      127     5582 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/ilcd/ilcd.rs
+-rw-r--r--   0     1001      127       29 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/ilcd/mod.rs
+-rw-r--r--   0     1001      127    16269 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/ilcd/parse.rs
+-rw-r--r--   0     1001      127     4042 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/categories.rs
+-rw-r--r--   0     1001      127     2045 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/edges.rs
+-rw-r--r--   0     1001      127       70 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/mod.rs
+-rw-r--r--   0     1001      127     8325 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/nodes.rs
+-rw-r--r--   0     1001      127    13236 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/parse.rs
+-rw-r--r--   0     1001      127     1788 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lcabyg/results.rs
+-rw-r--r--   0     1001      127       45 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/lib.rs
+-rw-r--r--   0     1001      127       30 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/slice/mod.rs
+-rw-r--r--   0     1001      127    13484 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/slice/model.rs
+-rw-r--r--   0     1001      127     5871 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/src/slice/parse.rs
+-rw-r--r--   0     1001      127      262 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/convert_tests.rs
+-rw-r--r--   0     1001      127    64785 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json
+-rw-r--r--   0     1001      127    68643 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json
+-rw-r--r--   0     1001      127    81962 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json
+-rw-r--r--   0     1001      127    70431 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json
+-rw-r--r--   0     1001      127    70200 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json
+-rw-r--r--   0     1001      127    84820 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json
+-rw-r--r--   0     1001      127    50733 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json
+-rw-r--r--   0     1001      127    80754 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json
+-rw-r--r--   0     1001      127   102497 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json
+-rw-r--r--   0     1001      127   111759 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json
+-rw-r--r--   0     1001      127    87077 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json
+-rw-r--r--   0     1001      127   100644 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json
+-rw-r--r--   0     1001      127    52735 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json
+-rwxr-xr-x   0     1001      127    69619 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json
+-rwxr-xr-x   0     1001      127    47820 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json
+-rw-r--r--   0     1001      127     4623 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/ilcd/test_parse_ilcd.rs
+-rw-r--r--   0     1001      127     2779 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json
+-rw-r--r--   0     1001      127    25028 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json
+-rw-r--r--   0     1001      127  2051524 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json
+-rw-r--r--   0     1001      127    13935 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json
+-rw-r--r--   0     1001      127     1961 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg.rs
+-rw-r--r--   0     1001      127     2157 2024-05-09 10:05:05.000000 lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs
+-rw-r--r--   0     1001      127      133 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/convert/tests/slice/datafixtures/results_slice_WLCR.parquet
+-rw-r--r--   0     1001      127      905 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/convert/tests/slice/test_parse_slice.rs
+-rw-r--r--   0     1001      127     1524 2024-05-09 10:05:05.000000 lcax-2.0.6/README.md
+-rw-r--r--   0     1001      127     1135 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/Cargo.toml
+-rw-r--r--   0     1001      127      967 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/assembly.rs
+-rw-r--r--   0     1001      127     4080 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/epd.rs
+-rw-r--r--   0     1001      127      124 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/lib.rs
+-rw-r--r--   0     1001      127     5764 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/life_cycle_base.rs
+-rw-r--r--   0     1001      127     1967 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/product.rs
+-rw-r--r--   0     1001      127     7201 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/project.rs
+-rw-r--r--   0     1001      127     1295 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/shared.rs
+-rw-r--r--   0     1001      127     1296 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/src/techflow.rs
+-rw-r--r--   0     1001      127      147 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/tests/test_epd.rs
+-rw-r--r--   0     1001      127      168 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/tests/test_project.rs
+-rw-r--r--   0     1001      127      180 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/models/tests/test_techflow.rs
+-rw-r--r--   0     1001      127      589 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/Cargo.toml
+-rw-r--r--   0     1001      127    20171 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/country.rs
+-rw-r--r--   0     1001      127     1391 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/dates.rs
+-rw-r--r--   0     1001      127       47 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/lib.rs
+-rw-r--r--   0     1001      127      686 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/core/src/utils.rs
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 lcax-2.0.6/modules/lcax/Cargo.toml
+-rw-r--r--   0     1001      127     1505 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/javascript.rs
+-rw-r--r--   0     1001      127      113 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/lib.rs
+-rw-r--r--   0     1001      127     1551 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/python.rs
+-rw-r--r--   0     1001      127      859 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/rust.rs
+-rw-r--r--   0     1001      127      246 2024-05-09 10:05:06.000000 lcax-2.0.6/modules/lcax/src/schemars.rs
+-rw-r--r--   0     1001      127    35772 2024-05-09 10:05:07.000000 lcax-2.0.6/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 lcax-2.0.6/Cargo.toml
+-rw-r--r--   0     1001      127     1441 2024-05-09 10:05:06.000000 lcax-2.0.6/pyproject.toml
+-rw-r--r--   0     1001      127     2825 2024-05-09 10:05:06.000000 lcax-2.0.6/packages/python/src/lcax/__init__.py
+-rw-r--r--   0     1001      127      407 2024-05-09 10:05:06.000000 lcax-2.0.6/packages/python/src/lcax/lcax.pyi
+-rw-r--r--   0     1001      127    14795 2024-05-09 10:05:08.000000 lcax-2.0.6/packages/python/src/lcax/pydantic.py
+-rw-r--r--   0     1001      127    10173 2024-05-09 10:05:05.000000 lcax-2.0.6/LICENSE
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 lcax-2.0.6/PKG-INFO
```

### Comparing `lcax-2.0.5/modules/convert/Cargo.toml` & `lcax-2.0.6/modules/convert/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/ilcd/ilcd.rs` & `lcax-2.0.6/modules/convert/src/ilcd/ilcd.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/ilcd/parse.rs` & `lcax-2.0.6/modules/convert/src/ilcd/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/lcabyg/categories.rs` & `lcax-2.0.6/modules/convert/src/lcabyg/categories.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/lcabyg/edges.rs` & `lcax-2.0.6/modules/convert/src/lcabyg/edges.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/lcabyg/nodes.rs` & `lcax-2.0.6/modules/convert/src/lcabyg/nodes.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/lcabyg/parse.rs` & `lcax-2.0.6/modules/convert/src/lcabyg/parse.rs`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     nodes: &Vec<Node>,
     edges: &Vec<Edge>,
 ) {
     let node_id = node.id.clone();
     let mut assembly = Assembly {
         id: node_id.to_string(),
         name: node.name.english.clone().unwrap(),
-        description: "".to_string(),
+        description: Some("".to_string()),
         comment: node.comment.english.clone(),
         quantity: 0.0,
         unit: Unit::M,
         category: None,
         classification: None,
         products: Default::default(),
         results: None,
@@ -351,15 +351,15 @@
     product_id: &String,
     edge: &edges::ConstructionToProductEdge,
     nodes: &Vec<Node>,
 ) -> LCAxProduct {
     let mut product = LCAxProduct {
         id: product_id.clone(),
         name: "".to_string(),
-        description: "".to_string(),
+        description: Some("".to_string()),
         reference_service_life: edge.lifespan,
         impact_data: Default::default(),
         quantity: edge.amount,
         unit: Unit::from(&edge.unit),
         transport: None,
         results: None,
         meta_data: None,
@@ -367,15 +367,15 @@
 
     let mut stages: Vec<nodes::Stage> = vec![];
 
     for node in nodes {
         match node {
             Node::Product(product_node) => {
                 product.name = product_node.name.english.clone().unwrap();
-                product.description = product_node.comment.english.clone().unwrap();
+                product.description = Some(product_node.comment.english.clone().unwrap());
             }
             Node::Stage(stage_node) => stages.append(&mut vec![stage_node.clone()]),
             _ => continue,
         }
     }
 
     let epd_data = epd_from_lcabyg_stages(&stages);
```

### Comparing `lcax-2.0.5/modules/convert/src/lcabyg/results.rs` & `lcax-2.0.6/modules/convert/src/lcabyg/results.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/src/slice/model.rs` & `lcax-2.0.6/modules/convert/src/slice/model.rs`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     uid.to_string()
 }
 
 fn assembly_from_slice(uid: &str, element: &SLiCEElement) -> Assembly {
     Assembly {
         id: uid.to_string(),
         name: element.element_class_sfb.clone(),
-        description: element.element_class_generic_name.clone(),
+        description: Some(element.element_class_generic_name.clone()),
         comment: None,
         quantity: 1.0,
         unit: Unit::KG,
         category: None,
         classification: Some(vec![Classification {
             system: "SfB".to_string(),
             code: element.element_class_sfb.clone(),
@@ -228,15 +228,15 @@
     }
 }
 
 fn product_from_slice(uid: &str, element: &SLiCEElement) -> Product {
     Product {
         id: uid.to_string(),
         name: element.worksection_class_sfb.clone(),
-        description: "".to_string(),
+        description: Some("".to_string()),
         reference_service_life: 50,
         impact_data: ImpactDataSource::TechFlow(create_tech_flow(element)),
         quantity: element.amount_material_kg_per_building,
         unit: Unit::KG,
         transport: None,
         results: None,
         meta_data: None,
```

### Comparing `lcax-2.0.5/modules/convert/src/slice/parse.rs` & `lcax-2.0.6/modules/convert/src/slice/parse.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/00c28f1f-1d49-4c81-9208-138922a1dd6c.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/023f3b97-976a-41c4-b0f1-5357b9dc5b3e.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b488798-140f-4efa-96e2-55aa46ed129a.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0b4c397d-c7a1-4ceb-9718-184334f6364e.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0cb92770-9007-48c6-bc03-466af8894419.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0d1e4a59-4901-4973-a26f-1698f65a780f.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e0c4e37-b7e6-4a4f-b1c9-d36da0aa16f5.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e80e6e7-6882-47be-8bd8-5cd869a746d9.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/0e9fd868-9656-489e-be6c-8251b3d43283.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/335241f9-db84-486c-9a19-cd5ebb791903.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/c23b2987-776d-4d55-91c7-5f2a0f2c50f1.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879-fa7d-4f91-813e-e816cbdf1927.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json` & `lcax-2.0.6/modules/convert/tests/ilcd/datafixtures/f63ac879_test.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/ilcd/test_parse_ilcd.rs` & `lcax-2.0.6/modules/convert/tests/ilcd/test_parse_ilcd.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-
-use std::fs;
-use std::path::Path;
 use lcax_convert::ilcd;
 use lcax_models::epd::Standard;
 use lcax_models::life_cycle_base::ImpactCategoryKey;
+use std::fs;
+use std::path::Path;
 
 macro_rules! parse_ilcd_a1_tests {
     ($($name:ident: $value:expr)*) => {
     $(
         #[test]
         fn $name() -> Result<(), String> {
             let (file_name, standard) = $value;
@@ -74,15 +73,14 @@
     ilcd_0e9fd868: ("0e9fd868-9656-489e-be6c-8251b3d43283.json", "a2")
     ilcd_0cb92770: ("0cb92770-9007-48c6-bc03-466af8894419.json", "a2")
     ilcd_0aa8b645: ("0aa8b645-02d9-41b4-8aa3-70335af2a9e7.json", "a2")
     ilcd_335241f9: ("335241f9-db84-486c-9a19-cd5ebb791903.json", "a2")
     ilcd_503dfca1: ("503dfca1-7c65-4179-9ffa-ebc6d8b48b7d.json", "a2")
 }
 
-
 #[test]
 fn test_parse_ilcd_short() -> Result<(), String> {
     let root_dir = Path::new(env!("CARGO_MANIFEST_DIR"));
     let file_path = root_dir.join("tests/ilcd/datafixtures/f63ac879_test.json");
     let contents = fs::read_to_string(file_path).expect("Should have been able to read the file");
 
     match ilcd::parse::parse_ilcd(&contents) {
```

### Comparing `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json` & `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/5aa09d72.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json` & `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_project.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json` & `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_example_results.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json` & `lcax-2.0.6/modules/convert/tests/lcabyg/datafixtures/lcabyg_project.json`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/convert/tests/lcabyg/test_parse_lcabyg.rs` & `lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::fs;
 use std::path::Path;
 
-use lcax_convert::lcabyg::nodes::{epd_from_lcabyg_stages, Stage, Node};
+use lcax_convert::lcabyg::nodes::{epd_from_lcabyg_stages, Node, Stage};
 use lcax_convert::lcabyg::parse::NodesAndEdges;
 use lcax_models::epd::Standard;
 use lcax_models::life_cycle_base::ImpactCategoryKey;
 
 macro_rules! parse_lcabyg_tests {
     ($($name:ident: $value:expr)*) => {
     $(
```

### Comparing `lcax-2.0.5/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs` & `lcax-2.0.6/modules/convert/tests/lcabyg/test_parse_lcabyg_project.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-
+use lcax_convert::lcabyg;
 use std::fs;
 use std::path::Path;
-use lcax_convert::lcabyg;
 
 #[test]
 fn test_parse_lcabyg_project() -> Result<(), String> {
     let root_dir = Path::new(env!("CARGO_MANIFEST_DIR"));
     let file_path = root_dir.join("tests/lcabyg/datafixtures/lcabyg_project.json");
     let contents = fs::read_to_string(file_path).expect("Should have been able to read the file");
```

### Comparing `lcax-2.0.5/modules/convert/tests/slice/test_parse_slice.rs` & `lcax-2.0.6/modules/convert/tests/slice/test_parse_slice.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/README.md` & `lcax-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/models/Cargo.toml` & `lcax-2.0.6/modules/models/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/models/src/assembly.rs` & `lcax-2.0.6/modules/models/src/assembly.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub struct Assembly {
     pub id: String,
     pub name: String,
-    pub description: String,
+    pub description: Option<String>,
     pub comment: Option<String>,
     pub quantity: f64,
     pub unit: Unit,
     pub category: Option<String>,
     pub classification: Option<Vec<Classification>>,
     pub products: HashMap<String, Product>,
     pub results: Results,
```

### Comparing `lcax-2.0.5/modules/models/src/epd.rs` & `lcax-2.0.6/modules/models/src/epd.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/models/src/life_cycle_base.rs` & `lcax-2.0.6/modules/models/src/life_cycle_base.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/models/src/product.rs` & `lcax-2.0.6/modules/models/src/product.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 #[derive(Deserialize, Serialize, JsonSchema, Clone)]
 #[serde(rename_all = "camelCase")]
 #[cfg_attr(feature = "jsbindings", derive(Tsify))]
 pub struct Product {
     pub id: String,
     pub name: String,
-    pub description: String,
+    pub description: Option<String>,
     pub reference_service_life: u32,
     pub impact_data: ImpactDataSource,
     pub quantity: f64,
     pub unit: Unit,
     pub transport: Option<Transport>,
     pub results: Results,
     pub meta_data: Option<HashMap<String, String>>,
```

### Comparing `lcax-2.0.5/modules/models/src/project.rs` & `lcax-2.0.6/modules/models/src/project.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/models/src/shared.rs` & `lcax-2.0.6/modules/models/src/shared.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/models/src/techflow.rs` & `lcax-2.0.6/modules/models/src/techflow.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/core/Cargo.toml` & `lcax-2.0.6/modules/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/core/src/country.rs` & `lcax-2.0.6/modules/core/src/country.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/core/src/dates.rs` & `lcax-2.0.6/modules/core/src/dates.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/core/src/utils.rs` & `lcax-2.0.6/modules/core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/lcax/Cargo.toml` & `lcax-2.0.6/modules/lcax/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/lcax/src/javascript.rs` & `lcax-2.0.6/modules/lcax/src/javascript.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 use wasm_bindgen::prelude::*;
 
 use lcax_convert::{ilcd, lcabyg, slice};
 use lcax_models::epd::EPD;
 use lcax_models::project::Project;
 use serde::{Deserialize, Serialize};
 extern crate console_error_panic_hook;
-use std::panic;
 
 #[global_allocator]
 static ALLOC: wee_alloc::WeeAlloc = wee_alloc::WeeAlloc::INIT;
 
 #[wasm_bindgen]
 extern "C" {
     fn alert(s: &str);
```

### Comparing `lcax-2.0.5/modules/lcax/src/python.rs` & `lcax-2.0.6/modules/lcax/src/python.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/modules/lcax/src/rust.rs` & `lcax-2.0.6/modules/lcax/src/rust.rs`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/Cargo.lock` & `lcax-2.0.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "lcax"
-version = "2.0.5"
+version = "2.0.6"
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
-version = "2.0.5"
+version = "2.0.6"
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
-version = "2.0.5"
+version = "2.0.6"
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
-version = "2.0.5"
+version = "2.0.6"
 dependencies = [
  "chrono",
  "console_error_panic_hook",
  "lcax_core",
  "pyo3",
  "schemars",
  "serde",
```

### Comparing `lcax-2.0.5/pyproject.toml` & `lcax-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/packages/python/src/lcax/__init__.py` & `lcax-2.0.6/packages/python/src/lcax/__init__.py`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/packages/python/src/lcax/pydantic.py` & `lcax-2.0.6/packages/python/src/lcax/pydantic.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,15 @@
     ] = Field(..., alias='transportEpd')
 
 
 class Product(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
-    description: str
+    description: Optional[str] = None
     id: str
     impact_data: Union[
         ImpactDataSource1, ImpactDataSource2, ImpactDataSource3, ImpactDataSource4
     ] = Field(..., alias='impactData')
     meta_data: Optional[Dict[str, Any]] = Field(None, alias='metaData')
     name: str
     quantity: float
@@ -639,15 +639,15 @@
 class Assembly(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     category: Optional[str] = None
     classification: Optional[List[Classification]] = None
     comment: Optional[str] = None
-    description: str
+    description: Optional[str] = None
     id: str
     meta_data: Optional[Dict[str, Any]] = Field(None, alias='metaData')
     name: str
     products: Dict[str, Product]
     quantity: float
     results: Optional[Dict[str, Any]] = None
     unit: Unit
```

### Comparing `lcax-2.0.5/LICENSE` & `lcax-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lcax-2.0.5/PKG-INFO` & `lcax-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lcax
-Version: 2.0.5
+Version: 2.0.6
 Requires-Dist: cffi
 Requires-Dist: pydantic >2.0.0
 Requires-Dist: mkdocs-material >=8.1.4, <9.0.0 ; extra == 'doc'
 Requires-Dist: mdx-include >=1.4.1, <2.0.0 ; extra == 'doc'
 Requires-Dist: datamodel-code-generator ; extra == 'codegen'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-datafixtures ; extra == 'tests'
```


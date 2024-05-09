# Comparing `tmp/dbt_hologres-1.7.8.tar.gz` & `tmp/dbt_hologres-1.7.8a0.tar.gz`

## Comparing `dbt_hologres-1.7.8.tar` & `dbt_hologres-1.7.8a0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/adapters/hologres/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/adapters/hologres/__version__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/adapters/hologres/impl.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/adapters/hologres/relation.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/dbt_project.yml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/profile_template.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/sample_profiles.yml
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/adapters.sql
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/catalog.sql
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations.sql
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/timestamps.sql
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/incremental.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/seed.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/table.sql
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/view.sql
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/describe.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/view/rename.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/view/replace.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/any_value.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/dateadd.sql
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/datediff.sql
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/last_day.sql
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/listagg.sql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/split_part.sql
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/LICENSE
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/README.md
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/__version__.py
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/date.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/impl.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/adapters/hologres/relation.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/dbt_project.yml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros.yml
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/profile_template.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/sample_profiles.yml
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/adapters.sql
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/catalog.sql
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations.sql
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/timestamps.sql
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/seed.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/table.sql
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/view.sql
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/any_value.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/dateutil.sql
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/LICENSE
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/README.md
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/pyproject.toml
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 dbt_hologres-1.7.8a0/PKG-INFO
```

### Comparing `dbt_hologres-1.7.8/dbt/adapters/hologres/impl.py` & `dbt_hologres-1.7.8a0/dbt/adapters/hologres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/adapters.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/catalog.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/relations.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/timestamps.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/incremental.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/seed.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/snapshot_merge.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/table.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/materializations/view.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/materialized_view/alter.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/relations/table/replace.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/relations/table/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/datediff.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/dbt/include/hologres/macros/utils/listagg.sql` & `dbt_hologres-1.7.8a0/dbt/include/hologres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/.gitignore` & `dbt_hologres-1.7.8a0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/LICENSE` & `dbt_hologres-1.7.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/README.md` & `dbt_hologres-1.7.8a0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/pyproject.toml` & `dbt_hologres-1.7.8a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_hologres-1.7.8/PKG-INFO` & `dbt_hologres-1.7.8a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-hologres
-Version: 1.7.8
+Version: 1.7.8a0
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/winwin-inc/dbt-hologres
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/winwin-inc/dbt-hologres.git
 Project-URL: Issues, https://github.com/winwin-inc/dbt-hologres/issues
 Project-URL: Changelog, https://github.com/winwin-inc/dbt-hologres/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-hologres Version: 1.7.8 Summary: The set of
+Metadata-Version: 2.1 Name: dbt-hologres Version: 1.7.8a0 Summary: The set of
 adapter protocols and base functionality that supports integration with dbt-
 core Project-URL: Homepage, https://github.com/winwin-inc/dbt-hologres Project-
 URL: Documentation, https://docs.getdbt.com Project-URL: Repository, https://
 github.com/winwin-inc/dbt-hologres.git Project-URL: Issues, https://github.com/
 winwin-inc/dbt-hologres/issues Project-URL: Changelog, https://github.com/
 winwin-inc/dbt-hologres/blob/main/CHANGELOG.md Author-email: dbt Labs
 dbtlabs.com> Maintainer-email: dbt Labs
```


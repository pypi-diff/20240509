# Comparing `tmp/perceval_mozilla-1.0.0rc2.tar.gz` & `tmp/perceval_mozilla-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_mozilla-1.0.0rc2.tar", max compression
+gzip compressed data, was "perceval_mozilla-1.0.1rc1.tar", max compression
```

## Comparing `perceval_mozilla-1.0.0rc2.tar` & `perceval_mozilla-1.0.1rc1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      216 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     3414 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/NEWS
--rw-r--r--   0        0        0     2373 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/README.md
--rw-r--r--   0        0        0        0 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/__init__.py
--rw-r--r--   0        0        0       91 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/_version.py
--rw-r--r--   0        0        0    10890 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/crates.py
--rw-r--r--   0        0        0    12869 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/kitsune.py
--rw-r--r--   0        0        0    11469 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/mozillaclub.py
--rw-r--r--   0        0        0    10907 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/remo.py
--rw-r--r--   0        0        0     1414 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0     1889 2024-04-11 10:49:15.697388 perceval_mozilla-1.0.0rc2/tests/base.py
--rw-r--r--   0        0        0        0 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_1
--rw-r--r--   0        0        0     2797 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_2
--rw-r--r--   0        0        0     1840 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_3
--rw-r--r--   0        0        0     6506 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_4
--rw-r--r--   0        0        0       19 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_team_1
--rw-r--r--   0        0        0      312 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_team_2
--rw-r--r--   0        0        0      295 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_team_3
--rw-r--r--   0        0        0      298 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_team_4
--rw-r--r--   0        0        0      324 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_1
--rw-r--r--   0        0        0      555 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_2
--rw-r--r--   0        0        0      555 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_3
--rw-r--r--   0        0        0      823 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_4
--rw-r--r--   0        0        0      369 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_version_downloads_1
--rw-r--r--   0        0        0        2 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_version_downloads_empty
--rw-r--r--   0        0        0      724 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_1
--rw-r--r--   0        0        0     3641 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_2
--rw-r--r--   0        0        0      748 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_3
--rw-r--r--   0        0        0     5010 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_4
--rw-r--r--   0        0        0     2181 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crates_page_1
--rw-r--r--   0        0        0     2352 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crates_page_2
--rw-r--r--   0        0        0       59 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crates_page_empty
--rw-r--r--   0        0        0    39923 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/crates/crates_summary
--rw-r--r--   0        0        0        0 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_answers_empty.json
--rw-r--r--   0        0        0     3693 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_question_answers.json
--rw-r--r--   0        0        0       78 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_question_answers_empy.json
--rw-r--r--   0        0        0     5730 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_questions_1_2.json
--rw-r--r--   0        0        0     8148 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_questions_2_2.json
--rw-r--r--   0        0        0       78 2024-04-11 10:49:15.701388 perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_questions_empty.json
--rw-r--r--   0        0        0  2047401 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/mozillaclub/feed.json
--rw-r--r--   0        0        0     1141 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities.json
--rw-r--r--   0        0        0     2893 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities_page_1_2.json
--rw-r--r--   0        0        0     2888 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities_page_2_2.json
--rw-r--r--   0        0        0       78 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities_page_empty.json
--rw-r--r--   0        0        0     1263 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events.json
--rw-r--r--   0        0        0     3463 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_1_2.json
--rw-r--r--   0        0        0     3784 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_2_2.json
--rw-r--r--   0        0        0      158 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_empty.json
--rw-r--r--   0        0        0     2904 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_page_1_2.json
--rw-r--r--   0        0        0     2889 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_page_2_2.json
--rw-r--r--   0        0        0       78 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_page_empty.json
--rw-r--r--   0        0        0    28055 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_reps.json
--rw-r--r--   0        0        0     2263 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users.json
--rw-r--r--   0        0        0     4143 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users_page_1_2.json
--rw-r--r--   0        0        0     4123 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users_page_2_2.json
--rw-r--r--   0        0        0       78 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users_page_empty.json
--rwxr-xr-x   0        0        0     1017 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/run_tests.py
--rw-r--r--   0        0        0    20404 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/test_crates.py
--rw-r--r--   0        0        0    16820 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/test_kitsune.py
--rw-r--r--   0        0        0    12118 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/test_mozillaclub.py
--rw-r--r--   0        0        0    17239 2024-04-11 10:49:15.705388 perceval_mozilla-1.0.0rc2/tests/test_remo.py
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 perceval_mozilla-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      216 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     3574 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/NEWS
+-rw-r--r--   0        0        0     2373 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/_version.py
+-rw-r--r--   0        0        0    10890 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/crates.py
+-rw-r--r--   0        0        0    12869 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/kitsune.py
+-rw-r--r--   0        0        0    11469 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/mozillaclub.py
+-rw-r--r--   0        0        0    10907 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/remo.py
+-rw-r--r--   0        0        0     1414 2024-05-09 08:00:28.531119 perceval_mozilla-1.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/__init__.py
+-rw-r--r--   0        0        0     1637 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_1
+-rw-r--r--   0        0        0     2797 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_2
+-rw-r--r--   0        0        0     1840 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_3
+-rw-r--r--   0        0        0     6506 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_4
+-rw-r--r--   0        0        0       19 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_team_1
+-rw-r--r--   0        0        0      312 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_team_2
+-rw-r--r--   0        0        0      295 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_team_3
+-rw-r--r--   0        0        0      298 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_team_4
+-rw-r--r--   0        0        0      324 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_1
+-rw-r--r--   0        0        0      555 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_2
+-rw-r--r--   0        0        0      555 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_3
+-rw-r--r--   0        0        0      823 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_4
+-rw-r--r--   0        0        0      369 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_version_downloads_1
+-rw-r--r--   0        0        0        2 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_version_downloads_empty
+-rw-r--r--   0        0        0      724 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_1
+-rw-r--r--   0        0        0     3641 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_2
+-rw-r--r--   0        0        0      748 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_3
+-rw-r--r--   0        0        0     5010 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_4
+-rw-r--r--   0        0        0     2181 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crates_page_1
+-rw-r--r--   0        0        0     2352 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crates_page_2
+-rw-r--r--   0        0        0       59 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crates_page_empty
+-rw-r--r--   0        0        0    39923 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/crates/crates_summary
+-rw-r--r--   0        0        0        0 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_answers_empty.json
+-rw-r--r--   0        0        0     3693 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_question_answers.json
+-rw-r--r--   0        0        0       78 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_question_answers_empy.json
+-rw-r--r--   0        0        0     5730 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_questions_1_2.json
+-rw-r--r--   0        0        0     8148 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_questions_2_2.json
+-rw-r--r--   0        0        0       78 2024-05-09 08:00:28.535119 perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_questions_empty.json
+-rw-r--r--   0        0        0  2047401 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/mozillaclub/feed.json
+-rw-r--r--   0        0        0     1141 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities.json
+-rw-r--r--   0        0        0     2893 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities_page_1_2.json
+-rw-r--r--   0        0        0     2888 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities_page_2_2.json
+-rw-r--r--   0        0        0       78 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities_page_empty.json
+-rw-r--r--   0        0        0     1263 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events.json
+-rw-r--r--   0        0        0     3463 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_1_2.json
+-rw-r--r--   0        0        0     3784 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_2_2.json
+-rw-r--r--   0        0        0      158 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_empty.json
+-rw-r--r--   0        0        0     2904 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_page_1_2.json
+-rw-r--r--   0        0        0     2889 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_page_2_2.json
+-rw-r--r--   0        0        0       78 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_page_empty.json
+-rw-r--r--   0        0        0    28055 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_reps.json
+-rw-r--r--   0        0        0     2263 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users.json
+-rw-r--r--   0        0        0     4143 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users_page_1_2.json
+-rw-r--r--   0        0        0     4123 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users_page_2_2.json
+-rw-r--r--   0        0        0       78 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users_page_empty.json
+-rwxr-xr-x   0        0        0     1017 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    20404 2024-05-09 08:00:28.539119 perceval_mozilla-1.0.1rc1/tests/test_crates.py
+-rw-r--r--   0        0        0    16820 2024-05-09 08:00:28.543119 perceval_mozilla-1.0.1rc1/tests/test_kitsune.py
+-rw-r--r--   0        0        0    12118 2024-05-09 08:00:28.543119 perceval_mozilla-1.0.1rc1/tests/test_mozillaclub.py
+-rw-r--r--   0        0        0    17239 2024-05-09 08:00:28.543119 perceval_mozilla-1.0.1rc1/tests/test_remo.py
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 perceval_mozilla-1.0.1rc1/PKG-INFO
```

### Comparing `perceval_mozilla-1.0.0rc2/LICENSE` & `perceval_mozilla-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/NEWS` & `perceval_mozilla-1.0.1rc1/NEWS`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+## perceval-mozilla 1.0.0 - (2024-04-13)
+
+**New features:**
+
+ * First major release\
+   GrimoireLab reached a stable status. This is our first major release.
+
+
   ## perceval-mozilla 0.4.3 - (2024-03-27)
   
   * Update Poetry's package dependencies
 
   ## perceval-mozilla 0.4.2 - (2024-03-12)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_mozilla-1.0.0rc2/README.md` & `perceval_mozilla-1.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/crates.py` & `perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/crates.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/kitsune.py` & `perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/kitsune.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/mozillaclub.py` & `perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/mozillaclub.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/perceval/backends/mozilla/remo.py` & `perceval_mozilla-1.0.1rc1/perceval/backends/mozilla/remo.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/pyproject.toml` & `perceval_mozilla-1.0.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-mozilla"
-version = "1.0.0-rc.2"
+version = "1.0.1-rc.1"
 description = "Bundle of Perceval backends for Mozilla ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_mozilla-1.0.0rc2/tests/base.py` & `perceval_mozilla-1.0.1rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_1` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_2` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_3` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_example_4` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_example_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_2` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_3` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_owner_user_4` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_owner_user_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_1` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_2` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_3` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_3`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crate_versions_4` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crate_versions_4`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crates_page_1` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crates_page_1`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crates_page_2` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crates_page_2`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/crates/crates_summary` & `perceval_mozilla-1.0.1rc1/tests/data/crates/crates_summary`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_question_answers.json` & `perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_question_answers.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_questions_1_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_questions_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/kitsune/kitsune_questions_2_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/kitsune/kitsune_questions_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/mozillaclub/feed.json` & `perceval_mozilla-1.0.1rc1/tests/data/mozillaclub/feed.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities_page_1_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_activities_page_2_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_activities_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_1_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_2_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_page_1_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_events_page_2_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_events_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_reps.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_reps.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users_page_1_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users_page_1_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/data/remo/remo_users_page_2_2.json` & `perceval_mozilla-1.0.1rc1/tests/data/remo/remo_users_page_2_2.json`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/run_tests.py` & `perceval_mozilla-1.0.1rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/test_crates.py` & `perceval_mozilla-1.0.1rc1/tests/test_crates.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/test_kitsune.py` & `perceval_mozilla-1.0.1rc1/tests/test_kitsune.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/test_mozillaclub.py` & `perceval_mozilla-1.0.1rc1/tests/test_mozillaclub.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/tests/test_remo.py` & `perceval_mozilla-1.0.1rc1/tests/test_remo.py`

 * *Files identical despite different names*

### Comparing `perceval_mozilla-1.0.0rc2/PKG-INFO` & `perceval_mozilla-1.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-mozilla
-Version: 1.0.0rc2
+Version: 1.0.1rc1
 Summary: Bundle of Perceval backends for Mozilla ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


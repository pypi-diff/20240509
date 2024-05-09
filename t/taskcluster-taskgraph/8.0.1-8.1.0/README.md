# Comparing `tmp/taskcluster-taskgraph-8.0.1.tar.gz` & `tmp/taskcluster-taskgraph-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-8.0.1.tar", last modified: Wed Apr 24 18:32:32 2024, max compression
+gzip compressed data, was "taskcluster-taskgraph-8.1.0.tar", last modified: Thu May  9 00:03:30 2024, max compression
```

## Comparing `taskcluster-taskgraph-8.0.1.tar` & `taskcluster-taskgraph-8.1.0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.492606 taskcluster-taskgraph-8.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.488606 taskcluster-taskgraph-8.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.492606 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 18:32:32.000000 taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/filter_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/loader/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    29072 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/morph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.496606 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/
--rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/hgrc
--rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/run-task
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.500606 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.500606 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.504606 taskcluster-taskgraph-8.0.1/src/taskgraph/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/set_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:32:32.512606 taskcluster-taskgraph-8.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_actions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_morph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_optimize_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_scripts_fetch_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_scripts_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transform_chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transform_docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transform_task_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_run_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_run_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_transforms_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_taskcluster.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-24 18:32:27.000000 taskcluster-taskgraph-8.0.1/test/test_util_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.148743 taskcluster-taskgraph-8.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.144743 taskcluster-taskgraph-8.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.148743 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 00:03:30.000000 taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.148743 taskcluster-taskgraph-8.1.0/src/taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8417 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29171 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/morph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20107 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.152743 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.156743 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.160743 taskcluster-taskgraph-8.1.0/src/taskgraph/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/set_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:30.164743 taskcluster-taskgraph-8.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_actions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_morph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_optimize_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_scripts_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transform_chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transform_docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transform_task_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_run_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_run_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_transforms_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-09 00:03:27.000000 taskcluster-taskgraph-8.1.0/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-8.0.1/LICENSE` & `taskcluster-taskgraph-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/PKG-INFO` & `taskcluster-taskgraph-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 8.0.1
+Version: 8.1.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-8.0.1/README.rst` & `taskcluster-taskgraph-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/pyproject.toml` & `taskcluster-taskgraph-8.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/requirements/base.txt` & `taskcluster-taskgraph-8.1.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/requirements/dev.txt` & `taskcluster-taskgraph-8.1.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/requirements/test.txt` & `taskcluster-taskgraph-8.1.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/setup.py` & `taskcluster-taskgraph-8.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 8.0.1
+Version: 8.1.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-8.1.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/__init__.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "8.0.1"
+__version__ = "8.1.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/config.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/create.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/decision.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/decision.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
      * processing decision task command-line options into parameters
      * running task-graph generation exactly the same way the other `mach
        taskgraph` commands do
      * generating a set of artifacts to memorialize the graph
      * calling TaskCluster APIs to create the graph
     """
+    if options.get("verbose"):
+        logging.root.setLevel(logging.DEBUG)
 
     parameters = parameters or (
         lambda graph_config: get_decision_parameters(graph_config, options)
     )
 
     decision_task_id = os.environ["TASK_ID"]
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/docker.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/generator.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/graph.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/main.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,14 +693,17 @@
     "--head-rev", required=True, help="Commit revision to use from head repository"
 )
 @argument("--head-tag", help="Tag attached to the revision", default="")
 @argument(
     "--tasks-for", required=True, help="the tasks_for value used to generate this task"
 )
 @argument("--try-task-config-file", help="path to try task configuration file")
+@argument(
+    "--verbose", "-v", action="store_true", help="include debug-level logging output"
+)
 def decision(options):
     from taskgraph.decision import taskgraph_decision
 
     taskgraph_decision(options)
 
 
 @command("action-callback", description="Run action callback used by action tasks")
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/morph.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from slugid import nice as slugid
 
 from taskgraph.graph import Graph
 from taskgraph.taskgraph import TaskGraph
 from taskgraph.util.parameterization import resolve_task_references, resolve_timestamps
 from taskgraph.util.python_path import import_sibling_modules
+from taskgraph.util.taskcluster import find_task_id_batched, status_task_batched
 
 logger = logging.getLogger(__name__)
 registry = {}
 
 
 def register_strategy(name, args=()):
     def wrap(cls):
@@ -47,14 +48,17 @@
     existing_tasks=None,
     strategy_override=None,
 ):
     """
     Perform task optimization, returning a taskgraph and a map from label to
     assigned taskId, including replacement tasks.
     """
+    # avoid circular import
+    from taskgraph.optimize.strategies import IndexSearch
+
     label_to_taskid = {}
     if not existing_tasks:
         existing_tasks = {}
 
     # instantiate the strategies for this optimization process
     strategies = registry.copy()
     if strategy_override:
@@ -66,22 +70,41 @@
         target_task_graph=target_task_graph,
         requested_tasks=requested_tasks,
         optimizations=optimizations,
         params=params,
         do_not_optimize=do_not_optimize,
     )
 
+    # Gather each relevant task's index
+    indexes = set()
+    for label in target_task_graph.graph.visit_postorder():
+        if label in do_not_optimize:
+            continue
+        _, strategy, arg = optimizations(label)
+        if isinstance(strategy, IndexSearch) and arg is not None:
+            indexes.update(arg)
+
+    index_to_taskid = {}
+    taskid_to_status = {}
+    if indexes:
+        # Find their respective status using TC index/queue batch APIs
+        indexes = list(indexes)
+        index_to_taskid = find_task_id_batched(indexes)
+        taskid_to_status = status_task_batched(list(index_to_taskid.values()))
+
     replaced_tasks = replace_tasks(
         target_task_graph=target_task_graph,
         optimizations=optimizations,
         params=params,
         do_not_optimize=do_not_optimize,
         label_to_taskid=label_to_taskid,
         existing_tasks=existing_tasks,
         removed_tasks=removed_tasks,
+        index_to_taskid=index_to_taskid,
+        taskid_to_status=taskid_to_status,
     )
 
     return (
         get_subgraph(
             target_task_graph,
             removed_tasks,
             replaced_tasks,
@@ -255,20 +278,25 @@
     target_task_graph,
     params,
     optimizations,
     do_not_optimize,
     label_to_taskid,
     removed_tasks,
     existing_tasks,
+    index_to_taskid,
+    taskid_to_status,
 ):
     """
     Implement the "Replacing Tasks" phase, returning a set of task labels of
     all replaced tasks. The replacement taskIds are added to label_to_taskid as
     a side-effect.
     """
+    # avoid circular import
+    from taskgraph.optimize.strategies import IndexSearch
+
     opt_counts = defaultdict(int)
     replaced = set()
     dependents_of = target_task_graph.graph.reverse_links_dict()
     dependencies_of = target_task_graph.graph.links_dict()
 
     for label in target_task_graph.graph.visit_postorder():
         logger.debug(f"replace_tasks: {label}")
@@ -303,24 +331,28 @@
         dependents = [target_task_graph.tasks[l] for l in dependents_of[label]]
         deadline = None
         if dependents:
             now = datetime.datetime.utcnow()
             deadline = max(
                 resolve_timestamps(now, task.task["deadline"]) for task in dependents
             )
+
+        if isinstance(opt, IndexSearch):
+            arg = arg, index_to_taskid, taskid_to_status
+
         repl = opt.should_replace_task(task, params, deadline, arg)
         if repl:
             if repl is True:
                 logger.debug(f"replace_tasks: {label} removed by optimization strategy")
                 # True means remove this task; get_subgraph will catch any
                 # problems with removed tasks being depended on
                 removed_tasks.add(label)
             else:
                 logger.debug(
-                    f"replace_tasks: {label} replaced by optimization strategy"
+                    f"replace_tasks: {label} replaced with {repl} by optimization strategy"
                 )
                 label_to_taskid[label] = repl
                 replaced.add(label)
             opt_counts[opt_by] += 1
             continue
         else:
             logger.debug(f"replace_tasks: {label} kept by optimization strategy")
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/optimize/strategies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from datetime import datetime
 
 from taskgraph.optimize.base import OptimizationStrategy, register_strategy
 from taskgraph.util.path import match as match_path
-from taskgraph.util.taskcluster import find_task_id, status_task
 
 logger = logging.getLogger(__name__)
 
 
 @register_strategy("index-search")
 class IndexSearch(OptimizationStrategy):
     # A task with no dependencies remaining after optimization will be replaced
@@ -18,33 +17,35 @@
     # - some changes altered the index_paths and new artifacts need to be
     # created.
     # In every of those cases, we need to run the task to create or refresh
     # artifacts.
 
     fmt = "%Y-%m-%dT%H:%M:%S.%fZ"
 
-    def should_replace_task(self, task, params, deadline, index_paths):
+    def should_replace_task(self, task, params, deadline, arg):
         "Look for a task with one of the given index paths"
+        index_paths, label_to_taskid, taskid_to_status = arg
+
         for index_path in index_paths:
             try:
-                task_id = find_task_id(index_path)
-                status = status_task(task_id)
+                task_id = label_to_taskid[index_path]
+                status = taskid_to_status[task_id]
                 # status can be `None` if we're in `testing` mode
                 # (e.g. test-action-callback)
                 if not status or status.get("state") in ("exception", "failed"):
                     continue
 
                 if deadline and datetime.strptime(
                     status["expires"], self.fmt
                 ) < datetime.strptime(deadline, self.fmt):
                     continue
 
                 return task_id
             except KeyError:
-                # 404 will end up here and go on to the next index path
+                # go on to the next index path
                 pass
 
         return False
 
 
 @register_strategy("skip-unless-changed")
 class SkipUnlessChanged(OptimizationStrategy):
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/parameters.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-8.1.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/task.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/chunking.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/__init__.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/common.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/index_search.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/run_task.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/run/toolchain.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/run/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/transforms/task_context.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/transforms/task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/path.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/set_name.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/set_name.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskcluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -189,14 +189,56 @@
     except requests.exceptions.HTTPError as e:
         if e.response.status_code == 404:
             raise KeyError(f"index path {index_path} not found")
         raise
     return response.json()["taskId"]
 
 
+def find_task_id_batched(index_paths, use_proxy=False):
+    """Gets the task id of multiple tasks given their respective index.
+
+    Args:
+        index_paths (List[str]): A list of task indexes.
+        use_proxy (bool): Whether to use taskcluster-proxy (default: False)
+
+    Returns:
+        Dict[str, str]: A dictionary object mapping each valid index path
+                        to its respective task id.
+
+    See the endpoint here:
+        https://docs.taskcluster.net/docs/reference/core/index/api#findTasksAtIndex
+    """
+    endpoint = liburls.api(get_root_url(use_proxy), "index", "v1", "tasks/indexes")
+    task_ids = {}
+    continuation_token = None
+
+    while True:
+        response = _do_request(
+            endpoint,
+            json={
+                "indexes": index_paths,
+            },
+            params={"continuationToken": continuation_token},
+        )
+
+        response_data = response.json()
+        if not response_data["tasks"]:
+            break
+        response_tasks = response_data["tasks"]
+        if (len(task_ids) + len(response_tasks)) > len(index_paths):
+            # Sanity check
+            raise ValueError("more task ids were returned than were asked for")
+        task_ids.update((t["namespace"], t["taskId"]) for t in response_tasks)
+
+        continuationToken = response_data.get("continuationToken")
+        if continuationToken is None:
+            break
+    return task_ids
+
+
 def get_artifact_from_index(index_path, artifact_path, use_proxy=False):
     full_path = index_path + "/artifacts/" + artifact_path
     response = _do_request(get_index_url(full_path, use_proxy))
     return _handle_artifact(full_path, response)
 
 
 def list_tasks(index_path, use_proxy=False):
@@ -267,14 +309,57 @@
         logger.info(f"Would have gotten status for {task_id}.")
     else:
         resp = _do_request(get_task_url(task_id, use_proxy) + "/status")
         status = resp.json().get("status", {})
         return status
 
 
+def status_task_batched(task_ids, use_proxy=False):
+    """Gets the status of multiple tasks given task_ids.
+
+    In testing mode, just logs that it would have retrieved statuses.
+
+    Args:
+        task_id (List[str]): A list of task ids.
+        use_proxy (bool): Whether to use taskcluster-proxy (default: False)
+
+    Returns:
+        dict: A dictionary object as defined here:
+          https://docs.taskcluster.net/docs/reference/platform/queue/api#statuses
+    """
+    if testing:
+        logger.info(f"Would have gotten status for {len(task_ids)} tasks.")
+        return
+    endpoint = liburls.api(get_root_url(use_proxy), "queue", "v1", "tasks/status")
+    statuses = {}
+    continuation_token = None
+
+    while True:
+        response = _do_request(
+            endpoint,
+            json={
+                "taskIds": task_ids,
+            },
+            params={
+                "continuationToken": continuation_token,
+            },
+        )
+        response_data = response.json()
+        if not response_data["statuses"]:
+            break
+        response_tasks = response_data["statuses"]
+        if (len(statuses) + len(response_tasks)) > len(task_ids):
+            raise ValueError("more task statuses were returned than were asked for")
+        statuses.update((t["taskId"], t["status"]) for t in response_tasks)
+        continuationToken = response_data.get("continuationToken")
+        if continuationToken is None:
+            break
+    return statuses
+
+
 def state_task(task_id, use_proxy=False):
     """Gets the state of a task given a task_id.
 
     In testing mode, just logs that it would have retrieved state. This is a subset of the
     data returned by :func:`status_task`.
 
     Args:
```

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/time.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-8.1.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.1.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_actions_registry.py` & `taskcluster-taskgraph-8.1.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_create.py` & `taskcluster-taskgraph-8.1.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_decision.py` & `taskcluster-taskgraph-8.1.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_docker.py` & `taskcluster-taskgraph-8.1.0/test/test_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_generator.py` & `taskcluster-taskgraph-8.1.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_graph.py` & `taskcluster-taskgraph-8.1.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_main.py` & `taskcluster-taskgraph-8.1.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_morph.py` & `taskcluster-taskgraph-8.1.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_optimize.py` & `taskcluster-taskgraph-8.1.0/test/test_optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,79 +265,83 @@
         optimizations=optimize_mod._get_optimizations(graph, strategies),
         **kwargs
     )
     assert got_removed == exp_removed
 
 
 @pytest.mark.parametrize(
-    "graph,kwargs,exp_replaced,exp_removed,exp_label_to_taskid",
+    "graph,kwargs,exp_replaced,exp_removed",
     (
         # A task cannot be replaced if it depends on one that was not replaced
         pytest.param(
             make_triangle(
                 t1={"replace": "e1"},
                 t3={"replace": "e3"},
             ),
-            {},
+            {
+                "index_to_taskid": {"t1": "e1"},
+            },
             # expectations
             {"t1"},
             set(),
-            {"t1": "e1"},
             id="blocked",
         ),
         # A task cannot be replaced if it should not be optimized
         pytest.param(
             make_triangle(
                 t1={"replace": "e1"},
                 t2={"replace": "xxx"},  # but do_not_optimize
                 t3={"replace": "e3"},
             ),
-            {"do_not_optimize": {"t2"}},
+            {
+                "do_not_optimize": {"t2"},
+                "index_to_taskid": {"t1": "e1"},
+            },
             # expectations
             {"t1"},
             set(),
-            {"t1": "e1"},
             id="do_not_optimize",
         ),
         # No tasks are replaced when strategy is 'never'
         pytest.param(
             make_triangle(),
             {},
             # expectations
             set(),
             set(),
-            {},
             id="never",
         ),
         # All replaceable tasks are replaced when strategy is 'replace'
         pytest.param(
             make_triangle(
                 t1={"replace": "e1"},
                 t2={"replace": "e2"},
                 t3={"replace": "e3"},
             ),
-            {},
+            {
+                "index_to_taskid": {"t1": "e1", "t2": "e2", "t3": "e3"},
+            },
             # expectations
             {"t1", "t2", "t3"},
             set(),
-            {"t1": "e1", "t2": "e2", "t3": "e3"},
             id="all",
         ),
         # A task can be replaced with nothing
         pytest.param(
             make_triangle(
                 t1={"replace": "e1"},
                 t2={"replace": True},
                 t3={"replace": True},
             ),
-            {},
+            {
+                "index_to_taskid": {"t1": "e1"},
+            },
             # expectations
             {"t1"},
             {"t2", "t3"},
-            {"t1": "e1"},
             id="tasks_removed",
         ),
         # A task which expires before a dependents deadline is not a valid replacement.
         pytest.param(
             make_graph(
                 make_task("t1", optimization={"replace": "e1"}),
                 make_task(
@@ -349,50 +353,49 @@
                 ("t2", "t1", "dep1"),
                 ("t3", "t1", "dep2"),
             ),
             {},
             # expectations
             set(),
             set(),
-            {},
             id="deadline",
         ),
     ),
 )
 def test_replace_tasks(
     graph,
     kwargs,
     exp_replaced,
     exp_removed,
-    exp_label_to_taskid,
 ):
     """Tests the `replace_tasks` function.
 
     Each test case takes five arguments:
 
     1. A `TaskGraph` instance.
     2. Keyword arguments to pass into `replace_tasks`.
     3. The set of task labels that are expected to be replaced.
     4. The set of task labels that are expected to be removed.
     5. The expected label_to_taskid.
     """
     kwargs.setdefault("params", {})
     kwargs.setdefault("do_not_optimize", set())
     kwargs.setdefault("label_to_taskid", {})
+    kwargs.setdefault("index_to_taskid", {})
+    kwargs.setdefault("taskid_to_status", {})
     kwargs.setdefault("removed_tasks", set())
     kwargs.setdefault("existing_tasks", {})
 
     got_replaced = optimize_mod.replace_tasks(
         target_task_graph=graph,
         optimizations=optimize_mod._get_optimizations(graph, default_strategies()),
         **kwargs
     )
     assert got_replaced == exp_replaced
     assert kwargs["removed_tasks"] == exp_removed
-    assert kwargs["label_to_taskid"] == exp_label_to_taskid
 
 
 @pytest.mark.parametrize(
     "graph,kwargs,exp_subgraph,exp_label_to_taskid",
     (
         # Test get_subgraph returns a similarly-shaped subgraph when nothing is removed
         pytest.param(
```

### Comparing `taskcluster-taskgraph-8.0.1/test/test_optimize_strategies.py` & `taskcluster-taskgraph-8.1.0/test/test_optimize_strategies.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Any copyright is dedicated to the public domain.
 # http://creativecommons.org/publicdomain/zero/1.0/
 
-import os
 from datetime import datetime
 from test.fixtures.gen import make_task
 from time import mktime
 
 import pytest
 
 from taskgraph.optimize.strategies import IndexSearch, SkipUnlessChanged
@@ -40,39 +39,33 @@
         (
             "failed",
             "2021-06-08T14:53:16.937Z",
             False,
         ),
     ),
 )
-def test_index_search(responses, params, state, expires, expected):
+def test_index_search(state, expires, expected):
     taskid = "abc"
     index_path = "foo.bar.latest"
-    responses.add(
-        responses.GET,
-        f"{os.environ['TASKCLUSTER_ROOT_URL']}/api/index/v1/task/{index_path}",
-        json={"taskId": taskid},
-        status=200,
-    )
-
-    responses.add(
-        responses.GET,
-        f"{os.environ['TASKCLUSTER_ROOT_URL']}/api/queue/v1/task/{taskid}/status",
-        json={
-            "status": {
-                "state": state,
-                "expires": expires,
-            }
-        },
-        status=200,
-    )
+    label_to_taskid = {index_path: taskid}
+    taskid_to_status = {
+        taskid: {
+            "state": state,
+            "expires": expires,
+        }
+    }
 
     opt = IndexSearch()
     deadline = "2021-06-07T19:03:20.482Z"
-    assert opt.should_replace_task({}, params, deadline, (index_path,)) == expected
+    assert (
+        opt.should_replace_task(
+            {}, params, deadline, ((index_path,), label_to_taskid, taskid_to_status)
+        )
+        == expected
+    )
 
 
 @pytest.mark.parametrize(
     "params,file_patterns,should_optimize",
     (
         pytest.param({"files_changed": []}, ["foo.txt"], True, id="no files changed"),
         pytest.param(
```

### Comparing `taskcluster-taskgraph-8.0.1/test/test_parameters.py` & `taskcluster-taskgraph-8.1.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-8.1.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_scripts_run_task.py` & `taskcluster-taskgraph-8.1.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_target_tasks.py` & `taskcluster-taskgraph-8.1.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_taskgraph.py` & `taskcluster-taskgraph-8.1.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transform_chunking.py` & `taskcluster-taskgraph-8.1.0/test/test_transform_chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transform_docker_image.py` & `taskcluster-taskgraph-8.1.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transform_task_context.py` & `taskcluster-taskgraph-8.1.0/test/test_transform_task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_base.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_cached_tasks.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_fetch.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_notify.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_run.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_run.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_run_run_task.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_run_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_run_toolchain.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_run_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_transforms_task.py` & `taskcluster-taskgraph-8.1.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_archive.py` & `taskcluster-taskgraph-8.1.0/test/test_util_archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_attributes.py` & `taskcluster-taskgraph-8.1.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_cached_tasks.py` & `taskcluster-taskgraph-8.1.0/test/test_util_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_dependencies.py` & `taskcluster-taskgraph-8.1.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_docker.py` & `taskcluster-taskgraph-8.1.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_parameterization.py` & `taskcluster-taskgraph-8.1.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_path.py` & `taskcluster-taskgraph-8.1.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_python_path.py` & `taskcluster-taskgraph-8.1.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_readonlydict.py` & `taskcluster-taskgraph-8.1.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_schema.py` & `taskcluster-taskgraph-8.1.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_taskcluster.py` & `taskcluster-taskgraph-8.1.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_templates.py` & `taskcluster-taskgraph-8.1.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_time.py` & `taskcluster-taskgraph-8.1.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_treeherder.py` & `taskcluster-taskgraph-8.1.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_vcs.py` & `taskcluster-taskgraph-8.1.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_verify.py` & `taskcluster-taskgraph-8.1.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_workertypes.py` & `taskcluster-taskgraph-8.1.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-8.0.1/test/test_util_yaml.py` & `taskcluster-taskgraph-8.1.0/test/test_util_yaml.py`

 * *Files identical despite different names*


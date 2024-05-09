# Comparing `tmp/netbox-data-flows-0.8.2.tar.gz` & `tmp/netbox_data_flows-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-data-flows-0.8.2.tar", last modified: Mon Jan 29 21:11:33 2024, max compression
+gzip compressed data, was "netbox_data_flows-0.8.3.tar", last modified: Thu May  9 17:22:44 2024, max compression
```

## Comparing `netbox-data-flows-0.8.2.tar` & `netbox_data_flows-0.8.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.060744 netbox-data-flows-0.8.2/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.060744 netbox-data-flows-0.8.2/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.064744 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.064744 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.064744 netbox-data-flows-0.8.2/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.064744 netbox-data-flows-0.8.2/netbox_data_flows/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.064744 netbox-data-flows-0.8.2/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.064744 netbox-data-flows-0.8.2/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.068744 netbox-data-flows-0.8.2/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.068744 netbox-data-flows-0.8.2/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.068744 netbox-data-flows-0.8.2/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.060744 netbox-data-flows-0.8.2/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/model_tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-01-29 21:11:33.000000 netbox-data-flows-0.8.2/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-01-29 21:11:33.000000 netbox-data-flows-0.8.2/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:11:33.000000 netbox-data-flows-0.8.2/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:11:32.000000 netbox-data-flows-0.8.2/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-29 21:11:33.000000 netbox-data-flows-0.8.2/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-29 21:11:19.000000 netbox-data-flows-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 21:11:33.072744 netbox-data-flows-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.163002 netbox_data_flows-0.8.3/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7591 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.167002 netbox_data_flows-0.8.3/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/graphql/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.171002 netbox_data_flows-0.8.3/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    14554 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/0010_alter_objectaliastarget_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.159002 netbox_data_flows-0.8.3/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.175002 netbox_data_flows-0.8.3/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/model_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:22:43.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 17:22:44.000000 netbox_data_flows-0.8.3/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 17:22:29.000000 netbox_data_flows-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:22:44.179002 netbox_data_flows-0.8.3/setup.cfg
```

### Comparing `netbox-data-flows-0.8.2/LICENSE` & `netbox_data_flows-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/PKG-INFO` & `netbox_data_flows-0.8.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.8.2
+Version: 0.8.3
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
@@ -34,17 +34,19 @@
 
 ## Installation and Configuration
 
 Full reference: [Using Plugins - NetBox Documentation](https://docs.netbox.dev/en/stable/plugins/)
 
 ### Requirements
 
-* NetBox (>=3.6.0)
+* NetBox (=3.7.x)
 * Python 3.8 or higher
 
+This is the last version compatible with NetBox 3. Future releases will support 4.0 only.
+
 *Note:* the plugin uses some classes that are not explicitely exported in 
 NetBox's plugin API, such as MPTT Tree-based models. Upward compatiblity is
 not guaranteed.
 
 ### Temporary installation
 
 Install the Python package:
```

### Comparing `netbox-data-flows-0.8.2/README.md` & `netbox_data_flows-0.8.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 
 ## Installation and Configuration
 
 Full reference: [Using Plugins - NetBox Documentation](https://docs.netbox.dev/en/stable/plugins/)
 
 ### Requirements
 
-* NetBox (>=3.6.0)
+* NetBox (=3.7.x)
 * Python 3.8 or higher
 
+This is the last version compatible with NetBox 3. Future releases will support 4.0 only.
+
 *Note:* the plugin uses some classes that are not explicitely exported in 
 NetBox's plugin API, such as MPTT Tree-based models. Upward compatiblity is
 not guaranteed.
 
 ### Temporary installation
 
 Install the Python package:
```

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/__init__.py` & `netbox_data_flows-0.8.3/netbox_data_flows/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
     description = (
         "NetBox plugin to document data flows between "
         "systems and applications."
     )
     version = __version__
     base_url = "data-flows"
     author = "Thomas Fargeix"
     required_settings = []
     default_settings = {}
-    min_version = "3.6.0"
+    min_version = "3.7.0"
+    max_version = "3.7.9"
 
     def ready(self):
         from . import signals  # noqa: F401
 
         super().ready()
```

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/dataflows.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/groups.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/nested.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/nested.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/serializers/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/urls.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/api/views.py` & `netbox_data_flows-0.8.3/netbox_data_flows/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/choices.py` & `netbox_data_flows-0.8.3/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/filtersets/addins.py` & `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/filtersets/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/filtersets/dataflows.py` & `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/filtersets/filters.py` & `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/filtersets/groups.py` & `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/filtersets/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/filtersets/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/forms/applicationroles.py` & `netbox_data_flows-0.8.3/netbox_data_flows/forms/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/forms/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/forms/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/forms/dataflows.py` & `netbox_data_flows-0.8.3/netbox_data_flows/forms/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/forms/groups.py` & `netbox_data_flows-0.8.3/netbox_data_flows/forms/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/forms/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/forms/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/graphql/__init__.py` & `netbox_data_flows-0.8.3/netbox_data_flows/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/graphql/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/graphql/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/graphql/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/graphql/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/migrations/0001_initial.py` & `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py` & `netbox_data_flows-0.8.3/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/models/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/models/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/models/dataflows.py` & `netbox_data_flows-0.8.3/netbox_data_flows/models/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/models/groups.py` & `netbox_data_flows-0.8.3/netbox_data_flows/models/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/models/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/models/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/navigation.py` & `netbox_data_flows-0.8.3/netbox_data_flows/navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from extras.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
+from netbox.plugins import PluginMenu, PluginMenuButton, PluginMenuItem
 from utilities.choices import ButtonColorChoices
 
 
 #
 # Utility functions
 #
```

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/search.py` & `netbox_data_flows-0.8.3/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/tables/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/tables/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/tables/dataflows.py` & `netbox_data_flows-0.8.3/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/tables/groups.py` & `netbox_data_flows-0.8.3/netbox_data_flows/tables/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/tables/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/tables/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox_data_flows-0.8.3/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/urls.py` & `netbox_data_flows-0.8.3/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/utils/aliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/utils/helpers.py` & `netbox_data_flows-0.8.3/netbox_data_flows/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/views/applicationroles.py` & `netbox_data_flows-0.8.3/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/views/applications.py` & `netbox_data_flows-0.8.3/netbox_data_flows/views/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/views/dataflows.py` & `netbox_data_flows-0.8.3/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/views/groups.py` & `netbox_data_flows-0.8.3/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/views/model_tabs.py` & `netbox_data_flows-0.8.3/netbox_data_flows/views/model_tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             model,
             name="dataflows-tab",
             path="dataflows",
         )(cls)
 
     queryset = None
     template_name = "netbox_data_flows/dataflow_tab.html"
-    actions = ("changelog",)
+    # Todo: actions = unlink
 
     tab = ViewTab(
         label="Data Flows",
         permission="netbox_data_flows.view_dataflow",
         badge=_count_related_aliases_or_dataflows,
         hide_if_empty=True,
     )
```

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows/views/objectaliases.py` & `netbox_data_flows-0.8.3/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows.egg-info/PKG-INFO` & `netbox_data_flows-0.8.3/netbox_data_flows.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.8.2
+Version: 0.8.3
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
@@ -34,17 +34,19 @@
 
 ## Installation and Configuration
 
 Full reference: [Using Plugins - NetBox Documentation](https://docs.netbox.dev/en/stable/plugins/)
 
 ### Requirements
 
-* NetBox (>=3.6.0)
+* NetBox (=3.7.x)
 * Python 3.8 or higher
 
+This is the last version compatible with NetBox 3. Future releases will support 4.0 only.
+
 *Note:* the plugin uses some classes that are not explicitely exported in 
 NetBox's plugin API, such as MPTT Tree-based models. Upward compatiblity is
 not guaranteed.
 
 ### Temporary installation
 
 Install the Python package:
```

### Comparing `netbox-data-flows-0.8.2/netbox_data_flows.egg-info/SOURCES.txt` & `netbox_data_flows-0.8.3/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.8.2/pyproject.toml` & `netbox_data_flows-0.8.3/pyproject.toml`

 * *Files identical despite different names*


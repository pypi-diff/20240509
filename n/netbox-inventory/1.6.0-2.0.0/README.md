# Comparing `tmp/netbox_inventory-1.6.0.tar.gz` & `tmp/netbox_inventory-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_inventory-1.6.0.tar", last modified: Thu Apr 18 14:53:17 2024, max compression
+gzip compressed data, was "netbox_inventory-2.0.0.tar", last modified: Thu May  9 15:09:56 2024, max compression
```

## Comparing `netbox_inventory-1.6.0.tar` & `netbox_inventory-2.0.0.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.580691 netbox_inventory-1.6.0/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/analyzers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.580691 netbox_inventory-1.6.0/netbox_inventory/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/nested_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15610 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.584691 netbox_inventory-1.6.0/netbox_inventory/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)    21988 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/bulk.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/bulk_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/forms/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.572691 netbox_inventory-1.6.0/netbox_inventory/management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.584691 netbox_inventory-1.6.0/netbox_inventory/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/management/commands/check_asset_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.584691 netbox_inventory-1.6.0/netbox_inventory/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0001_initial_prod.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0002_alter_asset_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/0006_purchase_status.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18925 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.572691 netbox_inventory-1.6.0/netbox_inventory/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset.html
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_create.html
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/delivery.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/purchase.html
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/supplier.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/tests/asset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/custom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.588692 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.592692 netbox_inventory-1.6.0/netbox_inventory/views/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/asset_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/purchase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/supplier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/netbox_inventory/views/tabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/netbox_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 14:53:17.000000 netbox_inventory-1.6.0/netbox_inventory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 14:53:11.000000 netbox_inventory-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:53:17.596691 netbox_inventory-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.918429 netbox_inventory-2.0.0/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/analyzers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.918429 netbox_inventory-2.0.0/netbox_inventory/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/nested_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15610 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.918429 netbox_inventory-2.0.0/netbox_inventory/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/bulk_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/forms/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.914429 netbox_inventory-2.0.0/netbox_inventory/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.922429 netbox_inventory-2.0.0/netbox_inventory/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/management/commands/check_asset_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.922429 netbox_inventory-2.0.0/netbox_inventory/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0001_initial_prod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0002_alter_asset_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0006_purchase_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/0007_alter_asset_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19653 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.914429 netbox_inventory-2.0.0/netbox_inventory/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.922429 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_assign.html
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_create.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/delivery.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/purchase.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/supplier.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/custom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.926429 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/asset_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/purchase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/supplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/netbox_inventory/views/tabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/netbox_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 15:09:56.000000 netbox_inventory-2.0.0/netbox_inventory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 15:09:34.000000 netbox_inventory-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:09:56.930429 netbox_inventory-2.0.0/setup.cfg
```

### Comparing `netbox_inventory-1.6.0/LICENSE` & `netbox_inventory-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/PKG-INFO` & `netbox_inventory-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.6.0
+Version: 2.0.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NetBox Inventory Plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin for hardware inventory.
 
@@ -67,24 +67,21 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.7.x to work. Older versions of the plugin
+This plugin requires netbox version 4.0 to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|       3.3      |      1.1.x     |
-|       3.4      |      1.2.x     |
-|       3.5      | 1.3.x & 1.4.x  |
-|       3.6      |      1.5.x     |
 |       3.7      |      1.6.x     |
+|       4.0      |      2.0.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox_inventory-1.6.0/README.md` & `netbox_inventory-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,24 +52,21 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.7.x to work. Older versions of the plugin
+This plugin requires netbox version 4.0 to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|       3.3      |      1.1.x     |
-|       3.4      |      1.2.x     |
-|       3.5      | 1.3.x & 1.4.x  |
-|       3.6      |      1.5.x     |
 |       3.7      |      1.6.x     |
+|       4.0      |      2.0.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/__init__.py` & `netbox_inventory-2.0.0/netbox_inventory/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from extras.plugins import PluginConfig
+from netbox.plugins import PluginConfig
 from .version import __version__
 
 
 class NetBoxInventoryConfig(PluginConfig):
     name = 'netbox_inventory'
     verbose_name = 'NetBox Inventory'
     version = __version__
     description = 'Inventory asset management in NetBox'
     author = 'Matej Vadnjal'
     author_email = 'matej.vadnjal@arnes.si'
     base_url = 'inventory'
-    min_version = '3.7.0'
+    min_version = '4.0.0'
     default_settings = {
         'top_level_menu': True,
         'used_status_name': 'used',
         'stored_status_name': 'stored',
         'sync_hardware_serial_asset_tag': False,
         'asset_import_create_purchase': False,
         'asset_import_create_device_type': False,
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/analyzers.py` & `netbox_inventory-2.0.0/netbox_inventory/analyzers.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/api/serializers.py` & `netbox_inventory-2.0.0/netbox_inventory/api/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,20 @@
 from rest_framework import serializers
 
 from dcim.api.serializers import (
-    NestedDeviceTypeSerializer, NestedDeviceSerializer,
-    NestedManufacturerSerializer,
-    NestedModuleTypeSerializer, NestedModuleSerializer,
-    NestedInventoryItemSerializer, NestedLocationSerializer
+    DeviceTypeSerializer, DeviceSerializer, ManufacturerSerializer,
+    ModuleTypeSerializer, ModuleSerializer, InventoryItemSerializer,
+    LocationSerializer
 )
-from tenancy.api.serializers import NestedContactSerializer, NestedTenantSerializer
-from netbox.api.serializers import NetBoxModelSerializer
+from tenancy.api.serializers import ContactSerializer, TenantSerializer
+from netbox.api.serializers import NestedGroupModelSerializer, NetBoxModelSerializer
 from .nested_serializers import *
 from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
-class AssetSerializer(NetBoxModelSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netbox_inventory-api:asset-detail'
-    )
-    device_type = NestedDeviceTypeSerializer(required=False, allow_null=True, default=None)
-    device = NestedDeviceSerializer(required=False, allow_null=True, default=None)
-    module_type = NestedModuleTypeSerializer(required=False, allow_null=True, default=None)
-    module = NestedModuleSerializer(required=False, allow_null=True, default=None)
-    inventoryitem_type = NestedInventoryItemTypeSerializer(required=False, allow_null=True, default=None) 
-    inventoryitem = NestedInventoryItemSerializer(required=False, allow_null=True, default=None)
-    storage_location = NestedLocationSerializer(required=False, allow_null=True, default=None)
-    delivery = NestedDeliverySerializer(required=False, allow_null=True, default=None)
-    purchase = NestedPurchaseSerializer(required=False, allow_null=True, default=None)
-    tenant = NestedTenantSerializer(required=False, allow_null=True, default=None)
-    contact = NestedContactSerializer(required=False, allow_null=True, default=None)
-    owner = NestedTenantSerializer(required=False, allow_null=True, default=None)
-
-    def to_internal_value(self, data):
-        ret = super().to_internal_value(data)
-        # if only delivery set, infer pruchase from it
-        if 'delivery' in ret and ret['delivery'] and not ret.get('purchase'):
-            ret['purchase'] = ret['delivery'].purchase
-        if 'asset_tag' in ret and ret['asset_tag'] == '':
-            ret['asset_tag'] = None
-        if 'serial' in ret and ret['serial'] == '':
-            ret['serial'] = None
-        return ret
-
-    class Meta:
-        model = Asset
-        fields = (
-            'id', 'url', 'display', 'name', 'asset_tag', 'serial', 'status',
-            'kind', 'device_type', 'device', 'module_type', 'module', 'inventoryitem_type','inventoryitem', 
-            'tenant', 'contact', 'storage_location', 'owner', 'delivery', 'purchase',
-            'warranty_start', 'warranty_end',
-            'comments', 'tags', 'custom_fields', 'created', 'last_updated'
-        )
-        # DRF autiomatically creates validator from model's unique_together contraints
-        # that doesn't work if we allow some filelds in a unique_together to be null
-        # so we remove DRF's auto generated validators and rely on model's validation
-        # logic to handle validation
-        # see  https://www.django-rest-framework.org/api-guide/validators/#optional-fields
-        validators = []
-
-
 class SupplierSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:supplier-detail'
     )
     asset_count = serializers.IntegerField(read_only=True)
     purchase_count = serializers.IntegerField(read_only=True)
     delivery_count = serializers.IntegerField(read_only=True)
@@ -68,72 +22,124 @@
     class Meta:
         model = Supplier
         fields = (
             'id', 'url', 'display', 'name', 'slug', 'description', 'comments',
             'tags', 'custom_fields', 'created', 'last_updated', 'asset_count',
             'purchase_count', 'delivery_count',
         )
+        brief_fields = ('id', 'url', 'display', 'name', 'slug', 'description')
 
 
 class PurchaseSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:purchase-detail'
     )
-    supplier = NestedSupplierSerializer()
+    supplier = SupplierSerializer(nested=True)
     asset_count = serializers.IntegerField(read_only=True)
     delivery_count = serializers.IntegerField(read_only=True)
     
     class Meta:
         model = Purchase
         fields = (
             'id', 'url', 'display', 'supplier', 'name', 'status', 'date', 'description',
             'comments', 'tags', 'custom_fields', 'created', 'last_updated',
             'asset_count', 'delivery_count',
         )
+        brief_fields = ('id', 'url', 'display', 'supplier', 'name', 'status', 'date', 'description')
 
 
 class DeliverySerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:delivery-detail'
     )
-    purchase = NestedPurchaseSerializer()
-    receiving_contact = NestedContactSerializer(required=False, allow_null=True, default=None)
+    purchase = PurchaseSerializer(nested=True)
+    receiving_contact = ContactSerializer(nested=True, required=False, allow_null=True, default=None)
     asset_count = serializers.IntegerField(read_only=True)
     
     class Meta:
         model = Delivery
         fields = (
             'id', 'url', 'display', 'purchase', 'name', 'date', 'description', 'comments',
             'receiving_contact', 'tags', 'custom_fields', 'created', 'last_updated', 'asset_count',
         )
+        brief_fields = ('id', 'url', 'display', 'name', 'date', 'description')
+
+
+class InventoryItemGroupSerializer(NestedGroupModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_inventory-api:inventoryitemgroup-detail'
+    )
+    parent = NestedInventoryItemGroupSerializer(required=False, allow_null=True, default=None)
+    asset_count = serializers.IntegerField(read_only=True)
+
+    class Meta:
+        model = InventoryItemGroup
+        fields = (
+            'id', 'url', 'display', 'name', 'parent', 'comments', 'tags', 'custom_fields',
+            'created', 'last_updated', 'asset_count', '_depth',
+        )
+        brief_fields = ('id', 'url', 'display', 'name', '_depth')
 
 
 class InventoryItemTypeSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_inventory-api:inventoryitemtype-detail'
     )
-    manufacturer = NestedManufacturerSerializer()
-    inventoryitem_group = NestedInventoryItemGroupSerializer(required=False, allow_null=True, default=None)
+    manufacturer = ManufacturerSerializer(nested=True)
+    inventoryitem_group = InventoryItemGroupSerializer(nested=True, required=False, allow_null=True, default=None)
     asset_count = serializers.IntegerField(read_only=True)
     
     class Meta:
         model = InventoryItemType
         fields = (
             'id', 'url', 'display', 'model', 'slug', 'manufacturer', 'part_number',
             'inventoryitem_group', 'comments', 'tags', 'custom_fields', 'created',
             'last_updated', 'asset_count',
         )
+        brief_fields = ('id', 'url', 'display', 'manufacturer', 'model', 'slug')
 
 
-class InventoryItemGroupSerializer(NetBoxModelSerializer):
+class AssetSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netbox_inventory-api:inventoryitemgroup-detail'
+        view_name='plugins-api:netbox_inventory-api:asset-detail'
     )
-    parent = NestedInventoryItemGroupSerializer(required=False, allow_null=True, default=None)
-    asset_count = serializers.IntegerField(read_only=True)
-    
+    device_type = DeviceTypeSerializer(nested=True, required=False, allow_null=True, default=None)
+    device = DeviceSerializer(nested=True, required=False, allow_null=True, default=None)
+    module_type = ModuleTypeSerializer(nested=True, required=False, allow_null=True, default=None)
+    module = ModuleSerializer(nested=True, required=False, allow_null=True, default=None)
+    inventoryitem_type = InventoryItemTypeSerializer(nested=True, required=False, allow_null=True, default=None) 
+    inventoryitem = InventoryItemSerializer(nested=True, required=False, allow_null=True, default=None)
+    storage_location = LocationSerializer(nested=True, required=False, allow_null=True, default=None)
+    delivery = DeliverySerializer(nested=True, required=False, allow_null=True, default=None)
+    purchase = PurchaseSerializer(nested=True, required=False, allow_null=True, default=None)
+    tenant = TenantSerializer(nested=True, required=False, allow_null=True, default=None)
+    contact = ContactSerializer(nested=True, required=False, allow_null=True, default=None)
+    owner = TenantSerializer(nested=True, required=False, allow_null=True, default=None)
+
+    def to_internal_value(self, data):
+        ret = super().to_internal_value(data)
+        # if only delivery set, infer pruchase from it
+        if 'delivery' in ret and ret['delivery'] and not ret.get('purchase'):
+            ret['purchase'] = ret['delivery'].purchase
+        if 'asset_tag' in ret and ret['asset_tag'] == '':
+            ret['asset_tag'] = None
+        if 'serial' in ret and ret['serial'] == '':
+            ret['serial'] = None
+        return ret
+
     class Meta:
-        model = InventoryItemGroup
+        model = Asset
         fields = (
-            'id', 'url', 'display', 'name', 'parent', 'comments', 'tags', 'custom_fields',
-            'created', 'last_updated', 'asset_count',
+            'id', 'url', 'display', 'name', 'asset_tag', 'serial', 'status',
+            'kind', 'device_type', 'device', 'module_type', 'module', 'inventoryitem_type','inventoryitem', 
+            'tenant', 'contact', 'storage_location', 'owner', 'delivery', 'purchase',
+            'warranty_start', 'warranty_end',
+            'comments', 'tags', 'custom_fields', 'created', 'last_updated'
         )
+        brief_fields = ('id', 'url', 'display', 'serial', 'name')
+        # DRF autiomatically creates validator from model's unique_together contraints
+        # that doesn't work if we allow some filelds in a unique_together to be null
+        # so we remove DRF's auto generated validators and rely on model's validation
+        # logic to handle validation
+        # see  https://www.django-rest-framework.org/api-guide/validators/#optional-fields
+        validators = []
+
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/api/urls.py` & `netbox_inventory-2.0.0/netbox_inventory/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/api/views.py` & `netbox_inventory-2.0.0/netbox_inventory/api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dcim.api.views import DeviceViewSet, InventoryItemViewSet, ModuleViewSet
 from netbox.api.viewsets import NetBoxModelViewSet
-from utilities.utils import count_related
+from utilities.query import count_related
 from .. import filtersets, models
 from .serializers import (
     AssetSerializer, InventoryItemTypeSerializer, InventoryItemGroupSerializer,
     DeliverySerializer, PurchaseSerializer, SupplierSerializer
 )
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/choices.py` & `netbox_inventory-2.0.0/netbox_inventory/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/filtersets.py` & `netbox_inventory-2.0.0/netbox_inventory/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/forms/assign.py` & `netbox_inventory-2.0.0/netbox_inventory/forms/assign.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django import forms
 
 from dcim.models import Device, InventoryItem, Module, Site
 from netbox.forms import NetBoxModelForm
 from tenancy.models import Contact, Tenant
 from utilities.forms.fields import DynamicModelChoiceField
+from utilities.forms.rendering import FieldSet
 from utilities.forms.widgets import APISelect
 from ..models import Asset
 
 __all__ = (
     'AssetDeviceAssignForm',
     'AssetModuleAssignForm',
     'AssetInventoryItemAssignForm',
@@ -89,17 +90,17 @@
             attrs={
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
-        ('Asset', ('device_type', 'name')),
-        ('Device', ('site', 'device')),
-        ('Assigned to', ('tenant', 'contact')),
+        FieldSet('device_type', 'name', name='Asset'),
+        FieldSet('site', 'device', name='Device'),
+        FieldSet('tenant', 'contact', name='Assigned to'),
     )
 
     class Meta:
         model = Asset
         fields = ('device_type', 'name', 'site', 'device', 'tenant', 'contact')
         widgets = {'device_type': forms.HiddenInput()}
 
@@ -127,17 +128,17 @@
             attrs={
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
-        ('Asset', ('module_type', 'name')),
-        ('Module', ('device', 'module',)),
-        ('Tenancy', ('tenant', 'contact')),
+        FieldSet('module_type', 'name', name='Asset'),
+        FieldSet('device', 'module', name='Module'),
+        FieldSet('tenant', 'contact', name='Tenancy'),
     )
 
     class Meta:
         model = Asset
         fields = ('module_type', 'name', 'device', 'module', 'tenant', 'contact')
         widgets = {'module_type': forms.HiddenInput()}
 
@@ -171,17 +172,17 @@
             attrs={
                 'data-static-params': '[{"queryParam":"has_asset_assigned","queryValue":"false"}]',
             },
         )
     )
 
     fieldsets = (
-        ('Asset', ('inventoryitem_type', 'name')),
-        ('Inventory Item', ('device', 'inventoryitem')),
-        ('Tenancy', ('tenant', 'contact')),
+        FieldSet('inventoryitem_type', 'name', name='Asset'),
+        FieldSet('device', 'inventoryitem', name='Inventory Item'),
+        FieldSet('tenant', 'contact', name='Tenancy'),
     )
 
     class Meta:
         model = Asset
         fields = ('inventoryitem_type', 'name', 'device', 'inventoryitem', 'tenant', 'contact')
         widgets = {'inventoryitem_type': forms.HiddenInput()}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/forms/bulk.py` & `netbox_inventory-2.0.0/netbox_inventory/forms/bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelBulkEditForm, NetBoxModelImportForm
 from utilities.forms import add_blank_choice
 from utilities.forms.fields import (
     CommentField, CSVChoiceField, CSVModelChoiceField,
     DynamicModelChoiceField
 )
+from utilities.forms.rendering import FieldSet
 from utilities.forms.widgets import DatePicker
 from tenancy.models import Contact, Tenant
 from ..choices import AssetStatusChoices, HardwareKindChoices, PurchaseStatusChoices
 from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_plugin_setting
 
 __all__ = (
@@ -102,19 +103,19 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = Asset
     fieldsets = (
-        ('General', ('name', 'status')),
-        ('Hardware', ('device_type', 'device', 'module_type', 'module')),
-        ('Purchase', ('owner', 'purchase', 'delivery', 'warranty_start', 'warranty_end')), 
-        ('Assigned to', ('tenant', 'contact')), 
-        ('Location', ('storage_location',)),
+        FieldSet('name', 'status', name='General'),
+        FieldSet('device_type', 'device', 'module_type', 'module', name='Hardware'),
+        FieldSet('owner', 'purchase', 'delivery', 'warranty_start', 'warranty_end', name='Purchase'), 
+        FieldSet('tenant', 'contact', name='Assigned to'), 
+        FieldSet('storage_location', name='Location'),
     )
     nullable_fields = (
         'name', 'device', 'module', 'owner', 'purchase', 'delivery', 'tenant', 'contact',
         'warranty_start', 'warranty_end',
     )
 
 
@@ -423,15 +424,15 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = Supplier
     fieldsets = (
-        ('General', ('description',)),
+        FieldSet('description', name='General'),
     )
     nullable_fields = ('description',)
 
 
 class PurchaseImportForm(NetBoxModelImportForm):
     supplier = CSVModelChoiceField(
         queryset=Supplier.objects.all(),
@@ -472,15 +473,15 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = Purchase
     fieldsets = (
-        ('General', ('date', 'status', 'supplier', 'description',)),
+        FieldSet('date', 'status', 'supplier', 'description', name='General'),
     )
     nullable_fields = ('date', 'description',)
 
 
 class DeliveryImportForm(NetBoxModelImportForm):
     purchase = CSVModelChoiceField(
         queryset=Purchase.objects.all(),
@@ -523,15 +524,15 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = Delivery
     fieldsets = (
-        ('General', ('date', 'purchase', 'receiving_contact', 'description',)),
+        FieldSet('date', 'purchase', 'receiving_contact', 'description', name='General'),
     )
     nullable_fields = ('date', 'description', 'receiving_contact',)
 
 
 class InventoryItemTypeImportForm(NetBoxModelImportForm):
     manufacturer = CSVModelChoiceField(
         queryset=Manufacturer.objects.all(),
@@ -566,15 +567,15 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = InventoryItemType
     fieldsets = (
-        ('Inventory Item Type', ('manufacturer', 'inventoryitem_group')),
+        FieldSet('manufacturer', 'inventoryitem_group', name='Inventory Item Type'),
     )
     nullable_fields = (
         'inventoryitem_group',
     )
 
 
 class InventoryItemGroupImportForm(NetBoxModelImportForm):
@@ -598,10 +599,10 @@
     )
     comments = CommentField(
         required=False,
     )
 
     model = InventoryItemGroup
     fieldsets = (
-        (None, ('parent',)),
+        FieldSet('parent'),
     )
-    nullable_fields = ('parent',)
+    nullable_fields = ('parent',)
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/forms/create.py` & `netbox_inventory-2.0.0/netbox_inventory/forms/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
-from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 
+from core.models import ObjectType
 from dcim.forms import DeviceForm, InventoryItemForm, ModuleForm
 from dcim.models import Device
 from utilities.forms.fields import DynamicModelChoiceField
 from ..utils import get_plugin_setting
 
 __all__ = (
     'AssetDeviceCreateForm',
@@ -120,13 +120,13 @@
         component_set = None
         for field_name in COMPONENT_FIELDS:
             field_value = self.cleaned_data.get(field_name)
             if field_value and component_set:
                 raise ValidationError('Only a single component can be selected')
             if field_value:
                 component_set = field_name
-                self.cleaned_data['component_type'] = ContentType.objects.get(app_label='dcim', model=field_name)
+                self.cleaned_data['component_type'] = ObjectType.objects.get(app_label='dcim', model=field_name)
                 self.cleaned_data['component_id'] = field_value.pk
                 self.cleaned_data.pop(field_name)
 
     def clean_manufacturer(self):
         return self.instance.assigned_asset.inventoryitem_type.manufacturer
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/forms/filters.py` & `netbox_inventory-2.0.0/netbox_inventory/forms/filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django import forms
 
 from dcim.models import Device, DeviceType, Manufacturer, ModuleType, Site, Location, Rack
 from netbox.forms import NetBoxModelFilterSetForm
 from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES
 from utilities.forms.fields import DynamicModelMultipleChoiceField, TagFilterField
+from utilities.forms.rendering import FieldSet
 from utilities.forms.widgets import DatePicker
 from tenancy.forms import ContactModelFilterForm
 from tenancy.models import Contact, Tenant
 from ..choices import HardwareKindChoices, AssetStatusChoices, PurchaseStatusChoices
 from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 
 
@@ -20,31 +21,34 @@
     'InventoryItemGroupFilterForm',
 )
 
 
 class AssetFilterForm(NetBoxModelFilterSetForm):
     model = Asset
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag', 'status')),
-        ('Hardware', (
+        FieldSet('q', 'filter_id', 'tag', 'status'),
+        FieldSet(
             'kind', 'manufacturer_id', 'device_type_id', 'module_type_id',
-            'inventoryitem_type_id', 'inventoryitem_group_id', 'is_assigned'
-        )),
-        ('Usage', ('tenant_id', 'contact_id')),
-        ('Purchase', (
+            'inventoryitem_type_id', 'inventoryitem_group_id', 'is_assigned',
+            name='Hardware'
+        ),
+        FieldSet('tenant_id', 'contact_id', name='Usage'),
+        FieldSet(
             'owner_id', 'delivery_id', 'purchase_id', 'supplier_id',
             'delivery_date_after', 'delivery_date_before', 'purchase_date_after',
             'purchase_date_before', 'warranty_start_after', 'warranty_start_before',
-            'warranty_end_after', 'warranty_end_before'
-        )),
-        ('Location', (
+            'warranty_end_after', 'warranty_end_before',
+            name='Purchase'
+        ),
+        FieldSet(
             'storage_site_id', 'storage_location_id', 'installed_site_id', 
             'installed_location_id', 'installed_rack_id', 'installed_device_id',
             'located_site_id', 'located_location_id',
-        )),
+            name='Location',
+        ),
     )
 
     status = forms.MultipleChoiceField(
         choices=AssetStatusChoices,
         required=False,
     )
     kind = forms.MultipleChoiceField(
@@ -240,26 +244,26 @@
     )
     tag = TagFilterField(model)
 
 
 class SupplierFilterForm(ContactModelFilterForm, NetBoxModelFilterSetForm):
     model = Supplier
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag')),
-        ('Contacts', ('contact', 'contact_role', 'contact_group')),
+        FieldSet('q', 'filter_id', 'tag'),
+        FieldSet('contact', 'contact_role', 'contact_group', name='Contacts'),
     )
 
     tag = TagFilterField(model)
 
 
 class PurchaseFilterForm(NetBoxModelFilterSetForm):
     model = Purchase
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag')),
-        ('Purchase', ('supplier_id', 'status', 'date_after', 'date_before')),
+        FieldSet('q', 'filter_id', 'tag'),
+        FieldSet('supplier_id', 'status', 'date_after', 'date_before', name='Purchase'),
     )
 
     supplier_id = DynamicModelMultipleChoiceField(
         queryset=Supplier.objects.all(),
         required=False,
         label='Supplier',
     )
@@ -279,22 +283,22 @@
     )
     tag = TagFilterField(model)
 
 
 class DeliveryFilterForm(NetBoxModelFilterSetForm):
     model = Delivery
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag')),
-        ('Delivery', (
+        FieldSet('q', 'filter_id', 'tag'),
+        FieldSet(
             'purchase_id',
             'supplier_id',
             'receiving_contact_id',
             'date_after',
-            'date_before'
-        )),
+            'date_before',
+            name='Delivery'),
     )
 
     purchase_id = DynamicModelMultipleChoiceField(
         queryset=Purchase.objects.all(),
         required=False,
         label='Purchase',
     )
@@ -320,16 +324,16 @@
     )
     tag = TagFilterField(model)
 
 
 class InventoryItemTypeFilterForm(NetBoxModelFilterSetForm):
     model = InventoryItemType
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag')),
-        ('Inventory Item Type', ('manufacturer_id', 'inventoryitem_group_id')),
+        FieldSet('q', 'filter_id', 'tag'),
+        FieldSet('manufacturer_id', 'inventoryitem_group_id', name='Inventory Item Type'),
     )
     manufacturer_id = DynamicModelMultipleChoiceField(
         queryset=Manufacturer.objects.all(),
         required=False,
         label='Manufacturer',
     )
     inventoryitem_group_id = DynamicModelMultipleChoiceField(
@@ -339,15 +343,15 @@
     )
     tag = TagFilterField(model)
 
 
 class InventoryItemGroupFilterForm(NetBoxModelFilterSetForm):
     model = InventoryItemGroup
     fieldsets = (
-        (None, ('q', 'filter_id', 'tag', 'parent_id')),
+        FieldSet('q', 'filter_id', 'tag', 'parent_id'),
     )
     parent_id = DynamicModelMultipleChoiceField(
         queryset=InventoryItemGroup.objects.all(),
         required=False,
         label='Parent group'
     )
     tag = TagFilterField(model)
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/forms/models.py` & `netbox_inventory-2.0.0/netbox_inventory/forms/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dcim.models import DeviceType, Manufacturer, ModuleType, Location, Site
 from netbox.forms import NetBoxModelForm
 from netbox_inventory.choices import HardwareKindChoices
 from utilities.forms.fields import CommentField, DynamicModelChoiceField, SlugField
+from utilities.forms.rendering import FieldSet
 from utilities.forms.widgets import DatePicker
 from tenancy.models import Contact, Tenant
 from ..models import Asset, Delivery, InventoryItemType, InventoryItemGroup, Purchase, Supplier
 from ..utils import get_tags_and_edit_protected_asset_fields
 
 __all__ = (
     'AssetForm',
@@ -90,49 +91,19 @@
         query_params={
             'site_id': '$storage_site',
         },
     )
     comments = CommentField()
 
     fieldsets = (
-        ('General', ('name', 'asset_tag', 'tags', 'status')),
-        (
-            'Hardware',
-            (
-                'serial',
-                'manufacturer',
-                'device_type',
-                'module_type',
-                'inventoryitem_type',
-            ),
-        ),
-        (
-            'Purchase',
-            (
-                'owner',
-                'purchase',
-                'delivery',
-                'warranty_start',
-                'warranty_end',
-            ),
-        ),
-        (
-            'Assigned to',
-            (
-                'tenant',
-                'contact',
-            ),
-        ),
-        (
-            'Location',
-            (
-                'storage_site',
-                'storage_location',
-            ),
-        ),
+        FieldSet('name', 'asset_tag', 'tags', 'status', name='General'),
+        FieldSet('serial', 'manufacturer', 'device_type', 'module_type', 'inventoryitem_type', name='Hardware'),
+        FieldSet('owner', 'purchase', 'delivery', 'warranty_start', 'warranty_end', name='Purchase'),
+        FieldSet('tenant', 'contact', name='Assigned to'),
+        FieldSet('storage_site', 'storage_location', name='Location'),
     )
 
     class Meta:
         model = Asset
         fields = (
             'name',
             'asset_tag',
@@ -209,15 +180,17 @@
             self.cleaned_data['purchase'] = delivery.purchase
 
 
 class SupplierForm(NetBoxModelForm):
     slug = SlugField(slug_source='name')
     comments = CommentField()
 
-    fieldsets = (('Supplier', ('name', 'slug', 'description', 'tags')),)
+    fieldsets = (
+        FieldSet('name', 'slug', 'description', 'tags', name='Supplier'),
+    )
 
     class Meta:
         model = Supplier
         fields = (
             'name',
             'slug',
             'description',
@@ -225,15 +198,17 @@
             'tags',
         )
 
 
 class PurchaseForm(NetBoxModelForm):
     comments = CommentField()
 
-    fieldsets = (('Purchase', ('supplier', 'name', 'status', 'date', 'description', 'tags')),)
+    fieldsets = (
+        FieldSet('supplier', 'name', 'status', 'date', 'description', 'tags', name='Purchase'),
+    )
 
     class Meta:
         model = Purchase
         fields = (
             'supplier',
             'name',
             'status',
@@ -246,22 +221,17 @@
             'date': DatePicker(),
         }
 
 
 class DeliveryForm(NetBoxModelForm):
     comments = CommentField()
 
-    fieldsets = (('Delivery', (
-        'purchase',
-        'name',
-        'date',
-        'receiving_contact',
-        'description',
-        'tags'
-    )),)
+    fieldsets = (
+        FieldSet('purchase', 'name', 'date', 'receiving_contact', 'description', 'tags', name='Delivery'),
+    )
 
     class Meta:
         model = Delivery
         fields = (
             'purchase',
             'name',
             'date',
@@ -276,18 +246,15 @@
 
 
 class InventoryItemTypeForm(NetBoxModelForm):
     slug = SlugField(slug_source='model')
     comments = CommentField()
 
     fieldsets = (
-        (
-            'Inventory Item Type',
-            ('manufacturer', 'model', 'slug', 'part_number', 'inventoryitem_group', 'tags'),
-        ),
+        FieldSet('manufacturer', 'model', 'slug', 'part_number', 'inventoryitem_group', 'tags', name='Inventory Item Type'),
     )
 
     class Meta:
         model = InventoryItemType
         fields = (
             'manufacturer',
             'model',
@@ -299,18 +266,15 @@
         )
 
 
 class InventoryItemGroupForm(NetBoxModelForm):
     comments = CommentField()
 
     fieldsets = (
-        (
-            'Inventory Item Group',
-            ('name', 'parent', 'tags'),
-        ),
+        FieldSet('name', 'parent', 'tags', name='Inventory Item Group'),
     )
 
     class Meta:
         model = InventoryItemGroup
         fields = (
             'name',
             'parent',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/forms/reassign.py` & `netbox_inventory-2.0.0/netbox_inventory/forms/reassign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/graphql.py` & `netbox_inventory-2.0.0/netbox_inventory/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/management/commands/check_asset_tags.py` & `netbox_inventory-2.0.0/netbox_inventory/management/commands/check_asset_tags.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/migrations/0001_initial_prod.py` & `netbox_inventory-2.0.0/netbox_inventory/migrations/0001_initial_prod.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py` & `netbox_inventory-2.0.0/netbox_inventory/migrations/0003_add_inventoryitemgroup.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py` & `netbox_inventory-2.0.0/netbox_inventory/migrations/0004_inventoryitemgroup_tree.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py` & `netbox_inventory-2.0.0/netbox_inventory/migrations/0005_delivery_asset_delivery.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/models.py` & `netbox_inventory-2.0.0/netbox_inventory/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,19 +372,37 @@
         if self.serial:
             return f'{self.hardware_type} {self.serial}'
         else:
             return f'{self.hardware_type} (id:{self.id})'
 
     class Meta:
         ordering = ('device_type', 'module_type', 'inventoryitem_type', 'serial',)
-        unique_together = (
-            ('device_type', 'serial'),
-            ('module_type', 'serial'),
-            ('inventoryitem_type', 'serial'),
-            ('owner', 'asset_tag'),
+        constraints = (
+            models.UniqueConstraint(
+                fields=('device_type', 'serial'),
+                name='unique_device_type_serial',
+            ),
+            models.UniqueConstraint(
+                fields=('module_type', 'serial'),
+                name='unique_module_type_serial',
+            ),
+            models.UniqueConstraint(
+                fields=('inventoryitem_type', 'serial'),
+                name='unique_inventoryitem_type_serial',
+            ),
+            models.UniqueConstraint(
+                fields=('owner', 'asset_tag'),
+                name='unique_owner_asset_tag',
+            ),
+            models.UniqueConstraint(
+                'asset_tag',
+                condition=models.Q(owner__isnull=True),
+                name='unique_asset_tag',
+                violation_error_message='Asset with this Asset Tag and no Owner already exists.',
+            ),
         )
 
 
 class Supplier(NetBoxModel, ContactsMixin):
     """
     Supplier is a legal entity that sold some assets that we keep track of.
     This can be the same entity as Manufacturer or a separate one. However
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/search.py` & `netbox_inventory-2.0.0/netbox_inventory/search.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/signals.py` & `netbox_inventory-2.0.0/netbox_inventory/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tables.py` & `netbox_inventory-2.0.0/netbox_inventory/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/template_content.py` & `netbox_inventory-2.0.0/netbox_inventory/template_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from django.template import Template
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins import PluginTemplateExtension
 
 from .models import Asset
 
 
 WARRANTY_PROGRESSBAR = '''
 {% with record.warranty_progress as wp %}
 {% with record.warranty_remaining as wr %}
 {% with settings.PLUGINS_CONFIG.netbox_inventory.asset_warranty_expire_warning_days as wthresh %}
 
 {% if wp is None and wr.days <= 0 %}
-    <div class="progress"><div role="progressbar" class="progress-bar progress-bar-striped bg-danger" style="width:100%;">Expired {{ record.warranty_end|timesince|split:','|first }} ago</div></div>
+  <div class="progress" role="progressbar">
+    <div class="progress-bar progress-bar-striped text-bg-danger" style="width:100%;">
+      Expired {{ record.warranty_end|timesince|split:','|first }} ago
+    </div>
+  </div>
 {% elif wp is None and wr.days > 0 %}
-    <div class="progress"><div role="progressbar" class="progress-bar progress-bar-striped {% if wthresh and wr.days < wthresh %}bg-warning{% else %}bg-success{% endif %}" style="width:100%;">{{ record.warranty_end|timeuntil|split:','|first }}</div></div>
+  <div class="progress" role="progressbar">
+    <div class="progress-bar progress-bar-striped text-bg-{% if wthresh and wr.days < wthresh %}warning{% else %}success{% endif %}" style="width:100%;">
+      {{ record.warranty_end|timeuntil|split:','|first }}
+    </div>
+  </div>
 {% elif wp is None %}
-    <span class="text-muted">No data</span>
+    {{ ""|placeholder }}
 {% else %}
 
-<div class="progress">
+<div
+  class="progress"
+  role="progressbar"
+  aria-valuemin="0"
+  aria-valuemax="100"
+  aria-valuenow="{% if wp < 0 %}0{% else %}{{ wp }}{% endif %}"
+>
   <div
-    role="progressbar"
-    aria-valuemin="0"
-    aria-valuemax="100"
-    aria-valuenow="{% if wp < 0 %}0{% else %}{{ wp }}{% endif %}"
-    class="progress-bar {% if wp >= 100 %}bg-danger{% elif wthresh and wr.days < wthresh %}bg-warning{% else %}bg-success{% endif %}"
+    class="progress-bar text-bg-{% if wp >= 100 %}danger{% elif wthresh and wr.days < wthresh %}warning{% else %}success{% endif %}"
     style="width: {% if wp < 0 %}0%{% else %}{{ wp }}%{% endif %};"
-  >
+  ></div>
   {% if record.warranty_progress >= 100 %}
-    Expired {{ record.warranty_end|timesince|split:','|first }} ago
-  </div>
+    <span class="justify-content-center d-flex align-items-center position-absolute text-light w-100 h-100">Expired {{ record.warranty_end|timesince|split:','|first }} ago</span>
   {% elif record.warranty_progress >= 35 %}
-    {{ record.warranty_end|timeuntil|split:','|first }}
-  </div>
+    <span class="justify-content-center d-flex align-items-center position-absolute text-body-emphasis w-100 h-100">{{ record.warranty_end|timeuntil|split:','|first }}</span>
   {% elif record.warranty_progress >= 0 %}
-  </div>
-    <span class="ps-1">{{ record.warranty_end|timeuntil|split:','|first }}</span>
+    <span class="justify-content-center d-flex align-items-center position-absolute text-body-emphasis w-100 h-100">{{ record.warranty_end|timeuntil|split:','|first }}</span>
   {% else %}
-  </div>
-    <span class="text-center" style="width: 100%">Starts in {{ record.warranty_start|timeuntil|split:','|first }}</span>
+    <span class="justify-content-center d-flex align-items-center position-absolute text-body-emphasis w-100 h-100">Starts in {{ record.warranty_start|timeuntil|split:','|first }}</span>
   {% endif %}
 </div>
 
 {% endif %}
 {% endwith wthresh %}
 {% endwith wr %}
 {% endwith wp %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset.html`

 * *Files 6% similar despite different names*

```diff
@@ -13,174 +13,168 @@
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Asset</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Asset Tag</th>
-              <td class="font-monospace">{{ object.asset_tag|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Serial Number</th>
-              <td class="font-monospace">{{ object.serial|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Status</th>
-              <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
-            </tr>
-            <tr>
-              <th scope="row">{{ object.get_kind_display }} Type</th>
-              <td><a href="{{object.hardware_type.get_absolute_url}}">{{ object.hardware_type.manufacturer }} {{ object.hardware_type }}</a></td>
-            </tr>
-            {% if object.kind == 'inventoryitem' %}
-            <tr>
-              <th scope="row">Inventory Item Group</th>
-              <td>
-                {% if object.inventoryitem_type.inventoryitem_group %}
-                  {% for group in object.inventoryitem_type.inventoryitem_group.get_ancestors %}
-                    {{ group|linkify }} /
-                  {% endfor %}
-                  {{ object.inventoryitem_type.inventoryitem_group|linkify }}
-                {% else %}
-                  {{ ''|placeholder }}
-                {% endif %}
-              </td>
-            </tr>
-            {% endif %}
-            <tr>
-              <th scope="row" title="Where is this asset stored when not in use">Storage Location</th>
-              <td>
-                {% if object.storage_location %}
-                  {{ object.storage_location.site }} /
-                {% endif %}
-                {{ object.storage_location|linkify|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Asset Tag</th>
+            <td class="font-monospace">{{ object.asset_tag|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Serial Number</th>
+            <td class="font-monospace">{{ object.serial|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Status</th>
+            <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
+          </tr>
+          <tr>
+            <th scope="row">{{ object.get_kind_display }} Type</th>
+            <td><a href="{{object.hardware_type.get_absolute_url}}">{{ object.hardware_type.manufacturer }} {{ object.hardware_type }}</a></td>
+          </tr>
+          {% if object.kind == 'inventoryitem' %}
+          <tr>
+            <th scope="row">Inventory Item Group</th>
+            <td>
+              {% if object.inventoryitem_type.inventoryitem_group %}
+                {% for group in object.inventoryitem_type.inventoryitem_group.get_ancestors %}
+                  {{ group|linkify }} /
+                {% endfor %}
+                {{ object.inventoryitem_type.inventoryitem_group|linkify }}
+              {% else %}
+                {{ ''|placeholder }}
+              {% endif %}
+            </td>
+          </tr>
+          {% endif %}
+          <tr>
+            <th scope="row" title="Where is this asset stored when not in use">Storage Location</th>
+            <td>
+              {% if object.storage_location %}
+                {{ object.storage_location.site }} /
+              {% endif %}
+              {{ object.storage_location|linkify|placeholder }}</td>
+          </tr>
+        </table>
       </div>
       <div class="card">
-        <h5 class="card-header">Assigned To</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Tenant</th>
-              <td>
-                {% if object.tenant.group %}
-                  {{ object.tenant.group|linkify }} /
-                {% endif %}
-                {{ object.tenant|linkify|placeholder }}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Contact</th>
-              <td>{{ object.contact|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">{{ object.get_kind_display }}</th>
-              <td>{{ object.hardware|linkify|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
-        <div class="card-footer text-end noprint">
-          {# only show create button if use has add permissions for the kind of hardware being created #}
-          {% if object.kind == 'device' and perms.dcim.add_device or object.kind == 'module' and perms.dcim.add_module or object.kind == 'inventoryitem' and perms.dcim.add_inventoryitem %}
-            {% if object.hardware %}
-            <a href="#" class="btn btn-sm btn-outline-dark disabled">
-              <span class="mdi mdi-vector-difference-ba" aria-hidden="true"></span> Create {{ object.get_kind_display }}
-            </a>
-            {% else %}
-            <a href="{% url 'plugins:netbox_inventory:asset_'|add:object.kind|add:'_create' %}?asset_id={{ object.pk }}" class="btn btn-sm btn-green" title="Create a new {{ object.get_kind_display }} from this asset">
-              <span class="mdi mdi-vector-difference-ba" aria-hidden="true"></span> Create {{ object.get_kind_display }}
-            </a>
+        <h5 class="card-header">
+          Assigned To
+          <div class="card-actions">
+            {# only show create button if use has add permissions for the kind of hardware being created #}
+            {% if object.kind == 'device' and perms.dcim.add_device or object.kind == 'module' and perms.dcim.add_module or object.kind == 'inventoryitem' and perms.dcim.add_inventoryitem %}
+              {% if object.hardware %}
+                <a href="#" class="btn btn-sm btn-ghost-dark disabled">
+                  <i class="mdi mdi-vector-difference-ba" aria-hidden="true"></i> Create {{ object.get_kind_display }}
+                </a>
+              {% else %}
+                <a href="{% url 'plugins:netbox_inventory:asset_'|add:object.kind|add:'_create' %}?asset_id={{ object.pk }}" class="btn btn-sm btn-ghost-green" title="Create a new {{ object.get_kind_display }} from this asset">
+                  <i class="mdi mdi-vector-difference-ba" aria-hidden="true"></i> Create {{ object.get_kind_display }}
+                </a>
+              {% endif %}
             {% endif %}
-          {% endif %}
-          {# only show edit button if user has change permission on asset #}
-          {% if perms.netbox_inventory.change_asset %}
-            <a href="{% url 'plugins:netbox_inventory:asset_assign' object.pk %}?return_url={{ object.get_absolute_url }}" class="btn btn-sm btn-orange">
-              <span class="mdi mdi-vector-link" aria-hidden="true"></span> Edit Assignment
-            </a>
-          {% endif %}
-        </div>
+            {# only show edit button if user has change permission on asset #}
+            {% if perms.netbox_inventory.change_asset %}
+              <a href="{% url 'plugins:netbox_inventory:asset_assign' object.pk %}?return_url={{ object.get_absolute_url }}" class="btn btn-sm btn-ghost-orange">
+                <i class="mdi mdi-vector-link" aria-hidden="true"></i> Edit Assignment
+              </a>
+            {% endif %}
+          </div>
+        </h5>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Tenant</th>
+            <td>
+              {% if object.tenant.group %}
+                {{ object.tenant.group|linkify }} /
+              {% endif %}
+              {{ object.tenant|linkify|placeholder }}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Contact</th>
+            <td>{{ object.contact|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">{{ object.get_kind_display }}</th>
+            <td>{{ object.hardware|linkify|placeholder }}</td>
+          </tr>
+        </table>
       </div>
       <div class="card">
         <h5 class="card-header">Installed Location</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Site</th>
-              <td>{{ object.installed_site|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Location</th>
-              <td>
-                {% if object.installed_location %}
-                  {% for location in object.installed_location.get_ancestors %}
-                    {{ location|linkify }} /
-                  {% endfor %}
-                  {{ object.installed_location|linkify }}
-                {% else %}
-                  {{ ''|placeholder }}
-                {% endif %}
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Rack</th>
-              <td>{{ object.installed_rack|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Device</th>
-              <td>{{ object.installed_device|linkify|placeholder }}</td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Site</th>
+            <td>{{ object.installed_site|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Location</th>
+            <td>
+              {% if object.installed_location %}
+                {% for location in object.installed_location.get_ancestors %}
+                  {{ location|linkify }} /
+                {% endfor %}
+                {{ object.installed_location|linkify }}
+              {% else %}
+                {{ ''|placeholder }}
+              {% endif %}
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Rack</th>
+            <td>{{ object.installed_rack|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Device</th>
+            <td>{{ object.installed_device|linkify|placeholder }}</td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Purchase</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Owner</th>
-              <td>{{ object.owner|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Purchase</th>
-              <td>{{ object.purchase|linkify|placeholder }}{% if object.purchase.date %} on {{ object.purchase.date|annotated_date }}{% endif %}</td>
-            </tr>
-            <tr>
-              <th scope="row">Delivery</th>
-              <td>{{ object.delivery|linkify:'name'|placeholder }}{% if object.delivery.date %} on {{ object.delivery.date|annotated_date }}{% endif %}</td>
-            </tr>
-            <tr>
-              <th scope="row">Warranty start</th>
-              <td>{{ object.warranty_start|annotated_date|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Warranty end</th>
-              <td>{{ object.warranty_end|annotated_date|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Warranty remaining</th>
-              <td>
-                {% include warranty_progressbar with record=object %}
-              </td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Owner</th>
+            <td>{{ object.owner|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Purchase</th>
+            <td>{{ object.purchase|linkify|placeholder }}{% if object.purchase.date %} on {{ object.purchase.date|isodate }}{% endif %}</td>
+          </tr>
+          <tr>
+            <th scope="row">Delivery</th>
+            <td>{{ object.delivery|linkify:'name'|placeholder }}{% if object.delivery.date %} on {{ object.delivery.date|isodate }}{% endif %}</td>
+          </tr>
+          <tr>
+            <th scope="row">Warranty start</th>
+            <td>{{ object.warranty_start|isodate|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Warranty end</th>
+            <td>{{ object.warranty_end|isodate|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Warranty remaining</th>
+            <td>
+              {% include warranty_progressbar with record=object %}
+            </td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/image_attachments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
```

#### html2text {}

```diff
@@ -18,46 +18,49 @@
 IInnvveennttoorryy IItteemm GGrroouupp    object.inventoryitem_type.inventoryitem_group.get_ancestors
                         %} {{ group|linkify }} / {% endfor %} {
                         { object.inventoryitem_type.inventoryitem_group|linkify }}
                         {% else %} {{ ''|placeholder }} {% endif %}
                         {% if object.storage_location %} {
 SSttoorraaggee LLooccaattiioonn        { object.storage_location.site }} / {% endif %} {
                         { object.storage_location|linkify|placeholder }}
-**** AAssssiiggnneedd TToo ****
+AAssssiiggnneedd TToo
+{{## oonnllyy sshhooww ccrreeaattee bbuuttttoonn iiff uussee hhaass aadddd ppeerrmmiissssiioonnss ffoorr tthhee kkiinndd ooff hhaarrddwwaarree
+bbeeiinngg ccrreeaatteedd ##}} {{%% iiff oobbjjeecctt..kkiinndd ==== ''ddeevviiccee'' aanndd ppeerrmmss..ddcciimm..aadddd__ddeevviiccee oorr
+oobbjjeecctt..kkiinndd ==== ''mmoodduullee'' aanndd ppeerrmmss..ddcciimm..aadddd__mmoodduullee oorr oobbjjeecctt..kkiinndd ====
+''iinnvveennttoorryyiitteemm'' aanndd ppeerrmmss..ddcciimm..aadddd__iinnvveennttoorryyiitteemm %%}} {{%% iiff oobbjjeecctt..hhaarrddwwaarree %%}}
+_CC_rr_ee_aa_tt_ee_ _{{_{{_ _oo_bb_jj_ee_cc_tt_.._gg_ee_tt____kk_ii_nn_dd____dd_ii_ss_pp_ll_aa_yy_ _}}_}}
+{{%% eellssee %%}}
+_CC_rr_ee_aa_tt_ee_ _{{_{{_ _oo_bb_jj_ee_cc_tt_.._gg_ee_tt____kk_ii_nn_dd____dd_ii_ss_pp_ll_aa_yy_ _}}_}}
+{{%% eennddiiff %%}} {{%% eennddiiff %%}} {{## oonnllyy sshhooww eeddiitt bbuuttttoonn iiff uusseerr hhaass cchhaannggee ppeerrmmiissssiioonn
+oonn aasssseett ##}} {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..cchhaannggee__aasssseett %%}}
+_EE_dd_ii_tt_ _AA_ss_ss_ii_gg_nn_mm_ee_nn_tt
+{{%% eennddiiff %%}}
                               {% if object.tenant.group %} {
 TTeennaanntt                        { object.tenant.group|linkify }} / {% endif %} {
                               { object.tenant|linkify|placeholder }}
 CCoonnttaacctt                       {{ object.contact|linkify|placeholder }}
 {{{{ oobbjjeecctt..ggeett__kkiinndd__ddiissppllaayy }}}} {{ object.hardware|linkify|placeholder }}
-{# only show create button if use has add permissions for the kind of hardware
-being created #} {% if object.kind == 'device' and perms.dcim.add_device or
-object.kind == 'module' and perms.dcim.add_module or object.kind ==
-'inventoryitem' and perms.dcim.add_inventoryitem %} {% if object.hardware %}
-_C_r_e_a_t_e_ _{_{_ _o_b_j_e_c_t_._g_e_t___k_i_n_d___d_i_s_p_l_a_y_ _}_}_ {% else %} _C_r_e_a_t_e_ _{
-_{_ _o_b_j_e_c_t_._g_e_t___k_i_n_d___d_i_s_p_l_a_y_ _}_}_ {% endif %} {% endif %} {# only show edit button
-if user has change permission on asset #} {% if
-perms.netbox_inventory.change_asset %} _E_d_i_t_ _A_s_s_i_g_n_m_e_n_t_ {% endif %}
 **** IInnssttaalllleedd LLooccaattiioonn ****
 SSiittee     {{ object.installed_site|linkify|placeholder }}
          {% if object.installed_location %} {% for location in
 LLooccaattiioonn object.installed_location.get_ancestors %} {{ location|linkify }} / {%
          endfor %} {{ object.installed_location|linkify }} {% else %} {
          { ''|placeholder }} {% endif %}
 RRaacckk     {{ object.installed_rack|linkify|placeholder }}
 DDeevviiccee   {{ object.installed_device|linkify|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 **** PPuurrcchhaassee ****
 OOwwnneerr              {{ object.owner|linkify|placeholder }}
                    {{ object.purchase|linkify|placeholder }}{% if
-PPuurrcchhaassee           object.purchase.date %} on {
-                   { object.purchase.date|annotated_date }}{% endif %}
+PPuurrcchhaassee           object.purchase.date %} on {{ object.purchase.date|isodate
+                   }}{% endif %}
                    {{ object.delivery|linkify:'name'|placeholder }}{% if
-DDeelliivveerryy           object.delivery.date %} on {
-                   { object.delivery.date|annotated_date }}{% endif %}
-WWaarrrraannttyy ssttaarrtt     {{ object.warranty_start|annotated_date|placeholder }}
-WWaarrrraannttyy eenndd       {{ object.warranty_end|annotated_date|placeholder }}
+DDeelliivveerryy           object.delivery.date %} on {{ object.delivery.date|isodate
+                   }}{% endif %}
+WWaarrrraannttyy ssttaarrtt     {{ object.warranty_start|isodate|placeholder }}
+WWaarrrraannttyy eenndd       {{ object.warranty_end|isodate|placeholder }}
 WWaarrrraannttyy rreemmaaiinniinngg {% include warranty_progressbar with record=object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/image_attachments.html' %} {% plugin_right_page object
 %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_bulk_import.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends "generic/bulk_import.html" %}
 
 {% load helpers %}
 {% load form_helpers %}
 
-{% block content-wrapper %}
+{% block content %}
 {{ block.super }}
 
     <div class="tab-content">
         <div class="row my-3">
             <div class="col col-md-12">
                 <div class="card">
                     <h5 class="card-header">
@@ -18,45 +18,49 @@
                         CSV import can automatically create objects related to each Asset being imported.
                         This is controlled via plugin's <a href="https://github.com/ArnesSI/netbox-inventory#settings" target="_blank">settings</a>.
                         If a related object is missing and is not allowed to be created autmatically, import will fail.
                         </p>
                         <p>
                         Values bellow show your current config values.
                         </p>
+                    </div>
                         <table class="table">
-                            <tr>
-                                <th>Object name</th>
-                                <th>Created if missing?</th>
-                                <th>Plugin setting name</th>
-                            </tr>
-                            <tr>
-                                <td>Manufacturer & Device Type</td>
-                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_device_type %}</td>
-                                <td><code>asset_import_create_device_type</code></td>
-                            </tr>
-                            <tr>
-                                <td>Manufacturer & Module Type</td>
-                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_module_type %}</td>
-                                <td><code>asset_import_create_module_type</code></td>
-                            </tr>
-                            <tr>
-                                <td>Manufacturer & InventoryItem Type</td>
-                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type %}</td>
-                                <td><code>asset_import_create_inventoryitem_type</code></td>
-                            </tr>
-                            <tr>
-                                <td>Supplier & Purchase</td>
-                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}</td>
-                                <td><code>asset_import_create_purchase</code></td>
-                            </tr>
-                            <tr>
-                                <td>Owner & Tenant</td>
-                                <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}</td>
-                                <td><code>asset_import_create_tenant</code></td>
-                            </tr>
+                            <thead>
+                                <tr>
+                                    <th>Object name</th>
+                                    <th>Created if missing?</th>
+                                    <th>Plugin setting name</th>
+                                </tr>
+                            </thead>
+                            <tbody>
+                                <tr>
+                                    <td>Manufacturer & Device Type</td>
+                                    <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_device_type %}</td>
+                                    <td class="font-monospace">asset_import_create_device_type</td>
+                                </tr>
+                                <tr>
+                                    <td>Manufacturer & Module Type</td>
+                                    <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_module_type %}</td>
+                                    <td class="font-monospace">asset_import_create_module_type</td>
+                                </tr>
+                                <tr>
+                                    <td>Manufacturer & InventoryItem Type</td>
+                                    <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type %}</td>
+                                    <td class="font-monospace">asset_import_create_inventoryitem_type</td>
+                                </tr>
+                                <tr>
+                                    <td>Supplier & Purchase</td>
+                                    <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}</td>
+                                    <td class="font-monospace">asset_import_create_purchase</td>
+                                </tr>
+                                <tr>
+                                    <td>Owner & Tenant</td>
+                                    <td>{% checkmark settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}</td>
+                                    <td class="font-monospace">asset_import_create_tenant</td>
+                                </tr>
+                            </tbody>
                         </table>
-                    </div>
                 </div>
             </div>
         </div>
     </div>
-{% endblock content-wrapper %}
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "generic/bulk_import.html" %} {% load helpers %} {% load
-form_helpers %} {% block content-wrapper %} {{ block.super }}
+form_helpers %} {% block content %} {{ block.super }}
 **** IImmppoorrtt sseettttiinnggss ****
 CSV import can automatically create objects related to each Asset being
 imported. This is controlled via plugin's _s_e_t_t_i_n_g_s. If a related object is
 missing and is not allowed to be created autmatically, import will fail.
 Values bellow show your current config values.
 OObbjjeecctt nnaammee   CCrreeaatteedd iiff mmiissssiinngg??                                                             PPlluuggiinn sseettttiinngg nnaammee
 Manufacturer  {% checkmark                                                                    asset_import_create_device_type
@@ -14,8 +14,8 @@
 &             settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_inventoryitem_type asset_import_create_inventoryitem_type
 InventoryItem %}
 Type
 Supplier &    {% checkmark                                                                    asset_import_create_purchase
 Purchase      settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_purchase %}
 Owner &       {% checkmark                                                                    asset_import_create_tenant
 Tenant        settings.PLUGINS_CONFIG.netbox_inventory.asset_import_create_tenant %}
-{% endblock content-wrapper %}
+{% endblock content %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_edit.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/asset_reassign.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/delivery.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/purchase.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,79 +2,92 @@
 {% load helpers %}
 {% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item">
-    <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.purchase.supplier.pk }}">{{ object.purchase.supplier }}</a>
-  </li>
-  <li class="breadcrumb-item">
-    <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?purchase_id={{ object.purchase.pk }}">{{ object.purchase }}</a>
+    <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.supplier.pk }}">{{ object.supplier }}</a>
   </li>
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Delivery</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Purchase</th>
-              <td>{{ object.purchase|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Receiving Contact</th>
-              <td>{{ object.receiving_contact|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Date</th>
-              <td>{{ object.date|annotated_date|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Assets</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?delivery_id={{ object.pk }}">{{ asset_count }}</a>
-              </td>
-            </tr>
-          </table>
-        </div>
+        <h5 class="card-header">Purchase</h5>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Supplier</th>
+            <td>{{ object.supplier|linkify }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Status</th>
+            <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
+          </tr>
+          <tr>
+            <th scope="row">Date</th>
+            <td>{{ object.date|isodate|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Deliveries</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?purchase_id={{ object.pk }}">{{ delivery_count }}</a>
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Assets</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:asset_list' %}?purchase_id={{ object.pk }}">{{ asset_count }}</a>
+            </td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Delivered Assets</h5>
-        <div class="card-body htmx-container table-responsive"
-          hx-get="{% url 'plugins:netbox_inventory:asset_list' %}?delivery_id={{ object.pk }}"
-          hx-trigger="load"
-        ></div>
-        {% if perms.netbox_inventory.add_asset %}
-          <div class="card-footer text-end noprint">
-            <a href="{% url 'plugins:netbox_inventory:asset_add' %}?delivery={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
-              <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Asset
-            </a>
-          </div>
-        {% endif %}
+        <h5 class="card-header">
+          Deliveries
+          {% if perms.netbox_inventory.add_delivery %}
+            <div class="card-actions">
+              <a href="{% url 'plugins:netbox_inventory:delivery_add' %}?purchase={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-ghost-primary btn-sm">
+                <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add a Delivery
+              </a>
+            </div>
+          {% endif %}
+        </h5>
+        {% htmx_table 'plugins:netbox_inventory:delivery_list' purchase_id=object.pk %}
+      </div>
+      <div class="card">
+        <h5 class="card-header">
+          Purchased Assets
+          {% if perms.netbox_inventory.add_asset %}
+            <div class="card-actions">
+              <a href="{% url 'plugins:netbox_inventory:asset_add' %}?purchase={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-ghost-primary btn-sm">
+                <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Asset
+              </a>
+            </div>
+          {% endif %}
+        </h5>
+        {% htmx_table 'plugins:netbox_inventory:asset_list' purchase_id=object.pk %}
       </div>
       {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
 load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
 }}
-_{_{_ _o_b_j_e_c_t_._p_u_r_c_h_a_s_e_._s_u_p_p_l_i_e_r_ _}_}
-_{_{_ _o_b_j_e_c_t_._p_u_r_c_h_a_s_e_ _}_}
+_{_{_ _o_b_j_e_c_t_._s_u_p_p_l_i_e_r_ _}_}
 {% endblock %} {% block content %}
-**** DDeelliivveerryy ****
-NNaammee              {{ object.name }}
-PPuurrcchhaassee          {{ object.purchase|linkify }}
-RReecceeiivviinngg CCoonnttaacctt {{ object.receiving_contact|linkify|placeholder }}
-DDaattee              {{ object.date|annotated_date|placeholder }}
-DDeessccrriippttiioonn       {{ object.description|placeholder }}
-AAsssseettss            _{_{_ _a_s_s_e_t___c_o_u_n_t_ _}_}
+**** PPuurrcchhaassee ****
+NNaammee        {{ object.name }}
+SSuupppplliieerr    {{ object.supplier|linkify }}
+SSttaattuuss      {% badge object.get_status_display bg_color=object.get_status_color
+            %}
+DDaattee        {{ object.date|isodate|placeholder }}
+DDeessccrriippttiioonn {{ object.description|placeholder }}
+DDeelliivveerriieess  _{_{_ _d_e_l_i_v_e_r_y___c_o_u_n_t_ _}_}
+AAsssseettss      _{_{_ _a_s_s_e_t___c_o_u_n_t_ _}_}
 {% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
 comments.html' %} {% plugin_right_page object %}
-**** DDeelliivveerreedd AAsssseettss ****
-{% if perms.netbox_inventory.add_asset %}
-_A_d_d_ _a_n_ _A_s_s_e_t
-{% endif %}
+DDeelliivveerriieess {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..aadddd__ddeelliivveerryy %%}}
+_AA_dd_dd_ _aa_ _DD_ee_ll_ii_vv_ee_rr_yy
+{{%% eennddiiff %%}}
+{% htmx_table 'plugins:netbox_inventory:delivery_list' purchase_id=object.pk %}
+PPuurrcchhaasseedd AAsssseettss {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..aadddd__aasssseett %%}}
+_AA_dd_dd_ _aa_nn_ _AA_ss_ss_ee_tt
+{{%% eennddiiff %%}}
+{% htmx_table 'plugins:netbox_inventory:asset_list' purchase_id=object.pk %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_edit_header.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_info.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 {% load helpers %}
 
 <div class="card">
-  <h5 class="card-header">Asset</h5>
-  <div class="card-body">
-  {% if asset %}
-    <table class="table table-hover attr-table">
-      <tr>
-        <th scope="row"><span title="Asset name">Name</span></th>
-        <td><a href="{% url "plugins:netbox_inventory:asset" asset.pk %}">{{ asset.hardware_type.manufacturer }} {{ asset }}{% if asset.name %} ({{ asset.name }}){% endif %}</a></td>
-      </tr>
-      <tr>
-        <th scope="row"><span title="Asset status">Status</span></a></th>
-        <td>{% badge asset.get_status_display bg_color=asset.get_status_color %}</a></td>
-      </tr>
-      <tr>
-        <th scope="row">Owner</th>
-        <td>{{ asset.owner|linkify|placeholder }}</td>
-      </tr>
-      <tr>
-        <th scope="row">Purchase</th>
-        <td>{{ asset.purchase|linkify|placeholder }}</td>
-      </tr>
-      <tr>
-        <th>Warranty remaining</th>
-        <td>
-          {% include warranty_progressbar with record=asset %}
-        </td>
-      </tr>
-    </table>
-  {% else %}
-    <div class="text-muted">None assigned</div>
-  {% endif %}
-  </div>
-  <div class="card-footer text-end noprint">
+  <h5 class="card-header">
+    Asset
     {# only show reassign button if user has change permissions on asset #}
     {% if perms.netbox_inventory.change_asset %}
-      {% with object|meta:"model_name" as object_type %}
-      {% if object_type == "device" %}
-      <a href="{% url 'plugins:netbox_inventory:asset_device_reassign' object.pk %}" class="btn btn-sm btn-orange">
-      {% elif object_type == "module" %}
-      <a href="{% url 'plugins:netbox_inventory:asset_module_reassign' object.pk %}" class="btn btn-sm btn-orange">
-      {% elif object_type == "inventoryitem" %}
-      <a href="{% url 'plugins:netbox_inventory:asset_inventoryitem_reassign' object.pk %}" class="btn btn-sm btn-orange">
-      {% endif %}
-      {% endwith %}
-        <span class="mdi mdi-vector-link" aria-hidden="true"></span> Edit Assignment
-      </a>
+      <div class="card-actions">
+        {% with object|meta:"model_name" as object_type %}
+        {% if object_type == "device" %}
+        <a href="{% url 'plugins:netbox_inventory:asset_device_reassign' object.pk %}" class="btn btn-sm btn-ghost-orange">
+        {% elif object_type == "module" %}
+        <a href="{% url 'plugins:netbox_inventory:asset_module_reassign' object.pk %}" class="btn btn-sm btn-ghost-orange">
+        {% elif object_type == "inventoryitem" %}
+        <a href="{% url 'plugins:netbox_inventory:asset_inventoryitem_reassign' object.pk %}" class="btn btn-sm btn-ghost-orange">
+        {% endif %}
+        {% endwith %}
+          <i class="mdi mdi-vector-link" aria-hidden="true"></i> Edit Assignment
+        </a>
+      </div>
     {% endif %}
-  </div>
+  </h5>
+  {% if asset %}
+  <table class="table table-hover attr-table">
+    <tr>
+      <th scope="row"><span title="Asset name">Name</span></th>
+      <td><a href="{% url "plugins:netbox_inventory:asset" asset.pk %}">{{ asset.hardware_type.manufacturer }} {{ asset }}{% if asset.name %} ({{ asset.name }}){% endif %}</a></td>
+    </tr>
+    <tr>
+      <th scope="row"><span title="Asset status">Status</span></a></th>
+      <td>{% badge asset.get_status_display bg_color=asset.get_status_color %}</a></td>
+    </tr>
+    <tr>
+      <th scope="row">Owner</th>
+      <td>{{ asset.owner|linkify|placeholder }}</td>
+    </tr>
+    <tr>
+      <th scope="row">Purchase</th>
+      <td>{{ asset.purchase|linkify|placeholder }}</td>
+    </tr>
+    <tr>
+      <th>Warranty remaining</th>
+      <td>
+        {% include warranty_progressbar with record=asset %}
+      </td>
+    </tr>
+  </table>
+  {% else %}
+  <div class="text-muted">None assigned</div>
+  {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
 {% load helpers %}
-**** AAsssseett ****
+AAsssseett {{## oonnllyy sshhooww rreeaassssiiggnn bbuuttttoonn iiff uusseerr hhaass cchhaannggee ppeerrmmiissssiioonnss oonn aasssseett ##}}
+{{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..cchhaannggee__aasssseett %%}}
+{{%% wwiitthh oobbjjeecctt||mmeettaa::""mmooddeell__nnaammee"" aass oobbjjeecctt__ttyyppee %%}} {{%% iiff oobbjjeecctt__ttyyppee ====
+""ddeevviiccee"" %%}}
+_{{_%%_ _ee_ll_ii_ff_ _oo_bb_jj_ee_cc_tt____tt_yy_pp_ee_ _==_==_ _""_mm_oo_dd_uu_ll_ee_""_ _%%_}}
+_{{_%%_ _ee_ll_ii_ff_ _oo_bb_jj_ee_cc_tt____tt_yy_pp_ee_ _==_==_ _""_ii_nn_vv_ee_nn_tt_oo_rr_yy_ii_tt_ee_mm_""_ _%%_}}
+_{{_%%_ _ee_nn_dd_ii_ff_ _%%_}}_ _{{_%%_ _ee_nn_dd_ww_ii_tt_hh_ _%%_}}_ _EE_dd_ii_tt_ _AA_ss_ss_ii_gg_nn_mm_ee_nn_tt
+{{%% eennddiiff %%}}
 {% if asset %}
 NNaammee               _{_{_ _a_s_s_e_t_._h_a_r_d_w_a_r_e___t_y_p_e_._m_a_n_u_f_a_c_t_u_r_e_r_ _}_}_ _{_{_ _a_s_s_e_t_ _}_}_{_%_ _i_f
                    _a_s_s_e_t_._n_a_m_e_ _%_}_ _(_{_{_ _a_s_s_e_t_._n_a_m_e_ _}_}_)_{_%_ _e_n_d_i_f_ _%_}
 SSttaattuuss             {% badge asset.get_status_display
                    bg_color=asset.get_status_color %}
 OOwwnneerr              {{ asset.owner|linkify|placeholder }}
 PPuurrcchhaassee           {{ asset.purchase|linkify|placeholder }}
 WWaarrrraannttyy rreemmaaiinniinngg {% include warranty_progressbar with record=asset %}
 {% else %}
 None assigned
 {% endif %}
-{# only show reassign button if user has change permissions on asset #} {% if
-perms.netbox_inventory.change_asset %} {% with object|meta:"model_name" as
-object_type %} {% if object_type == "device" %} _{_%_ _e_l_i_f_ _o_b_j_e_c_t___t_y_p_e_ _=_=_ _"_m_o_d_u_l_e_"
-_%_}_ _{_%_ _e_l_i_f_ _o_b_j_e_c_t___t_y_p_e_ _=_=_ _"_i_n_v_e_n_t_o_r_y_i_t_e_m_"_ _%_}_ _{_%_ _e_n_d_i_f_ _%_}_ _{_%_ _e_n_d_w_i_t_h_ _%_}_ _E_d_i_t
-_A_s_s_i_g_n_m_e_n_t_ _{_%_ _e_n_d_i_f_ _%_}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inc/asset_stats_counts.html`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 <div class="card">
   <h5 class="card-header">Assets</h5>
   <ul class="list-group list-group-flush">
     {% for asset_stat in asset_stats %}
       <a href="{% url 'plugins:netbox_inventory:asset_list' %}?{{ asset_stat.filter_field }}={{ object.pk }}{{ asset_stat.extra_filter }}" class="list-group-item list-group-item-action d-flex justify-content-between">
         {{ asset_stat.label|bettertitle }}
         {% if asset_stat.count %}
-          <span class="badge bg-primary rounded-pill">{{ asset_stat.count }}</span>
+          <span class="badge text-bg-primary rounded-pill">{{ asset_stat.count }}</span>
         {% else %}
-          <span class="badge bg-light rounded-pill">&mdash;</span>
+          <span class="badge text-bg-light rounded-pill">&mdash;</span>
         {% endif %}
       </tr>
       </a>
     {% endfor %}
   </ul>
 </div>
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemgroup.html`

 * *Files 7% similar despite different names*

```diff
@@ -8,139 +8,129 @@
   {% for group in object.get_ancestors %}
     <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:inventoryitemgroup' group.pk %}">{{ group }}</a></li>
   {% endfor %}
 {% endblock %}
 
 {% block extra_controls %}
   {% if perms.netbox_inventory.add_inventoryitemtype %}
-    <a href="{% url 'plugins:netbox_inventory:inventoryitemtype_add' %}?inventoryitem_group={{ object.pk }}" class="btn btn-sm btn-primary">
+    <a href="{% url 'plugins:netbox_inventory:inventoryitemtype_add' %}?inventoryitem_group={{ object.pk }}" class="btn btn-primary">
       <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add inventory item type
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Inventory Item Group</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Parent</th>
-              <td>{{ object.parent|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Assets</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_group_id={{ object.pk }}">{{ asset_table.rows|length }}</a>
-              </td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Parent</th>
+            <td>{{ object.parent|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Assets</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_group_id={{ object.pk }}">{{ asset_table.rows|length }}</a>
+            </td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
 
 
         <div class="card">
         <h5 class="card-header">Asset count by status</h5>
-        <div class="card-body">
-          <table class="table table-hover object-list">
-          <thead>
-            <tr>
-              <th>Status</th>
-              <th>Count</th>
-            </tr>
-          </thead>
-          <tbody>
-            {% for sc in status_counts.values %}
-            <tr>
-              <td>{% badge value=sc.label bg_color=sc.color %}</td>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_group_id={{ object.pk }}&status={{ sc.value }}">
-                  {{ sc.count }}
-                </a>
-              </td>
-            </tr>
-            {% empty %}
-            <tr><td class="text-center text-muted" colspan="2">— No assets found —</td></tr>
-            {% endfor %}
-          </tbody>
-          </table>
-        </div>
+        <table class="table table-hover object-list">
+        <thead>
+          <tr>
+            <th>Status</th>
+            <th>Count</th>
+          </tr>
+        </thead>
+        <tbody>
+          {% for sc in status_counts.values %}
+          <tr>
+            <td>{% badge value=sc.label bg_color=sc.color %}</td>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_group_id={{ object.pk }}&status={{ sc.value }}">
+                {{ sc.count }}
+              </a>
+            </td>
+          </tr>
+          {% empty %}
+          <tr><td class="text-center text-muted" colspan="2">— No assets found —</td></tr>
+          {% endfor %}
+        </tbody>
+        </table>
       </div>
 
       <div class="card">
         <h5 class="card-header">Asset count by type & status</h5>
-        <div class="card-body">
-          <table class="table table-hover object-list table-striped">
-          <thead>
-            <tr>
-              <th>Inventory Item Type</th>
-              <th>Status - Count</th>
-            </tr>
-          </thead>
-          <tbody>
-            {% for tsc in type_status_objects %}
-            <tr>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:inventoryitemtype' tsc.inventoryitem_type %}">
-                  {{ tsc.inventoryitem_type__manufacturer__name }} {{ tsc.inventoryitem_type__model }}
-                </a>
-              </td>
-              <td style="max-width:400px;">
-                <div class="d-flex" style="overflow:auto;">
-                  {% for status in tsc.status_list %}
-                    <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ tsc.inventoryitem_type }}&status={{ status.status }}" class="w-100 me-2">
-                      {% badge value=status.label|add:' - '|add:status.count bg_color=status.color|add:' w-100' %}
-                    </a>
-                  {% endfor %}
-                </div>
-              </td>
-            </tr>
-            {% empty %}
-            <tr><td class="text-center text-muted" colspan="2">— No assets found —</td></tr>
-            {% endfor %}
-          </tbody>
-          </table>
-        </div>
+        <table class="table table-hover object-list table-striped">
+        <thead>
+          <tr>
+            <th>Inventory Item Type</th>
+            <th>Status - Count</th>
+          </tr>
+        </thead>
+        <tbody>
+          {% for tsc in type_status_objects %}
+          <tr>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:inventoryitemtype' tsc.inventoryitem_type %}">
+                {{ tsc.inventoryitem_type__manufacturer__name }} {{ tsc.inventoryitem_type__model }}
+              </a>
+            </td>
+            <td style="max-width:400px;">
+              <div class="d-flex" style="overflow:auto;">
+                {% for status in tsc.status_list %}
+                  <a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ tsc.inventoryitem_type }}&status={{ status.status }}" class="w-100 me-2">
+                    {% badge value=status.label|add:' - '|add:status.count bg_color=status.color|add:' w-100' %}
+                  </a>
+                {% endfor %}
+              </div>
+            </td>
+          </tr>
+          {% empty %}
+          <tr><td class="text-center text-muted" colspan="2">— No assets found —</td></tr>
+          {% endfor %}
+        </tbody>
+        </table>
       </div>
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">
           Child Groups
+          {% if perms.netbox_inventory.add_inventoryitemgroup %}
+            <div class="card-actions">
+              <a href="{% url 'plugins:netbox_inventory:inventoryitemgroup_add' %}?parent={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-ghost-primary btn-sm">
+                <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add Group
+              </a>
+            </div>
+          {% endif %}
         </h5>
-        <div class="card-body table-responsive">
-          {% render_table child_groups_table 'inc/table.html' %}
-        </div>
-        {% if perms.netbox_inventory.add_inventoryitemgroup %}
-          <div class="card-footer text-end noprint">
-            <a href="{% url 'plugins:netbox_inventory:inventoryitemgroup_add' %}?parent={{ object.pk }}" class="btn btn-sm btn-primary">
-              <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Add Group
-            </a>
-          </div>
-        {% endif %}
+        {% render_table child_groups_table 'inc/table.html' %}
       </div>
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Assets</h5>
-        <div class="card-body table-responsive">
-          {% render_table asset_table 'inc/table.html' %}
-          {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
-        </div>
+        {% render_table asset_table 'inc/table.html' %}
+        {% include 'inc/paginator.html' with paginator=asset_table.paginator page=asset_table.page %}
       </div>
       {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -20,19 +20,18 @@
 _{                                          {% for status in tsc.status_list %}
 _{                                          _{_%_ _b_a_d_g_e_ _v_a_l_u_e_=_s_t_a_t_u_s_._l_a_b_e_l_|_a_d_d_:_'_ _-
 _t_s_c_._i_n_v_e_n_t_o_r_y_i_t_e_m___t_y_p_e_____m_a_n_u_f_a_c_t_u_r_e_r_____n_a_m_e _'_|_a_d_d_:_s_t_a_t_u_s_._c_o_u_n_t
 _}_}_ _{_{_ _t_s_c_._i_n_v_e_n_t_o_r_y_i_t_e_m___t_y_p_e_____m_o_d_e_l_ _}_}     _b_g___c_o_l_o_r_=_s_t_a_t_u_s_._c_o_l_o_r_|_a_d_d_:_'_ _w_-_1_0_0_'
                                            _%_}_ {% endfor %}
 â No assets found â
 {% plugin_left_page object %}
-**** CChhiilldd GGrroouuppss ****
+CChhiilldd GGrroouuppss {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..aadddd__iinnvveennttoorryyiitteemmggrroouupp %%}}
+_AA_dd_dd_ _GG_rr_oo_uu_pp
+{{%% eennddiiff %%}}
 {% render_table child_groups_table 'inc/table.html' %}
-{% if perms.netbox_inventory.add_inventoryitemgroup %}
-_A_d_d_ _G_r_o_u_p
-{% endif %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% plugin_right_page object %}
 **** AAsssseettss ****
 {% render_table asset_table 'inc/table.html' %} {% include 'inc/paginator.html'
 with paginator=asset_table.paginator page=asset_table.page %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/inventoryitemtype.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,49 +6,47 @@
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:inventoryitemtype_list' %}?manufacturer_id={{ object.manufacturer.pk }}">{{ object.manufacturer }}</a></li>
 {% endblock %}
 
 {% block extra_controls %}
   {% if perms.netbox_inventory.add_asset %}
-    <a href="{% url 'plugins:netbox_inventory:asset_add' %}?inventoryitem_type={{ object.pk }}&manufacturer={{ object.manufacturer.pk }}" class="btn btn-sm btn-primary">
+    <a href="{% url 'plugins:netbox_inventory:asset_add' %}?inventoryitem_type={{ object.pk }}&manufacturer={{ object.manufacturer.pk }}" class="btn btn-primary">
       <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add asset
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Inventory Item Type</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Manufacturer</th>
-              <td>{{ object.manufacturer|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Model</th>
-              <td>{{ object.model }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Part number</th>
-              <td>{{ object.part_number }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Group</th>
-              <td>{{ object.inventoryitem_group|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Assets</th>
-              <td><a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ object.pk }}">{{ asset_count }}</a></td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Manufacturer</th>
+            <td>{{ object.manufacturer|linkify }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Model</th>
+            <td>{{ object.model }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Part number</th>
+            <td>{{ object.part_number }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Group</th>
+            <td>{{ object.inventoryitem_group|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Assets</th>
+            <td><a href="{% url 'plugins:netbox_inventory:asset_list' %}?inventoryitem_type_id={{ object.pk }}">{{ asset_count }}</a></td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/purchase.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/delivery.html`

 * *Files 24% similar despite different names*

```diff
@@ -2,96 +2,76 @@
 {% load helpers %}
 {% load plugins %}
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
   {{ block.super }}
   <li class="breadcrumb-item">
-    <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.supplier.pk }}">{{ object.supplier }}</a>
+    <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.purchase.supplier.pk }}">{{ object.purchase.supplier }}</a>
+  </li>
+  <li class="breadcrumb-item">
+    <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?purchase_id={{ object.purchase.pk }}">{{ object.purchase }}</a>
   </li>
 {% endblock %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
-        <h5 class="card-header">Purchase</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Supplier</th>
-              <td>{{ object.supplier|linkify }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Status</th>
-              <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
-            </tr>
-            <tr>
-              <th scope="row">Date</th>
-              <td>{{ object.date|annotated_date|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description|placeholder }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Deliveries</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?purchase_id={{ object.pk }}">{{ delivery_count }}</a>
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Assets</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?purchase_id={{ object.pk }}">{{ asset_count }}</a>
-              </td>
-            </tr>
-          </table>
-        </div>
+        <h5 class="card-header">Delivery</h5>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Purchase</th>
+            <td>{{ object.purchase|linkify }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Receiving Contact</th>
+            <td>{{ object.receiving_contact|linkify|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Date</th>
+            <td>{{ object.date|isodate|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description|placeholder }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Assets</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:asset_list' %}?delivery_id={{ object.pk }}">{{ asset_count }}</a>
+            </td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
-        <h5 class="card-header">Deliveries</h5>
-        <div class="card-body htmx-container table-responsive"
-          hx-get="{% url 'plugins:netbox_inventory:delivery_list' %}?purchase_id={{ object.pk }}"
-          hx-trigger="load"
-        ></div>
-        {% if perms.netbox_inventory.add_delivery %}
-          <div class="card-footer text-end noprint">
-            <a href="{% url 'plugins:netbox_inventory:delivery_add' %}?purchase={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
-              <i class="mdi mdi-plus-thick" aria-hidden="true"></i>Add a Delivery
-            </a>
-          </div>
-        {% endif %}
-      </div>
-      <div class="card">
-        <h5 class="card-header">Purchased Assets</h5>
-        <div class="card-body htmx-container table-responsive"
-          hx-get="{% url 'plugins:netbox_inventory:asset_list' %}?purchase_id={{ object.pk }}"
-          hx-trigger="load"
-        ></div>
-        {% if perms.netbox_inventory.add_asset %}
-          <div class="card-footer text-end noprint">
-            <a href="{% url 'plugins:netbox_inventory:asset_add' %}?purchase={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
-              <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Asset
-            </a>
-          </div>
-        {% endif %}
+        <h5 class="card-header">
+          Delivered Assets
+          {% if perms.netbox_inventory.add_asset %}
+            <div class="card-actions">
+              <a href="{% url 'plugins:netbox_inventory:asset_add' %}?delivery={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-ghost-primary btn-sm">
+                <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add an Asset
+              </a>
+            </div>
+          {% endif %}
+        </h5>
+        {% htmx_table 'plugins:netbox_inventory:asset_list' delivery_id=object.pk %}
       </div>
       {% plugin_full_width_page object %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,27 +1,22 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
 load render_table from django_tables2 %} {% block breadcrumbs %} {{ block.super
 }}
-_{_{_ _o_b_j_e_c_t_._s_u_p_p_l_i_e_r_ _}_}
+_{_{_ _o_b_j_e_c_t_._p_u_r_c_h_a_s_e_._s_u_p_p_l_i_e_r_ _}_}
+_{_{_ _o_b_j_e_c_t_._p_u_r_c_h_a_s_e_ _}_}
 {% endblock %} {% block content %}
-**** PPuurrcchhaassee ****
-NNaammee        {{ object.name }}
-SSuupppplliieerr    {{ object.supplier|linkify }}
-SSttaattuuss      {% badge object.get_status_display bg_color=object.get_status_color
-            %}
-DDaattee        {{ object.date|annotated_date|placeholder }}
-DDeessccrriippttiioonn {{ object.description|placeholder }}
-DDeelliivveerriieess  _{_{_ _d_e_l_i_v_e_r_y___c_o_u_n_t_ _}_}
-AAsssseettss      _{_{_ _a_s_s_e_t___c_o_u_n_t_ _}_}
+**** DDeelliivveerryy ****
+NNaammee              {{ object.name }}
+PPuurrcchhaassee          {{ object.purchase|linkify }}
+RReecceeiivviinngg CCoonnttaacctt {{ object.receiving_contact|linkify|placeholder }}
+DDaattee              {{ object.date|isodate|placeholder }}
+DDeessccrriippttiioonn       {{ object.description|placeholder }}
+AAsssseettss            _{_{_ _a_s_s_e_t___c_o_u_n_t_ _}_}
 {% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
 comments.html' %} {% plugin_right_page object %}
-**** DDeelliivveerriieess ****
-{% if perms.netbox_inventory.add_delivery %}
-_A_d_d_ _a_ _D_e_l_i_v_e_r_y
-{% endif %}
-**** PPuurrcchhaasseedd AAsssseettss ****
-{% if perms.netbox_inventory.add_asset %}
-_A_d_d_ _a_n_ _A_s_s_e_t
-{% endif %}
+DDeelliivveerreedd AAsssseettss {{%% iiff ppeerrmmss..nneettbbooxx__iinnvveennttoorryy..aadddd__aasssseett %%}}
+_AA_dd_dd_ _aa_nn_ _AA_ss_ss_ee_tt
+{{%% eennddiiff %%}}
+{% htmx_table 'plugins:netbox_inventory:asset_list' delivery_id=object.pk %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/supplier.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/supplier.html`

 * *Files 8% similar despite different names*

```diff
@@ -4,70 +4,65 @@
 
 {% block breadcrumbs %}
   <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_inventory:supplier_list' %}">Suppliers</a></li>
 {% endblock %}
 
 {% block extra_controls %}
   {% if perms.netbox_inventory.add_purchase %}
-    <a href="{% url 'plugins:netbox_inventory:purchase_add' %}?supplier={{ object.pk }}" class="btn btn-sm btn-primary">
+    <a href="{% url 'plugins:netbox_inventory:purchase_add' %}?supplier={{ object.pk }}" class="btn btn-primary">
       <i class="mdi mdi-plus-thick" aria-hidden="true"></i> Add purchase
     </a>
   {% endif %}
 {% endblock extra_controls %}
 
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Supplier</h5>
-        <div class="card-body">
-          <table class="table table-hover attr-table">
-            <tr>
-              <th scope="row">Name</th>
-              <td>{{ object.name }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Description</th>
-              <td>{{ object.description }}</td>
-            </tr>
-            <tr>
-              <th scope="row">Purchases</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.pk }}">{{ purchase_count }}</a>
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Deliveries</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.pk }}">{{ delivery_count }}</a>
-              </td>
-            </tr>
-            <tr>
-              <th scope="row">Assets</th>
-              <td>
-                <a href="{% url 'plugins:netbox_inventory:asset_list' %}?supplier_id={{ object.pk }}">{{ asset_count }}</a>
-              </td>
-            </tr>
-          </table>
-        </div>
+        <table class="table table-hover attr-table">
+          <tr>
+            <th scope="row">Name</th>
+            <td>{{ object.name }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Description</th>
+            <td>{{ object.description }}</td>
+          </tr>
+          <tr>
+            <th scope="row">Purchases</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:purchase_list' %}?supplier_id={{ object.pk }}">{{ purchase_count }}</a>
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Deliveries</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:delivery_list' %}?supplier_id={{ object.pk }}">{{ delivery_count }}</a>
+            </td>
+          </tr>
+          <tr>
+            <th scope="row">Assets</th>
+            <td>
+              <a href="{% url 'plugins:netbox_inventory:asset_list' %}?supplier_id={{ object.pk }}">{{ asset_count }}</a>
+            </td>
+          </tr>
+        </table>
       </div>
       {% include 'inc/panels/tags.html' %}
       {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
       {% plugin_right_page object %}
     </div>
   </div>
   <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Supplied Assets</h5>
-        <div class="card-body htmx-container table-responsive"
-          hx-get="{% url 'plugins:netbox_inventory:asset_list' %}?supplier_id={{ object.pk }}"
-          hx-trigger="load"
-        ></div>
+        {% htmx_table 'plugins:netbox_inventory:asset_list' supplier_id=object.pk %}
       </div>
       {% plugin_full_width_page object %}
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -11,9 +11,10 @@
 PPuurrcchhaasseess   _{_{_ _p_u_r_c_h_a_s_e___c_o_u_n_t_ _}_}
 DDeelliivveerriieess  _{_{_ _d_e_l_i_v_e_r_y___c_o_u_n_t_ _}_}
 AAsssseettss      _{_{_ _a_s_s_e_t___c_o_u_n_t_ _}_}
 {% include 'inc/panels/tags.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
 comments.html' %} {% plugin_right_page object %}
 **** SSuupppplliieedd AAsssseettss ****
+{% htmx_table 'plugins:netbox_inventory:asset_list' supplier_id=object.pk %}
 {% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_base.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_location.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_rack.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html` & `netbox_inventory-2.0.0/netbox_inventory/templates/netbox_inventory/tabs/located_assets_site.html`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_api.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import copy
-from django.contrib.contenttypes.models import ContentType
+
+from core.models import ObjectType
 from dcim.models import Device, DeviceRole, DeviceType, InventoryItem, Manufacturer, ModuleType, Site
 from users.models import ObjectPermission
 from utilities.testing import APIViewTestCases, disable_warnings
 from rest_framework import status
 
 from ..custom import APITestCase
 from ...models import Asset, Delivery, InventoryItemType, Purchase, Supplier
@@ -13,15 +14,15 @@
         APITestCase, 
         APIViewTestCases.GetObjectViewTestCase,
         APIViewTestCases.ListObjectsViewTestCase,
         APIViewTestCases.CreateObjectViewTestCase,
         APIViewTestCases.UpdateObjectViewTestCase,
         APIViewTestCases.DeleteObjectViewTestCase):
     model = Asset
-    brief_fields = ['display', 'id', 'serial', 'url']
+    brief_fields = ['display', 'id', 'name', 'serial', 'url']
 
     bulk_update_data = {
         'status': 'used',
     }
 
     def test_assign_device_matching_device_type(self):
         """
@@ -30,15 +31,15 @@
         # Add object-level permission
         obj_perm = ObjectPermission(
             name='Test permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         update_data = {'device':self.device1.pk}
 
         response = self.client.post(self._get_list_url(), self.create_data[0], format='json', **self.header)
         instance = self._get_queryset().get(pk=response.data['id'])
         url = self._get_detail_url(instance)
         response = self.client.patch(url, update_data, format='json', **self.header)
@@ -58,15 +59,15 @@
         # Add object-level permission
         obj_perm = ObjectPermission(
             name='Test permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         update_data = {'device':self.device2.pk}
 
         response = self.client.post(self._get_list_url(), self.create_data[0], format='json', **self.header)
         instance = self._get_queryset().get(pk=response.data['id'])
         url = self._get_detail_url(instance)
         response = self.client.patch(url, update_data, format='json', **self.header)
@@ -80,15 +81,15 @@
         # Add object-level permission
         obj_perm = ObjectPermission(
             name='Test permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         update_data = {'inventoryitem':self.inventoryitem1.pk}
 
         response = self.client.post(self._get_list_url(), self.create_data[0], format='json', **self.header)
         instance = self._get_queryset().get(pk=response.data['id'])
         url = self._get_detail_url(instance)
         response = self.client.patch(url, update_data, format='json', **self.header)
@@ -102,15 +103,15 @@
         # Add object-level permission
         obj_perm = ObjectPermission(
             name='Test permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         create_data = self.create_data[2]
         response = self.client.post(self._get_list_url(), create_data, format='json', **self.header)
         instance = self._get_queryset().get(pk=response.data['id'])
         self.assertEqual(instance.purchase, self.purchase1)
 
     def test_serial_asset_tag_empty(self):
@@ -120,15 +121,15 @@
         # Add object-level permission
         obj_perm = ObjectPermission(
             name='Test permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         create_data = copy(self.create_data[0])
         create_data['serial'] = ''
         create_data['asset_tag'] = ''
         response = self.client.post(self._get_list_url(), create_data, format='json', **self.header)
         instance = self._get_queryset().get(pk=response.data['id'])
         self.assertEqual(instance.serial, None)
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_models.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from django.contrib.contenttypes.models import ContentType
 from django.test import override_settings
 
+from core.models import ObjectType
 from dcim.models import Manufacturer, DeviceType, DeviceRole, Device, Site
 from users.models import ObjectPermission
 from utilities.testing import post_data, ViewTestCases
 
 from netbox_inventory.tests.custom import ModelViewTestCase
 from netbox_inventory.models import Asset, Delivery, Purchase, Supplier
 from ..settings import CONFIG_ALLOW_CREATE_DEVICE_TYPE
@@ -104,16 +104,16 @@
         # Assign unconstrained permission
         obj_perm = ObjectPermission(
             name='test-device-assign permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
-        obj_perm.object_types.add(ContentType.objects.get_for_model(Device))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(Device))
 
         asset = Asset.objects.create(
             status='stored',
             serial='123assign',
             device_type=DeviceType.objects.first(),
         )
         device = Device.objects.create(
@@ -156,15 +156,15 @@
         # Assign unconstrained permission
         obj_perm = ObjectPermission(
             name='test-asset permission',
             actions=['add', 'change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         supplier1 = Supplier.objects.create(
             name='Supplier1-autoset',
             slug='supplier1-autoset',
         )
         purchase1 = Purchase.objects.create(
             name='Purchase1-autoset',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_create.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_create.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/asset/test_views_reassign.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/asset/test_views_reassign.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.contrib.contenttypes.models import ContentType
 from django.test import override_settings
 
+from core.models import ObjectType
 from dcim.models import Manufacturer, DeviceType, DeviceRole, Device, InventoryItem, Module, ModuleBay, ModuleType, Site
 from extras.choices import ObjectChangeActionChoices
 from extras.models import ObjectChange
 from users.models import ObjectPermission
 from utilities.testing import ViewTestCases
 from utilities.testing.utils import post_data
 
@@ -133,15 +134,15 @@
         # Assign model-level permission
         obj_perm = ObjectPermission(
             name='Test permission',
             actions=['change']
         )
         obj_perm.save()
         obj_perm.users.add(self.user)
-        obj_perm.object_types.add(ContentType.objects.get_for_model(self.model))
+        obj_perm.object_types.add(ObjectType.objects.get_for_model(self.model))
 
         # Try GET with model-level permission
         self.assertHttpStatus(self.client.get(self._get_url('edit', instance)), 200)
 
         # Try POST with model-level permission
         request = {
             'path': self._get_url('edit', instance),
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/custom.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_api.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         APITestCase, 
         APIViewTestCases.GetObjectViewTestCase,
         APIViewTestCases.ListObjectsViewTestCase,
         APIViewTestCases.CreateObjectViewTestCase,
         APIViewTestCases.UpdateObjectViewTestCase,
         APIViewTestCases.DeleteObjectViewTestCase):
     model = Delivery
-    brief_fields = ['date', 'display', 'id', 'name', 'url']
+    brief_fields = ['date', 'description', 'display', 'id', 'name', 'url']
 
     bulk_update_data = {
         'description': 'new description',
     }
 
     @classmethod
     def setUpTestData(cls) -> None:
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/delivery/test_views.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/delivery/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_api.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_group/test_views.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_group/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_api.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/inventoryitem_type/test_views.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/inventoryitem_type/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_api.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         APITestCase, 
         APIViewTestCases.GetObjectViewTestCase,
         APIViewTestCases.ListObjectsViewTestCase,
         APIViewTestCases.CreateObjectViewTestCase,
         APIViewTestCases.UpdateObjectViewTestCase,
         APIViewTestCases.DeleteObjectViewTestCase):
     model = Purchase
-    brief_fields = ['date', 'display', 'id', 'name', 'status', 'supplier', 'url']
+    brief_fields = ['date', 'description', 'display', 'id', 'name', 'status', 'supplier', 'url']
 
     bulk_update_data = {
         'description': 'new description',
     }
 
     @classmethod
     def setUpTestData(cls) -> None:
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/purchase/test_views.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/purchase/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/settings.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/settings.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_api.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         APITestCase, 
         APIViewTestCases.GetObjectViewTestCase,
         APIViewTestCases.ListObjectsViewTestCase,
         APIViewTestCases.CreateObjectViewTestCase,
         APIViewTestCases.UpdateObjectViewTestCase,
         APIViewTestCases.DeleteObjectViewTestCase):
     model = Supplier
-    brief_fields = ['display', 'id', 'name', 'slug', 'url']
+    brief_fields = ['description', 'display', 'id', 'name', 'slug', 'url']
     create_data = [
         {
             'name': 'Supplier 4',
             'slug': 'supplier4',
         },
         {
             'name': 'Supplier 5',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/supplier/test_views.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/supplier/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             ),
         )
         ContactAssignment.objects.bulk_create(assignments)
 
         tags = create_tags('Alpha', 'Bravo', 'Charlie')
 
         cls.form_data = {
-            'content_type': ContentType.objects.get_for_model(Supplier).pk,
+            'object_type': ContentType.objects.get_for_model(Supplier).pk,
             'object_id': suppliers[3].pk,
             'contact': contacts[3].pk,
             'role': contact_roles[3].pk,
             'priority': ContactPriorityChoices.PRIORITY_INACTIVE,
             'tags': [t.pk for t in tags],
         }
 
@@ -129,10 +129,10 @@
 
     def _get_url(self, action, instance=None):
         # Override creation URL to append content_type & object_id parameters
         if action == 'add':
             url = reverse('tenancy:contactassignment_add')
             content_type = ContentType.objects.get_for_model(Supplier).pk
             object_id = Supplier.objects.first().pk
-            return f"{url}?content_type={content_type}&object_id={object_id}"
+            return f"{url}?object_type={content_type}&object_id={object_id}"
 
         return super()._get_url(action, instance=instance)
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/tests/test_load.py` & `netbox_inventory-2.0.0/netbox_inventory/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class NetboxInventoryVersionTestCase(SimpleTestCase):
     """
     Test for netbox_inventory package
     """
 
     def test_version(self):
-        assert __version__ == "1.6.0"
+        assert __version__ == "2.0.0"
 
 
 class AppTest(APITestCase):
     """
     Test the availability of the plugin API root
     """
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/urls.py` & `netbox_inventory-2.0.0/netbox_inventory/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/utils.py` & `netbox_inventory-2.0.0/netbox_inventory/utils.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/asset.py` & `netbox_inventory-2.0.0/netbox_inventory/views/asset.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/asset_assign.py` & `netbox_inventory-2.0.0/netbox_inventory/views/asset_assign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/asset_create.py` & `netbox_inventory-2.0.0/netbox_inventory/views/asset_create.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,12 +56,7 @@
 
 class AssetInventoryItemCreateView(AssetCreateView):
     queryset = InventoryItem.objects.all()
     form = AssetInventoryItemCreateForm
 
     def get_object(self, **kwargs):
         return InventoryItem(assigned_asset=self.asset)
-
-    def get_extra_context(self, request, instance):
-        context = super().get_extra_context(request, instance)
-        context['template_extends'] = 'dcim/inventoryitem_edit.html'
-        return context
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/asset_reassign.py` & `netbox_inventory-2.0.0/netbox_inventory/views/asset_reassign.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/delivery.py` & `netbox_inventory-2.0.0/netbox_inventory/views/delivery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.views import generic
-from utilities.utils import count_related
+from utilities.query import count_related
 from .. import filtersets, forms, models, tables
 
 __all__ = (
     'DeliveryView',
     'DeliveryListView',
     'DeliveryEditView',
     'DeliveryDeleteView',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_group.py` & `netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_group.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/inventoryitem_type.py` & `netbox_inventory-2.0.0/netbox_inventory/views/inventoryitem_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.views import generic
-from utilities.utils import count_related
+from utilities.query import count_related
 from .. import filtersets, forms, models, tables
 
 __all__ = (
     'InventoryItemTypeView',
     'InventoryItemTypeListView',
     'InventoryItemTypeEditView',
     'InventoryItemTypeDeleteView',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/purchase.py` & `netbox_inventory-2.0.0/netbox_inventory/views/purchase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from netbox.views import generic
-from utilities.utils import count_related
+from utilities.query import count_related
 from .. import filtersets, forms, models, tables
 
 __all__ = (
     'PurchaseView',
     'PurchaseListView',
     'PurchaseEditView',
     'PurchaseDeleteView',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/supplier.py` & `netbox_inventory-2.0.0/netbox_inventory/views/supplier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from netbox.views import generic
 from tenancy.views import ObjectContactsView
-from utilities.utils import count_related
+from utilities.query import count_related
 from utilities.views import register_model_view
 from .. import filtersets, forms, models, tables
 
 __all__ = (
     'SupplierView',
     'SupplierListView',
     'SupplierEditView',
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory/views/tabs.py` & `netbox_inventory-2.0.0/netbox_inventory/views/tabs.py`

 * *Files identical despite different names*

### Comparing `netbox_inventory-1.6.0/netbox_inventory.egg-info/PKG-INFO` & `netbox_inventory-2.0.0/netbox_inventory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: netbox-inventory
-Version: 1.6.0
+Version: 2.0.0
 Summary: Inventory asset management in NetBox
 Author-email: Matej Vadnjal <matej.vadnjal@arnes.si>
 Project-URL: Homepage, https://github.com/ArnesSI/netbox-inventory/
 Project-URL: Bug Tracker, https://github.com/ArnesSI/netbox-inventory/issues/
 Keywords: netbox,netbox-plugin,inventory
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NetBox Inventory Plugin
 
 A [Netbox](https://github.com/netbox-community/netbox) plugin for hardware inventory.
 
@@ -67,24 +67,21 @@
 
 With `asset_disable_editing_fields_for_tags` and `asset_disable_deletion_for_tags` you can prevent changes to specified asset data for assets that have certain tags attached. Changes are only prevented via web interface. API modifications are allowed.
 
 The idea is that an external system uses some assets stored in netbox_inventory, and you want to prevent accidental changes to data directly in NetBox web interface. Only that external system should modify the data.
 
 ## Compatibility
 
-This plugin requires netbox version 3.7.x to work. Older versions of the plugin
+This plugin requires netbox version 4.0 to work. Older versions of the plugin
 support older netbox version as per table below:
 
 | NetBox Version | Plugin Version |
 |----------------|----------------|
-|       3.3      |      1.1.x     |
-|       3.4      |      1.2.x     |
-|       3.5      | 1.3.x & 1.4.x  |
-|       3.6      |      1.5.x     |
 |       3.7      |      1.6.x     |
+|       4.0      |      2.0.x     |
 
 ## Installing
 
 Review [official Netbox plugin documentation](https://docs.netbox.dev/en/stable/plugins/#installing-plugins) for installation instructions.
 
 You install the plugin from pypi with pip. Make sure you activate Netbox's virtual
 environment first:
```

### Comparing `netbox_inventory-1.6.0/netbox_inventory.egg-info/SOURCES.txt` & `netbox_inventory-2.0.0/netbox_inventory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 netbox_inventory/management/commands/check_asset_tags.py
 netbox_inventory/migrations/0001_initial_prod.py
 netbox_inventory/migrations/0002_alter_asset_serial.py
 netbox_inventory/migrations/0003_add_inventoryitemgroup.py
 netbox_inventory/migrations/0004_inventoryitemgroup_tree.py
 netbox_inventory/migrations/0005_delivery_asset_delivery.py
 netbox_inventory/migrations/0006_purchase_status.py
+netbox_inventory/migrations/0007_alter_asset_unique_together_and_more.py
 netbox_inventory/migrations/__init__.py
 netbox_inventory/templates/netbox_inventory/asset.html
 netbox_inventory/templates/netbox_inventory/asset_assign.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_add.html
 netbox_inventory/templates/netbox_inventory/asset_bulk_import.html
 netbox_inventory/templates/netbox_inventory/asset_create.html
 netbox_inventory/templates/netbox_inventory/asset_edit.html
```

### Comparing `netbox_inventory-1.6.0/pyproject.toml` & `netbox_inventory-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-inventory"
-version = "1.6.0"
+version = "2.0.0"
 authors = [
   { name="Matej Vadnjal", email="matej.vadnjal@arnes.si" },
 ]
 description = "Inventory asset management in NetBox"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["netbox", "netbox-plugin", "inventory"]
```


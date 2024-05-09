# Comparing `tmp/descarteslabs-3.0.5.tar.gz` & `tmp/descarteslabs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descarteslabs-3.0.5.tar", last modified: Thu Mar 21 23:58:52 2024, max compression
+gzip compressed data, was "descarteslabs-3.1.0.tar", last modified: Thu May  9 15:51:28 2024, max compression
```

## Comparing `descarteslabs-3.0.5.tar` & `descarteslabs-3.1.0.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)   100162 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29549 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/auth/tests/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/compute/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/config/
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/config/settings.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/config/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/config/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/config/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs/core/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.463572 descarteslabs-3.0.5/descarteslabs/core/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64062 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    33151 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/band.py
--rw-r--r--   0 runner    (1001) docker     (127)    37222 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/blob_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/blob_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/blob_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    37891 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/catalog_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.463572 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/blobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/products.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.463572 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    63700 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    49929 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/image_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/image_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/image_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/named_catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21219 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/product.py
--rw-r--r--   0 runner    (1001) docker     (127)    25947 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.467572 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   115187 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_band.py
--rw-r--r--   0 runner    (1001) docker     (127)    32203 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)    16050 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_catalog_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    46052 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_image_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    24940 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_image_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    23871 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_product.py
--rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19934 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.467572 descarteslabs-3.0.5/descarteslabs/core/client/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/addons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.467572 descarteslabs-3.0.5/descarteslabs/core/client/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.467572 descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.467572 descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/scripts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/scripts/lazy_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/scripts/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/geotiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41637 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/test_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/services/service/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/service/api_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    29553 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/services/service/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/service/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/services/service/tests/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/tests/test_clear_client_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.471572 descarteslabs-3.0.5/descarteslabs/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/client/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/client/tests/test_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15901 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/collection/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/collection/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/collection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/collection/tests/test_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/display/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/display/_display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/display/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/display/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/display/tests/test_display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/dltile/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/_tiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/rasterize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/dltile/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/tests/test_dltiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19537 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dltile/utm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.475572 descarteslabs-3.0.5/descarteslabs/core/common/dotdict/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dotdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dotdict/dotdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/dotdict/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dotdict/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14087 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/dotdict/tests/test_dotdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51950 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/geo/geocontext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/geo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/geo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/geo/tests/test_geocontext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/geo/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/geo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/http/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/http/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/tests/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/retry/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/retry/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.479572 descarteslabs-3.0.5/descarteslabs/core/common/retry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/retry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/retry/tests/test_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/common/threading/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/threading/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/common/threading/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/threading/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/threading/tests/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/common/vector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/common/vector/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/compute/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/compute_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    54978 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/job_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/compute/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/compute/tests/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/third_party/boltons/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/third_party/boltons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32185 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/third_party/boltons/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.483572 descarteslabs-3.0.5/descarteslabs/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/descarteslabs/core/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/features.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/products.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/descarteslabs/core/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_products.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    42046 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/core/vector/vector_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/descarteslabs/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/descarteslabs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/descarteslabs/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/descarteslabs/vector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:58:52.459572 descarteslabs-3.0.5/descarteslabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-21 23:58:52.000000 descarteslabs-3.0.5/descarteslabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-03-21 23:58:52.000000 descarteslabs-3.0.5/descarteslabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 23:58:52.000000 descarteslabs-3.0.5/descarteslabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-21 23:58:52.000000 descarteslabs-3.0.5/descarteslabs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-21 23:58:52.000000 descarteslabs-3.0.5/descarteslabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-21 23:58:52.000000 descarteslabs-3.0.5/descarteslabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 23:58:52.487572 descarteslabs-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-21 23:58:48.000000 descarteslabs-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)   101712 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.898627 descarteslabs-3.1.0/descarteslabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.898627 descarteslabs-3.1.0/descarteslabs/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29549 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.898627 descarteslabs-3.1.0/descarteslabs/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/auth/tests/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.898627 descarteslabs-3.1.0/descarteslabs/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.898627 descarteslabs-3.1.0/descarteslabs/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.902627 descarteslabs-3.1.0/descarteslabs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/config/settings.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.902627 descarteslabs-3.1.0/descarteslabs/config/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/config/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/config/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.902627 descarteslabs-3.1.0/descarteslabs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.902627 descarteslabs-3.1.0/descarteslabs/core/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64062 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33151 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/band.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42475 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/blob_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/blob_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37891 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/catalog_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.906627 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/blobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.906627 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63700 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49929 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/image_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/image_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/image_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8588 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/named_catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25947 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.906627 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115187 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36523 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_band.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34326 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16050 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_catalog_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46052 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_image_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24940 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_image_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23881 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19934 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.906627 descarteslabs-3.1.0/descarteslabs/core/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/addons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.906627 descarteslabs-3.1.0/descarteslabs/core/client/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/scripts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/scripts/lazy_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/scripts/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/geotiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41637 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/test_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/services/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/service/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29553 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/services/service/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/service/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/services/service/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/tests/test_clear_client_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.910627 descarteslabs-3.1.0/descarteslabs/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/client/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15901 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/collection/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/collection/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/collection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/collection/tests/test_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/display/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/display/_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/display/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/display/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/display/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/dltile/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/_tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/rasterize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/dltile/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/tests/test_dltiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19537 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dltile/utm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.914627 descarteslabs-3.1.0/descarteslabs/core/common/dotdict/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dotdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dotdict/dotdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/dotdict/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dotdict/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14087 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/dotdict/tests/test_dotdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51950 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/geo/geocontext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/geo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/geo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/geo/tests/test_geocontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/geo/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/geo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/http/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22688 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/tests/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/retry/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/retry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/retry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/retry/tests/test_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.918627 descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/common/threading/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/threading/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/common/threading/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/threading/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/threading/tests/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/common/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/common/vector/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/compute_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54978 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/job_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/compute/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32325 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/compute/tests/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/third_party/boltons/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/third_party/boltons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32185 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/third_party/boltons/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.922627 descarteslabs-3.1.0/descarteslabs/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/descarteslabs/core/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/descarteslabs/core/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42046 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/core/vector/vector_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/descarteslabs/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/descarteslabs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/descarteslabs/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/descarteslabs/vector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:51:28.898627 descarteslabs-3.1.0/descarteslabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-09 15:51:28.000000 descarteslabs-3.1.0/descarteslabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-09 15:51:28.000000 descarteslabs-3.1.0/descarteslabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:51:28.000000 descarteslabs-3.1.0/descarteslabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 15:51:28.000000 descarteslabs-3.1.0/descarteslabs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-09 15:51:28.000000 descarteslabs-3.1.0/descarteslabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 15:51:28.000000 descarteslabs-3.1.0/descarteslabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:51:28.926627 descarteslabs-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-09 15:51:20.000000 descarteslabs-3.1.0/setup.py
```

### Comparing `descarteslabs-3.0.5/LICENSE` & `descarteslabs-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/PKG-INFO` & `descarteslabs-3.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: descarteslabs
-Version: 3.0.5
+Version: 3.1.0
 Summary: Descartes Labs Python Client
 Home-page: https://github.com/descarteslabs/descarteslabs-python
 Author: Descartes Labs
 Author-email: hello@descarteslabs.com
 License: Apache 2.0
-Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v3.0.5.tar.gz
+Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v3.1.0.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: ~=3.8
+Requires-Python: ~=3.9
 Provides-Extra: complete
 Provides-Extra: tests
 Provides-Extra: visualization
 License-File: LICENSE
 
 .. code-block:: bash
```

### Comparing `descarteslabs-3.0.5/README.md` & `descarteslabs-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 The `descarteslabs` python package, available at [https://pypi.org/project/descarteslabs/](https://pypi.org/project/descarteslabs/), provides client-side access to the Descartes Labs Platform for our customers. You must be a registered customer with access to our Descartes Labs Platform before you can make use of this package with our platform.
 
 The documentation for the latest release can be found at [https://docs.descarteslabs.com](https://docs.descarteslabs.com). For any issues please request Customer Support at [https://support.descarteslabs.com](https://support.descarteslabs.com).
 
 Changelog
 =========
 
+## [3.1.0] - 2024-05-09
+
+### General
+
+- Due to declining support for Python 3.8 across the ecosystem, we have discontinued our support for Python 3.8. It is expected that the client will continue to function until Python 3.8 is End of Life (October 2024), but we can no longer test new releases against this version.
+
+### Catalog
+
+- The Catalog Storage Blob deletion methods have been enhanced to support waiting for completion of the operation. When a blob is deleted, it is removed immediately from the catalog and a background asynchronous task is launched to clean up the contents of the blob from the backing storage. If a blob is deleted and then a new blob with the identical id is immediately created and uploaded before this background task completes, it is possible for the background task to end up deleting the new blob contents. As of this release the `Blob` instance and class delete methods return a `BlobDeletionTaskStatus` object which provides a `wait_for_completion` method which can be used to wait until the background task completes and it is safe to create a new blob with the same id. For the `Blob.delete_many` method, the `wait_for_completion=True` parameter can be used to wait for all the supplied blobs to be completely deleted. Note that in the case of the `Blob.delete` class method, this is a very slight breaking change, as it used to return True or False, and now instead returns a `BlobDeletionTaskStatus` or `None`, which have the same truthiness and hence are very likely to behave identically in practical use.
+
 ## [3.0.5] - 2024-03-21
 
 Bugfix only
 
 ### General
 
 - The `descarteslabs` client CLI script generated by the installation process was broken. Now it works!
```

### Comparing `descarteslabs-3.0.5/descarteslabs/__init__.py` & `descarteslabs-3.1.0/descarteslabs/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/auth/__init__.py` & `descarteslabs-3.1.0/descarteslabs/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/auth/auth.py` & `descarteslabs-3.1.0/descarteslabs/auth/auth.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/auth/tests/test_auth.py` & `descarteslabs-3.1.0/descarteslabs/auth/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/catalog/__init__.py` & `descarteslabs-3.1.0/descarteslabs/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/compute/__init__.py` & `descarteslabs-3.1.0/descarteslabs/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/config/__init__.py` & `descarteslabs-3.1.0/descarteslabs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/config/settings.toml` & `descarteslabs-3.1.0/descarteslabs/config/settings.toml`

 * *Files 5% similar despite different names*

```diff
@@ -63,21 +63,21 @@
 iam_url = "@format https://iam.{this.DEFAULT_DOMAIN}"
 metadata_url = "@format {this.PLATFORM_URL}/metadata/v1"
 raster_url = "@format {this.PLATFORM_URL}/raster/v2"
 usage_url = "@format {this.PLATFORM_URL}/usage/v1"
 vector_url = "@format {this.PLATFORM_URL}/vector/v1"
 yaas_url = "@format {this.PLATFORM_URL}/yaas/v1"
 
-[aws-testing]
-# testing is now for aws but keep this until it is removed everywhere
-default_domain = "@format dev.aws.{this.DOMAIN}"
-platform_url = "@format https://platform.{this.DEFAULT_DOMAIN}"
+[local]
+# feel free to mess with anything here as needed
+default_domain = "dev.localhost"
+platform_url = "@format https://platform.dev.aws.descarteslabs.com"
 testing = true
 
 catalog_v2_url = "@format {this.PLATFORM_URL}/metadata/v1/catalog/v2"
 compute_url = "@format {this.PLATFORM_URL}/compute/v1"
-iam_url = "@format https://iam.{this.DEFAULT_DOMAIN}"
+iam_url = "@format https://{this.DEFAULT_DOMAIN}:8000"
 metadata_url = "@format {this.PLATFORM_URL}/metadata/v1"
 raster_url = "@format {this.PLATFORM_URL}/raster/v2"
 usage_url = "@format {this.PLATFORM_URL}/usage/v1"
 vector_url = "@format {this.PLATFORM_URL}/vector/v1"
 yaas_url = "@format {this.PLATFORM_URL}/yaas/v1"
```

### Comparing `descarteslabs-3.0.5/descarteslabs/config/tests/test_config.py` & `descarteslabs-3.1.0/descarteslabs/config/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         settings = Settings.get_settings()
         self.assertEqual(settings.current_env, os.environ.get("DESCARTESLABS_ENV"))
         self.assertEqual(id(settings), id(Settings._settings))
         self.assertEqual(id(settings), id(Settings.get_settings()))
 
     def test_peek_settings(self):
         current_env = os.environ["DESCARTESLABS_ENV"]
-        env = "aws-testing"
+        env = "aws-production"
         settings = Settings.peek_settings(env)
         assert os.environ["DESCARTESLABS_ENV"] == current_env
         assert settings.env == env
         assert Settings._settings is None
 
     def test_bad_env(self):
         env = "non-existent"
@@ -101,30 +101,25 @@
             Settings.peek_settings(env)
 
         with self.assertRaises(ConfigError):
             Settings.select_env(env)
 
     def test_default_auth(self):
         a = Auth()
-        a.domain == "http://gcp_url"
+        assert a.domain == "https://iam.dev.aws.descarteslabs.com"
 
     def test_auth_with_env(self):
-        with patch.dict(os.environ, {"DESCARTESLABS_ENV": "aws-testing"}):
+        with patch.dict(os.environ, {"DESCARTESLABS_ENV": "aws-production"}):
             a = Auth()
-            a.domain == "http://aws_url"
+            assert a.domain == "https://iam.production.aws.descarteslabs.com"
 
-    def test_auth_with_aws_config(self):
-        Settings.select_env("aws-testing")
+    def test_auth_with_test_config(self):
+        Settings.select_env("aws-production")
         a = Auth()
-        a.domain == "http://aws_url"
-
-    def test_auth_with_gcp_config(self):
-        Settings.select_env("testing")
-        a = Auth()
-        a.domain == "http://gcp_url"
+        assert a.domain == "https://iam.production.aws.descarteslabs.com"
 
     def test_env(self):
         peek1_env = "aws-dev"
         env = "aws-staging"
 
         assert Settings.env is None
         s1 = Settings.peek_settings(peek1_env)
@@ -171,27 +166,14 @@
             "METADATA_URL": "https://platform.staging.aws.descarteslabs.com/metadata/v1",
             "PLATFORM_URL": "https://platform.staging.aws.descarteslabs.com",
             "RASTER_URL": "https://platform.staging.aws.descarteslabs.com/raster/v2",
             "USAGE_URL": "https://platform.staging.aws.descarteslabs.com/usage/v1",
             "VECTOR_URL": "https://platform.staging.aws.descarteslabs.com/vector/v1",
             "YAAS_URL": "https://platform.staging.aws.descarteslabs.com/yaas/v1",
         },
-        "aws-testing": {
-            "CATALOG_V2_URL": "https://platform.dev.aws.descarteslabs.com/metadata/v1/catalog/v2",
-            "COMPUTE_URL": "https://platform.dev.aws.descarteslabs.com/compute/v1",
-            "IAM_URL": "https://iam.dev.aws.descarteslabs.com",
-            "LOG_LEVEL": "WARNING",
-            "METADATA_URL": "https://platform.dev.aws.descarteslabs.com/metadata/v1",
-            "PLATFORM_URL": "https://platform.dev.aws.descarteslabs.com",
-            "RASTER_URL": "https://platform.dev.aws.descarteslabs.com/raster/v2",
-            "TESTING": True,
-            "USAGE_URL": "https://platform.dev.aws.descarteslabs.com/usage/v1",
-            "VECTOR_URL": "https://platform.dev.aws.descarteslabs.com/vector/v1",
-            "YAAS_URL": "https://platform.dev.aws.descarteslabs.com/yaas/v1",
-        },
         "testing": {
             "CATALOG_V2_URL": "https://platform.dev.aws.descarteslabs.com/metadata/v1/catalog/v2",
             "COMPUTE_URL": "https://platform.dev.aws.descarteslabs.com/compute/v1",
             "IAM_URL": "https://iam.dev.aws.descarteslabs.com",
             "LOG_LEVEL": "WARNING",
             "METADATA_URL": "https://platform.dev.aws.descarteslabs.com/metadata/v1",
             "PLATFORM_URL": "https://platform.dev.aws.descarteslabs.com",
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from .task import TaskState
 from .product import (
     DeletionTaskStatus,
     Product,
     ProductCollection,
-    TaskState,
 )
 from .band import (
     Band,
     BandCollection,
     BandType,
     ClassBand,
     Colormap,
@@ -34,15 +34,22 @@
     GenericBand,
     MaskBand,
     MicrowaveBand,
     ProcessingLevelsAttribute,
     ProcessingStepAttribute,
     SpectralBand,
 )
-from .blob import Blob, BlobCollection, BlobSearch, BlobSummaryResult, StorageType
+from .blob import (
+    Blob,
+    BlobCollection,
+    BlobDeletionTaskStatus,
+    BlobSearch,
+    BlobSummaryResult,
+    StorageType,
+)
 from .image import Image, ImageSearch, ImageSummaryResult
 from .image_types import ResampleAlgorithm, DownloadFileFormat
 from .image_upload import (
     ImageUpload,
     ImageUploadEvent,
     ImageUploadEventSeverity,
     ImageUploadEventType,
@@ -83,14 +90,15 @@
     "AggregateDateField",
     "AttributeValidationError",
     "Band",
     "BandCollection",
     "BandType",
     "Blob",
     "BlobCollection",
+    "BlobDeletionTaskStatus",
     "BlobSearch",
     "BlobSummaryResult",
     "CatalogClient",
     "CatalogObject",
     "ClassBand",
     "Colormap",
     "DataType",
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/attributes.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/band.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/band.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/blob.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/blob.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,18 +27,24 @@
     GeometryAttribute,
     ListAttribute,
     StorageState,
     Timestamp,
     TypedAttribute,
     parse_iso_datetime,
 )
-from .blob_delete import BlobDelete
 from .blob_download import BlobDownload
-from .catalog_base import CatalogClient, CatalogObject, check_deleted
+from .catalog_base import (
+    CatalogClient,
+    CatalogObject,
+    check_deleted,
+    check_derived,
+    UnsavedObjectError,
+)
 from .search import AggregateDateField, GeoSearch, SummarySearchMixin
+from .task import TaskStatus
 
 properties = Properties()
 
 
 class StorageType(StrEnum):
     """The storage type for a blob.
 
@@ -907,28 +913,35 @@
                     response.close()
 
             dest = generator
 
         return cls(id=id, client=client)._do_download(dest=dest, range=range)
 
     @classmethod
-    def delete_many(cls, ids, client=None):
+    def delete_many(
+        cls, ids, raise_on_missing=False, wait_for_completion=False, client=None
+    ):
         """Delete many blobs from the Descartes Labs catalog.
 
         Only those blobs that exist and are owned by the user will be deleted.
-        No errors will be raised for blobs that do not exist or are not owned by
-        the user. If you need to know, compare the supplied list of ids with the
-        returned list of delete ids.
+        No errors will be raised for blobs that do not exist or are visible but
+        not owned by the user. If you need to know, compare the supplied list of
+        ids with the returned list of deleted ids.
 
         All blobs to be deleted must belong to the same purchase.
 
         Parameters
         ----------
         ids : list(str)
             A list of blob ids to delete.
+        raise_on_missing : bool, optional
+            If True, raise an exception if any of the blobs are not found, otherwise ignore
+            missing blobs. Defaults to False.
+        wait_for_completion : bool, optional
+            If True, wait for the deletion to complete before returning. Defaults to False.
         client : CatalogClient, optional
             A `CatalogClient` instance to use for requests to the Descartes Labs catalog.
             The :py:meth:`~descarteslabs.catalog.CatalogClient.get_default_client` will
             be used if not set.
 
         Returns
         -------
@@ -937,19 +950,25 @@
 
         Raises
         ------
         ~descarteslabs.exceptions.ClientError or ~descarteslabs.exceptions.ServerError
             :ref:`Spurious exception <network_exceptions>` that can occur during a
             network request.
         """
-        blob_delete = BlobDelete(ids=ids, client=client)
+        if client is None:
+            client = CatalogClient.get_default_client()
 
-        blob_delete.save()
+        task_status = BlobDeletionTaskStatus.create(
+            ids=ids, raise_on_missing=raise_on_missing, client=client
+        )
 
-        return blob_delete.ids
+        if wait_for_completion:
+            task_status.wait_for_completion()
+
+        return task_status.ids
 
     def _do_download(self, dest=None, range=None):
         download = BlobDownload.get(id=self.id, client=self._client)
 
         # BlobDownload.get() returns None if the blob does not exist
         # raise a NotFoundError in this case
         if not download:
@@ -989,14 +1008,151 @@
                 else:
                     for chunk in r.iter_content(1048576):
                         dest.write(chunk)
                     return dest.name
             finally:
                 r.close()
 
+    @classmethod
+    @check_derived
+    def delete(cls, id, client=None):
+        """Delete the catalog object with the given `id`.
+
+        Parameters
+        ----------
+        id : str
+            The id of the object to be deleted.
+        client : CatalogClient, optional
+            A `CatalogClient` instance to use for requests to the Descartes Labs
+            catalog.  The
+            :py:meth:`~descarteslabs.catalog.CatalogClient.get_default_client` will
+            be used if not set.
+
+        Returns
+        -------
+        BlobDeletionTaskStatus
+            The status of the deletion task which can be used to wait for completion. ``None`` if the
+            object was not found.
+
+        Raises
+        ------
+        ConflictError
+            If the object has related objects (bands, images) that exist.
+        ~descarteslabs.exceptions.ClientError or ~descarteslabs.exceptions.ServerError
+            :ref:`Spurious exception <network_exceptions>` that can occur during a
+            network request.
+
+        Example
+        -------
+        >>> Image.delete('my-image-id') # doctest: +SKIP
+        """
+        if client is None:
+            client = CatalogClient.get_default_client()
+
+        try:
+            return BlobDeletionTaskStatus.create(
+                ids=[id], raise_on_missing=True, client=client
+            )
+        except NotFoundError:
+            return None
+
+    @check_deleted
+    def _instance_delete(self):
+        """Delete this catalog object from the Descartes Labs catalog.
+
+        Once deleted, you cannot use the catalog object and should release any
+        references.
+
+        Returns
+        -------
+        BlobDeletionTaskStatus
+            The status of the deletion task which can be used to wait for completion.
+
+        Raises
+        ------
+        DeletedObjectError
+            If this catalog object was already deleted.
+        UnsavedObjectError
+            If this catalog object is being deleted without having been saved.
+        ~descarteslabs.exceptions.ClientError or ~descarteslabs.exceptions.ServerError
+            :ref:`Spurious exception <network_exceptions>` that can occur during a
+            network request.
+        """
+        if self.state == DocumentState.UNSAVED:
+            raise UnsavedObjectError("You cannot delete an unsaved object.")
+
+        task_status = BlobDeletionTaskStatus.create(
+            ids=[self.id], raise_on_missing=True, client=self._client
+        )
+        self._deleted = True  # non-200 will raise an exception
+        return task_status
+
 
 class BlobCollection(Collection):
     _item_type = Blob
 
 
 # handle circular references
 Blob._collection_type = BlobCollection
+
+
+class BlobDeletionTaskStatus(TaskStatus):
+    """The asynchronous deletion task's status
+
+    Attributes
+    ----------
+    id : str
+        The id of the object for which this task is running.
+    status : TaskState
+        The state of the task as explained in `TaskState`.
+    start_datetime : datetime
+        The date and time at which the task started running.
+    duration_in_seconds : float
+        The duration of the task.
+    objects_deleted : int
+        The number of objects (a combination of bands or images) that were deleted.
+    errors : list
+        In case the status is ``FAILED`` this will contain a list of errors
+        that were encountered.  In all other states this will not be set.
+    ids : list
+        The ids of the objects that were deleted.
+    """
+
+    _task_name = "delete task"
+    _url = "/storage/delete/{}"
+
+    def __init__(self, objects_deleted=None, ids=None, **kwargs):
+        super(BlobDeletionTaskStatus, self).__init__(**kwargs)
+        self.objects_deleted = objects_deleted
+        self.ids = ids
+
+    @classmethod
+    def create(cls, ids, raise_on_missing, client):
+        # TaskStatus objects are not catalog objects so we need to do this manually
+        response = client.session.post(
+            "/storage/delete",
+            json={
+                "data": {
+                    "attributes": {
+                        "ids": ids,
+                        "raise_on_missing": raise_on_missing,
+                    },
+                    "type": "storage_delete",
+                }
+            },
+        )
+
+        if response.status_code == 201:
+            data = response.json()["data"]
+            return BlobDeletionTaskStatus(
+                id=data["id"], _client=client, **data["attributes"]
+            )
+        else:
+            return None
+
+    def __repr__(self):
+        text = super(BlobDeletionTaskStatus, self).__repr__()
+
+        if self.objects_deleted:
+            text += "\n  - {:,} objects deleted".format(self.objects_deleted)
+
+        return text
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/blob_delete.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/blob_download.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .attributes import ListAttribute, TypedAttribute
+from .attributes import TypedAttribute
 from .catalog_base import CatalogObjectBase
 
 
-class BlobDelete(CatalogObjectBase):
-    """Internal class used to perform bulk deleting of blobs."""
+class BlobDownload(CatalogObjectBase):
+    """Internal class used to initiate a blob upload."""
 
-    _doc_type = "storage_delete"
-    _url = "/storage/delete"
+    _doc_type = "storage_download"
+    _url = "/storage/download"
     _no_inherit = True
 
-    ids = ListAttribute(
-        TypedAttribute(str),
-        mutable=False,
-        serializable=True,
-        doc="""list[str]: List of blob IDs to delete.""",
+    resumable_url = TypedAttribute(
+        str,
+        readonly=True,
+        doc="""str: Download URL from which the client will transfer the file contents.
+
+        This field is for internal use by the client only.
+        """,
     )
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/blob_download.py` & `descarteslabs-3.1.0/descarteslabs/core/common/collection/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .attributes import TypedAttribute
-from .catalog_base import CatalogObjectBase
+from .collection import Collection, Eacher
 
-
-class BlobDownload(CatalogObjectBase):
-    """Internal class used to initiate a blob upload."""
-
-    _doc_type = "storage_download"
-    _url = "/storage/download"
-    _no_inherit = True
-
-    resumable_url = TypedAttribute(
-        str,
-        readonly=True,
-        doc="""str: Download URL from which the client will transfer the file contents.
-
-        This field is for internal use by the client only.
-        """,
-    )
+__all__ = ["Collection", "Eacher"]
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/blob_upload.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/blob_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/catalog_base.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/catalog_client.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/catalog_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/cli/bands.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/cli/bands.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/cli/blobs.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/cli/blobs.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/cli/products.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/cli/products.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/cli/tests/test_cli.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/cli/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/helpers.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/helpers.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/image.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/image.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/image_collection.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/image_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/image_types.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/image_types.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/image_upload.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/image_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/named_catalog_base.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/named_catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/product.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/product.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,34 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import time
-from concurrent.futures import TimeoutError
-
-from strenum import StrEnum
-
 from ..common.collection import Collection
 from ..common.property_filtering import Properties
 from .attributes import (
     BooleanAttribute,
     ListAttribute,
     Resolution,
     Timestamp,
     TypedAttribute,
 )
 from .catalog_base import (
     CatalogClient,
     CatalogObject,
-    _new_abstract_class,
     check_deleted,
 )
+from .task import TaskStatus
 
 
 properties = Properties()
 
 
 class Product(CatalogObject):
     """A raster product that connects band information to imagery.
@@ -480,149 +475,29 @@
     _item_type = Product
 
 
 # handle circular references
 Product._collection_type = ProductCollection
 
 
-class TaskState(StrEnum):
-    """The state of a task.
-
-    Attributes
-    ----------
-    NEVERRAN : enum
-        The operation was never invoked.
-    RUNNING : enum
-        The operation is in progress.
-    SUCCEEDED : enum
-        The operation was successfully completed.
-    FAILED : enum
-        The operation resulted in a failure and may not have been completed.
-    """
-
-    NEVERRAN = "NONE"  # The operation was never started
-    RUNNING = "RUNNING"
-    SUCCEEDED = "SUCCESS"
-    FAILED = "FAILURE"
-
-
-class TaskStatus(object):
-    """A base class for the status of asynchronous jobs."""
-
-    _TERMINAL_STATES = [TaskState.SUCCEEDED, TaskState.FAILED]
-    _POLLING_INTERVAL = 60
-
-    # The following 2 attributes must be set correctly in any derived class
-    _task_name = "task"  # The name of the task as shown in __repr__()
-    _url = "{}"  # The url for getting the status of the task with the `id` passed in
-
-    def __new__(cls, *args, **kwargs):
-        return _new_abstract_class(cls, TaskStatus)
-
-    def __init__(
-        self,
-        id=None,
-        status=None,
-        start_datetime=None,
-        duration_in_seconds=None,
-        errors=None,
-        _client=None,
-        **kwargs
-    ):
-        self.product_id = id
-        self.start_datetime = start_datetime
-        self.duration_in_seconds = duration_in_seconds
-        self.errors = errors
-        self._client = _client or CatalogClient.get_default_client()
-
-        try:
-            self.status = TaskState(status)
-        except ValueError:
-            pass
-
-    def __repr__(self):
-        status = self.status.value if self.status else "UNKNOWN"
-        text = ["{} {} status: {}".format(self.product_id, self._task_name, status)]
-        if self.start_datetime:
-            text.append("  - started: {}".format(self.start_datetime))
-
-        if self.duration_in_seconds:
-            text.append("  - took {:,.4f} seconds".format(self.duration_in_seconds))
-
-        if self.errors:
-            text.append("  - {} errors reported:".format(len(self.errors)))
-            for e in self.errors:
-                text.append("    - {}".format(e))
-        return "\n".join(text)
-
-    def reload(self):
-        """Update the task information.
-
-        Raises
-        ------
-        ~descarteslabs.exceptions.ClientError or ~descarteslabs.exceptions.ServerError
-            :ref:`Spurious exception <network_exceptions>` that can occur during a
-            network request.
-        """
-        r = self._client.session.get(self._url.format(self.product_id))
-        response = r.json()
-        new_values = response["data"]["attributes"]
-
-        self.status = TaskState(new_values.pop("status"))
-        for key, value in new_values.items():
-            setattr(self, key, value)
-
-    def wait_for_completion(self, timeout=None):
-        """Wait for the task to complete.
-
-        Parameters
-        ----------
-        timeout : int, optional
-            If specified, will wait up to specified number of seconds and will raise
-            a :py:exc:`concurrent.futures.TimeoutError` if the task has not completed.
-
-        Raises
-        ------
-        :py:exc:`concurrent.futures.TimeoutError`
-            If the specified timeout elapses and the task has not completed
-        """
-        if self.status in self._TERMINAL_STATES:
-            return
-
-        if timeout:
-            timeout = time.time() + timeout
-        while True:
-            self.reload()
-            if self.status in self._TERMINAL_STATES:
-                return
-            if timeout:
-                t = timeout - time.time()
-                if t <= 0:
-                    raise TimeoutError()
-                t = min(t, self._POLLING_INTERVAL)
-            else:
-                t = self._POLLING_INTERVAL
-            time.sleep(t)
-
-
 class DeletionTaskStatus(TaskStatus):
     """The asynchronous deletion task's status
 
     Attributes
     ----------
-    product_id : str
-        The id of the product for which this task is running.
+    id : str
+        The id of the object for which this task is running.
     status : TaskState
         The state of the task as explained in `TaskState`.
     start_datetime : datetime
         The date and time at which the task started running.
     duration_in_seconds : float
         The duration of the task.
     objects_deleted : int
-        The number of object (a combination of bands or images) that were deleted.
+        The number of objects (a combination of bands or images) that were deleted.
     errors: list
         In case the status is ``FAILED`` this will contain a list of errors
         that were encountered.  In all other states this will not be set.
     """
 
     _task_name = "delete task"
     _url = "/products/{}/delete_related_objects"
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/scaling.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/scaling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/search.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/base.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/mock_data.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_attributes.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_band.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_band.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_blob.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from datetime import datetime
 from tempfile import NamedTemporaryFile
 from unittest.mock import patch
 
 from descarteslabs.exceptions import BadRequestError
 from .base import ClientTestCase
 from ..attributes import AttributeValidationError
-from ..blob import Blob, BlobCollection, BlobSearch, StorageType
+from ..blob import Blob, BlobCollection, BlobDeletionTaskStatus, BlobSearch, StorageType
 from ..blob_upload import BlobUpload
 from ..catalog_base import DocumentState, DeletedObjectError
 from ...common.property_filtering import Properties
 
 
 def _namespace_id(namespace_id, client=None):
     return "descarteslabs:test-namespace"
@@ -623,61 +623,142 @@
         b = Blob(
             id="data/descarteslabs:test-namespace/test-blob",
             name="test-blob",
             client=self.client,
             _saved=True,
         )
         self.mock_response(
-            responses.DELETE,
+            responses.POST,
             {
+                "data": {
+                    "id": "123",
+                    "attributes": {
+                        "status": "RUNNING",
+                        "ids": [b.id],
+                    },
+                    "type": "storage_delete",
+                },
                 "meta": {"message": "Object successfully deleted"},
                 "jsonapi": {"version": "1.0"},
             },
+            status=201,
         )
 
-        b.delete()
+        task = b.delete()
+        assert isinstance(task, BlobDeletionTaskStatus)
         assert b.state == DocumentState.DELETED
 
     @responses.activate
+    def test_class_delete(self):
+        blob_id = "data/descarteslabs:test-namespace/test-blob"
+        self.mock_response(
+            responses.POST,
+            {
+                "data": {
+                    "id": "123",
+                    "attributes": {
+                        "status": "RUNNING",
+                        "ids": [blob_id],
+                    },
+                    "type": "storage_delete",
+                },
+                "jsonapi": {"version": "1.0"},
+            },
+            status=201,
+        )
+
+        task = Blob.delete(blob_id, client=self.client)
+        assert isinstance(task, BlobDeletionTaskStatus)
+        assert task.id == "123"
+        assert task.status == "RUNNING"
+        assert task.ids == [blob_id]
+
+        self.mock_response(
+            responses.GET,
+            {
+                "data": {
+                    "id": "123",
+                    "attributes": {
+                        "status": "SUCCESS",
+                        "objects_deleted": 1,
+                        "errors": None,
+                    },
+                    "type": "storage_delete",
+                },
+                "jsonapi": {"version": "1.0"},
+            },
+        )
+
+        task.wait_for_completion()
+        assert task.status == "SUCCESS"
+        assert task.objects_deleted == 1
+        assert task.ids == [blob_id]
+
+    @responses.activate
     def test_delete_non_existent(self):
         b = Blob(
             id="data/descarteslabs:test-namespace/nonexistent-blob",
             name="nonexistent-blob",
             client=self.client,
             _saved=True,
         )
-        self.mock_response(responses.DELETE, self.not_found_json, status=404)
+
+        self.mock_response(
+            responses.POST,
+            self.not_found_json,
+            status=404,
+        )
 
         with pytest.raises(DeletedObjectError):
             b.delete()
 
     @responses.activate
     def test_delete_many(self):
         self.mock_response(
             responses.POST,
             {
                 "data": {
                     "attributes": {
+                        "status": "RUNNING",
+                        "start_datetime": "2024-01-01T00:00:00Z",
                         "ids": [
                             "data/descarteslabs:test-namespace/test-blob-0",
                             "data/descarteslabs:test-namespace/test-blob-1",
-                        ]
+                        ],
                     },
-                    "id": "unique-test-id",
+                    "id": "123",
                     "type": "storage_delete",
                 }
             },
+            201,
+        )
+        self.mock_response(
+            responses.GET,
+            {
+                "data": {
+                    "attributes": {
+                        "status": "SUCCESS",
+                        "start_datetime": "2024-01-01T00:00:00Z",
+                        "duration_in_seconds": 1.0,
+                        "objects_deleted": 2,
+                    },
+                    "id": "123",
+                    "type": "storage_delete",
+                }
+            },
+            201,
         )
 
         deleted_blobs = Blob.delete_many(
             [
                 "data/descarteslabs:test-namespace/test-blob-0",
                 "data/descarteslabs:test/test-blob-1",
                 "data/descarteslabs:test/nonexistent-blob",
             ],
+            wait_for_completion=True,
             client=self.client,
         )
 
         assert "data/descarteslabs:test-namespace/test-blob-0" in deleted_blobs
         assert "data/descarteslabs:test-namespace/test-blob-1" in deleted_blobs
         assert "data/descarteslabs:test-namespace/nonexistent-blob" not in deleted_blobs
 
@@ -836,19 +917,14 @@
             client=self.client,
         )
 
         b.name = None
         with pytest.raises(ValueError):
             b.upload_data(data="")
 
-        b.name = "test-blob"
-        b._saved = False
-        with pytest.raises(DeletedObjectError):
-            b.upload_data(data="")
-
     @patch.object(Blob, "namespace_id", _namespace_id)
     def test_invalid_upload(self):
         b = Blob(
             name="test-blob",
             id="data/descarteslabs:test-namespace/test-blob",
             storage_type="data",
             storage_state="available",
@@ -862,16 +938,9 @@
         with NamedTemporaryFile(delete=False) as f1:
             try:
                 f1.close()
 
                 with pytest.raises(ValueError):
                     _ = b.upload(f1.name)
 
-                b.name = None
-                b._save = False
-
-                with pytest.raises(ValueError):
-                    with open(f1.name, "wb") as temp:
-                        _ = b.upload(temp)
-
             finally:
                 os.unlink(f1.name)
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_catalog_base.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_catalog_base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_download.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_filters.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_image.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_image_collection.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_image_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_image_upload.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_image_upload.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_product.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_product.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 from ..attributes import AttributeValidationError
 from ..catalog_base import DocumentState, DeletedObjectError
 from ..image_upload import ImageUploadStatus
 from ..product import (
     Product,
     Resolution,
-    TaskState,
-    TaskStatus,
     DeletionTaskStatus,
 )
+from ..task import TaskState, TaskStatus
 from .base import ClientTestCase
 
 
 class TestProduct(ClientTestCase):
     def test_constructor(self):
         p = Product(
             id="p1", name="Test Product", start_datetime="2019-01-01", tags=["tag"]
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_scaling.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_search.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/catalog/tests/test_summary.py` & `descarteslabs-3.1.0/descarteslabs/core/catalog/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 if sys.version_info < (3, 8):
     msg = "Python version {}.{} not supported by the descarteslabs client".format(
         sys.version_info.major, sys.version_info.minor
     )
     raise ImportError(msg)
 
+if sys.version_info < (3, 9):
+    msg = "Python version {}.{} is no longer supported. You may encounter unexpected errors.".format(
+        sys.version_info.major, sys.version_info.minor
+    )
+    warnings.warn(msg, FutureWarning)
+
 if sys.version_info >= (3, 12):
     msg = "Python version {}.{} is not supported yet. You may encounter unexpected errors.".format(
         sys.version_info.major, sys.version_info.minor
     )
     warnings.warn(msg, FutureWarning)
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/addons.py` & `descarteslabs-3.1.0/descarteslabs/core/client/addons.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/cli.py` & `descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/auth/cli/tests/test_cli.py` & `descarteslabs-3.1.0/descarteslabs/core/client/auth/cli/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/deprecation.py` & `descarteslabs-3.1.0/descarteslabs/core/client/deprecation.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/exceptions.py` & `descarteslabs-3.1.0/descarteslabs/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/scripts/__main__.py` & `descarteslabs-3.1.0/descarteslabs/core/client/scripts/__main__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/scripts/cli.py` & `descarteslabs-3.1.0/descarteslabs/core/client/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/scripts/lazy_group.py` & `descarteslabs-3.1.0/descarteslabs/core/client/scripts/lazy_group.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/scripts/tests/test_cli.py` & `descarteslabs-3.1.0/descarteslabs/core/client/scripts/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/geotiff_utils.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/geotiff_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/raster.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/e2e/iowa_geometry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/e2e/test_raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/test_geotiff_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/test_raster.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/raster/tests/test_raster_rasterio.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/service/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/service/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/service/api_service.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/service/api_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/service/service.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/service/service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/services/service/tests/test_service.py` & `descarteslabs-3.1.0/descarteslabs/core/client/services/service/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/tests/test_clear_client_state.py` & `descarteslabs-3.1.0/descarteslabs/core/client/tests/test_clear_client_state.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/tests/test_deprecation.py` & `descarteslabs-3.1.0/descarteslabs/core/client/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/client/version.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "3.0.5"
+
+class BoundGlobalError(NameError):
+    """
+    Raised when a global is referenced in a function where it won't be available
+    when executed remotely.
+    """
+
+    pass
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/attributes.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/document.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/document.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/search.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/sort.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/sort.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/tests/test_attributes.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/client/tests/test_search.py` & `descarteslabs-3.1.0/descarteslabs/core/common/client/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/collection/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/display/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .collection import Collection, Eacher
+from ._display import LayoutDirection, display, save_image
 
-__all__ = ["Collection", "Eacher"]
+__all__ = ["LayoutDirection", "display", "save_image"]
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/collection/collection.py` & `descarteslabs-3.1.0/descarteslabs/core/common/collection/collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/collection/tests/test_collection.py` & `descarteslabs-3.1.0/descarteslabs/core/common/collection/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/display/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/client/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ._display import LayoutDirection, display, save_image
-
-__all__ = ["LayoutDirection", "display", "save_image"]
+__version__ = "3.1.0"
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/display/_display.py` & `descarteslabs-3.1.0/descarteslabs/core/common/display/_display.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/display/tests/test_display.py` & `descarteslabs-3.1.0/descarteslabs/core/common/display/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/_tiling.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/_tiling.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/conversions.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/conversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/exceptions.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/rasterize.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/rasterize.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/tests/test_conversions.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/tests/test_dltiles.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/tests/test_dltiles.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/tile.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/tile.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/utils.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dltile/utm.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dltile/utm.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dotdict/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dotdict/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dotdict/dotdict.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dotdict/dotdict.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/dotdict/tests/test_dotdict.py` & `descarteslabs-3.1.0/descarteslabs/core/common/dotdict/tests/test_dotdict.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/geo/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/geo/geocontext.py` & `descarteslabs-3.1.0/descarteslabs/core/common/geo/geocontext.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/geo/tests/test_geocontext.py` & `descarteslabs-3.1.0/descarteslabs/core/common/geo/tests/test_geocontext.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/geo/tests/test_utils.py` & `descarteslabs-3.1.0/descarteslabs/core/common/geo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/geo/utils.py` & `descarteslabs-3.1.0/descarteslabs/core/common/geo/utils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/authorization.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/authorization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/proxy.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/proxy.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/retry.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/service.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/session.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/session.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_authorization.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_proxy.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_retry.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/http/tests/test_service.py` & `descarteslabs-3.1.0/descarteslabs/core/common/http/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/filtering.py` & `descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/filtering.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/property_filtering/tests/test_filtering.py` & `descarteslabs-3.1.0/descarteslabs/core/common/property_filtering/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/registry/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/registry/registry.py` & `descarteslabs-3.1.0/descarteslabs/core/common/registry/registry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/retry/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/retry/retry.py` & `descarteslabs-3.1.0/descarteslabs/core/common/retry/retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/retry/tests/test_retry.py` & `descarteslabs-3.1.0/descarteslabs/core/common/retry/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py` & `descarteslabs-3.1.0/descarteslabs/core/common/shapely_support/tests/test_shapely_support.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/threading/local.py` & `descarteslabs-3.1.0/descarteslabs/core/common/threading/local.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/threading/tests/test_local.py` & `descarteslabs-3.1.0/descarteslabs/core/common/threading/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/common/vector/models.py` & `descarteslabs-3.1.0/descarteslabs/core/common/vector/models.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/__init__.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/compute_client.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/compute_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/exceptions.py` & `descarteslabs-3.1.0/descarteslabs/core/third_party/boltons/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from . import funcutils
 
-class BoundGlobalError(NameError):
-    """
-    Raised when a global is referenced in a function where it won't be available
-    when executed remotely.
-    """
-
-    pass
+__all__ = ["funcutils"]
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/function.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/function.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/job.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/job.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/job_statistics.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/job_statistics.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/result.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/result.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/tests/base.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/tests/base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/tests/test_function.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/compute/tests/test_job.py` & `descarteslabs-3.1.0/descarteslabs/core/compute/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/third_party/boltons/__init__.py` & `descarteslabs-3.1.0/descarteslabs/vector/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import funcutils
-
-__all__ = ["funcutils"]
+from descarteslabs.core.vector import *  # noqa F401 F403
```

### Comparing `descarteslabs-3.0.5/descarteslabs/core/third_party/boltons/funcutils.py` & `descarteslabs-3.1.0/descarteslabs/core/third_party/boltons/funcutils.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/features.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/features.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/layers.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/layers.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/products.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/products.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/tests/base.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/tests/base.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_features.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_products.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_products.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_tiles.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_tiles.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/tests/test_vector.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/tiles.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/tiles.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/util.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/util.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/vector.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/vector.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/core/vector/vector_client.py` & `descarteslabs-3.1.0/descarteslabs/core/vector/vector_client.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/exceptions.py` & `descarteslabs-3.1.0/descarteslabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs/geo/__init__.py` & `descarteslabs-3.1.0/descarteslabs/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `descarteslabs-3.0.5/descarteslabs.egg-info/PKG-INFO` & `descarteslabs-3.1.0/descarteslabs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: descarteslabs
-Version: 3.0.5
+Version: 3.1.0
 Summary: Descartes Labs Python Client
 Home-page: https://github.com/descarteslabs/descarteslabs-python
 Author: Descartes Labs
 Author-email: hello@descarteslabs.com
 License: Apache 2.0
-Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v3.0.5.tar.gz
+Download-URL: https://github.com/descarteslabs/descarteslabs-python/archive/v3.1.0.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: ~=3.8
+Requires-Python: ~=3.9
 Provides-Extra: complete
 Provides-Extra: tests
 Provides-Extra: visualization
 License-File: LICENSE
 
 .. code-block:: bash
```

### Comparing `descarteslabs-3.0.5/descarteslabs.egg-info/SOURCES.txt` & `descarteslabs-3.1.0/descarteslabs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 descarteslabs/config/tests/__init__.py
 descarteslabs/config/tests/test_config.py
 descarteslabs/core/__init__.py
 descarteslabs/core/catalog/__init__.py
 descarteslabs/core/catalog/attributes.py
 descarteslabs/core/catalog/band.py
 descarteslabs/core/catalog/blob.py
-descarteslabs/core/catalog/blob_delete.py
 descarteslabs/core/catalog/blob_download.py
 descarteslabs/core/catalog/blob_upload.py
 descarteslabs/core/catalog/catalog_base.py
 descarteslabs/core/catalog/catalog_client.py
 descarteslabs/core/catalog/helpers.py
 descarteslabs/core/catalog/image.py
 descarteslabs/core/catalog/image_collection.py
 descarteslabs/core/catalog/image_types.py
 descarteslabs/core/catalog/image_upload.py
 descarteslabs/core/catalog/named_catalog_base.py
 descarteslabs/core/catalog/product.py
 descarteslabs/core/catalog/scaling.py
 descarteslabs/core/catalog/search.py
+descarteslabs/core/catalog/task.py
 descarteslabs/core/catalog/cli/__init__.py
 descarteslabs/core/catalog/cli/bands.py
 descarteslabs/core/catalog/cli/blobs.py
 descarteslabs/core/catalog/cli/cli.py
 descarteslabs/core/catalog/cli/products.py
 descarteslabs/core/catalog/cli/utils.py
 descarteslabs/core/catalog/cli/tests/__init__.py
```

### Comparing `descarteslabs-3.0.5/descarteslabs.egg-info/requires.txt` & `descarteslabs-3.1.0/descarteslabs.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 affine>=2.2.2
 blosc>=1.10.6
 cachetools>=3.1.1
 dill>=0.3.6
 dynaconf>=3.1.11
 geojson>=2.5.0
 geopandas>=0.13.2
-imagecodecs>=2021.5.20
 lazy_object_proxy>=1.7.1
 mercantile>=1.1.3
 pyarrow>=14.0.1
 pydantic>=2.1.0
 pytz>=2021.1
 requests<3,>=2.31.0
 setuptools>=65.6.3
 shapely>=2.0.0
 strenum>=0.4.8
 tqdm>=4.32.1
 urllib3!=2.0.0,!=2.0.1,!=2.0.2,!=2.0.3,!=2.0.4,>=1.26.18
 
 [:python_version == "3.8"]
+imagecodecs<=2023.3.16,>=2021.6.8
 tifffile==2023.4.12
 
 [:python_version >= "3.11"]
 numpy>=1.23.2
 
 [:python_version >= "3.8" and python_version < "3.11"]
 numpy>=1.22.0
 
 [:python_version >= "3.9"]
+imagecodecs>=2023.3.16
 tifffile>=2023.9.26
 
 [complete]
 ipyleaflet>=0.17.2
 matplotlib>=3.1.2
 
 [tests]
```

### Comparing `descarteslabs-3.0.5/setup.py` & `descarteslabs-3.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         long_description="\n".join(DOCLINES[2:]),
         author="Descartes Labs",
         author_email="hello@descarteslabs.com",
         url="https://github.com/descarteslabs/descarteslabs-python",
         classifiers=[
             "Programming Language :: Python",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
         license="Apache 2.0",
         download_url=(
             "https://github.com/descarteslabs/descarteslabs-python/archive/v{}.tar.gz".format(
@@ -87,24 +86,25 @@
         },
         include_package_data=True,
         entry_points={
             "console_scripts": [
                 "descarteslabs = descarteslabs.core.client.scripts.__main__:main"
             ]
         },
-        python_requires="~=3.8",
+        python_requires="~=3.9",
         install_requires=[
             "affine>=2.2.2",
             "blosc>=1.10.6",
             "cachetools>=3.1.1",
             "dill>=0.3.6",
             "dynaconf>=3.1.11",
             "geojson>=2.5.0",
             "geopandas>=0.13.2",
-            "imagecodecs>=2021.5.20",
+            "imagecodecs>=2021.6.8,<=2023.3.16;python_version=='3.8'",
+            "imagecodecs>=2023.3.16;python_version>='3.9'",
             "lazy_object_proxy>=1.7.1",
             "mercantile>=1.1.3",
             "numpy>=1.22.0;python_version>='3.8' and python_version<'3.11'",
             "numpy>=1.23.2;python_version>='3.11'",
             "Pillow>=9.2.0",
             "pyarrow>=14.0.1",
             "pydantic>=2.1.0",
```


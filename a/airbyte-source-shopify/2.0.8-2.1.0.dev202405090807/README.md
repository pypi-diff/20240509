# Comparing `tmp/airbyte_source_shopify-2.0.8.tar.gz` & `tmp/airbyte_source_shopify-2.1.0.dev202405090807.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.8.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.1.0.dev202405090807.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.8.tar` & `airbyte_source_shopify-2.1.0.dev202405090807.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0     4519 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/README.md
--rw-r--r--   0        0        0      800 2024-05-02 15:40:09.627828 airbyte_source_shopify-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/run.py
--rw-r--r--   0        0        0    28417 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     2548 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     2135 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     2151 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0     1889 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0     1173 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     2162 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     3100 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     2628 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      986 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0    10233 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0     1621 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0     1775 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    24211 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     9939 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    23930 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     2042 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0     1114 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     2806 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0     1919 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0     1881 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0     1925 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0     1957 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0     2008 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0     1800 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0     1874 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0     1985 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0     1782 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0     1919 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0     2078 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0     1873 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0     1985 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    26296 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0     1549 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0   103922 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     2093 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     7004 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0     1760 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     4650 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0    13110 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     3598 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     8137 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0     2009 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0     2006 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     6603 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    19793 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    56188 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     1734 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/retry.py
--rw-r--r--   0        0        0      328 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/status.py
--rw-r--r--   0        0        0     3629 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/spec.json
--rw-r--r--   0        0        0    37206 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11968 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/transform.py
--rw-r--r--   0        0        0    13468 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/utils.py
--rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     4529 2024-05-09 08:01:04.344695 airbyte_source_shopify-2.1.0.dev202405090807/README.md
+-rw-r--r--   0        0        0      816 2024-05-09 08:07:22.911137 airbyte_source_shopify-2.1.0.dev202405090807/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2162 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1114 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0     1549 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4886 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    13110 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/scopes.py
+-rw-r--r--   0        0        0        0 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/__init__.py
+-rw-r--r--   0        0        0     1813 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    20409 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    74083 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     1727 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/retry.py
+-rw-r--r--   0        0        0      328 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/status.py
+-rw-r--r--   0        0        0     3629 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-05-09 08:01:04.356695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/spec.json
+-rw-r--r--   0        0        0    37215 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11754 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/transform.py
+-rw-r--r--   0        0        0    13468 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/utils.py
+-rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.0.dev202405090807/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.8/README.md` & `airbyte_source_shopify-2.1.0.dev202405090807/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Shopify source connector
 
-
 This is the repository for the Shopify source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/shopify).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/shopify)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_shopify/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-shopify spec
 poetry run source-shopify check --config secrets/config.json
 poetry run source-shopify discover --config secrets/config.json
 poetry run source-shopify read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-shopify build
 ```
 
 An image will be available on your host with the tag `airbyte/source-shopify:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-shopify:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-shopify:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-shopify:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-shopify:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-shopify test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-shopify test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/shopify.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_shopify-2.0.8/pyproject.toml` & `airbyte_source_shopify-2.1.0.dev202405090807/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.8"
+version = "2.1.0.dev202405090807"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/__init__.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/auth.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_saved_search.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_saved_search.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_variants.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999758873456791%*

 * *Differences: {"'properties'": "{'presentment_prices': {'items': {'properties': {'compare_at_price': {'type': "*

 * *                 "{insert: [(1, 'object')], delete: [1]}, 'properties': OrderedDict([('amount', "*

 * *                 "OrderedDict([('description', 'The amount of the price'), ('type', ['null', "*

 * *                 "'number'])])), ('currency_code', OrderedDict([('description', 'The currency code "*

 * *                 "of the price'), ('type', ['null', 'string'])]))]), delete: ['description']}}}}}"}*

```diff
@@ -122,18 +122,33 @@
             ]
         },
         "presentment_prices": {
             "description": "The prices of the variant for presentation in different currencies",
             "items": {
                 "properties": {
                     "compare_at_price": {
-                        "description": "The original price of the variant in a different currency before any discount",
+                        "properties": {
+                            "amount": {
+                                "description": "The amount of the price",
+                                "type": [
+                                    "null",
+                                    "number"
+                                ]
+                            },
+                            "currency_code": {
+                                "description": "The currency code of the price",
+                                "type": [
+                                    "null",
+                                    "string"
+                                ]
+                            }
+                        },
                         "type": [
                             "null",
-                            "number"
+                            "object"
                         ]
                     },
                     "price": {
                         "description": "The price of the variant in a different currency",
                         "properties": {
                             "amount": {
                                 "description": "The amount of the price",
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/scopes.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
         def __init__(self, message: str, **kwargs) -> None:
             super().__init__(internal_message=message, failure_type=self.failure_type, **kwargs)
 
     class BulkJobError(BaseBulkException):
         """Raised when there are BULK Job Errors in response"""
 
-    class BulkJobUnknownError(BaseBulkException):
-        """Raised when BULK Job has FAILED with Unknown status"""
+    class BulkJobNonHandableError(BaseBulkException):
+        """Raised when there are non-actionable BULK Job Errors in response"""
+
+        failure_type: FailureType = FailureType.system_error
 
     class BulkJobBadResponse(BaseBulkException):
         """Raised when the requests.Response object could not be parsed"""
 
     class BulkJobResultUrlError(BaseBulkException):
         """Raised when BULK Job has ACCESS_DENIED status"""
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     _job_check_interval: Final[int] = 3
 
     # 0.1 ~= P2H, default value, lower boundary for slice size
     _job_size_min: Final[float] = 0.1
     # P365D, upper boundary for slice size
     _job_size_max: Final[float] = 365.0
     # dynamically adjusted slice interval
-    _job_size: float = field(init=False, default=0.0)
+    job_size: float = field(init=False, default=0.0)
     # expand slice factor
     _job_size_expand_factor: int = field(init=False, default=2)
     # reduce slice factor
     _job_size_reduce_factor: int = field(init=False, default=2)
     # whether or not the slicer should revert the previous start value
     _job_should_revert_slice: bool = field(init=False, default=False)
 
@@ -134,18 +134,18 @@
                 self._job_should_revert_slice = True
                 return True
         # reset slicer to normal mode
         self._job_should_revert_slice = False
         return False
 
     def _expand_job_size(self) -> None:
-        self._job_size += self._job_size_adjusted_expand_factor
+        self.job_size += self._job_size_adjusted_expand_factor
 
     def _reduce_job_size(self) -> None:
-        self._job_size /= self._job_size_adjusted_reduce_factor
+        self.job_size /= self._job_size_adjusted_reduce_factor
 
     def _save_latest_request(self, response: requests.Response) -> None:
         self._request = response.request
 
     def _job_size_reduce_next(self) -> None:
         # revert the flag
         self._job_should_revert_slice = False
@@ -158,15 +158,15 @@
             if job_current_elapsed_time < 1 or job_current_elapsed_time < self._job_last_elapsed_time:
                 self._expand_job_size()
             elif job_current_elapsed_time > self._job_last_elapsed_time < self._job_max_elapsed_time:
                 pass
             # set the last job time
             self._job_last_elapsed_time = job_current_elapsed_time
             # check the job size slice interval are acceptable
-            self._job_size = max(self._job_size_min, min(self._job_size, self._job_size_max))
+            self.job_size = max(self._job_size_min, min(self.job_size, self._job_size_max))
 
     def __reset_state(self) -> None:
         # reset the job state to default
         self._job_state = None
         # reset the filename to default
         self._job_result_filename = None
         # setting self-cancelation to default
@@ -278,40 +278,64 @@
 
     def _on_access_denied_job(self, **kwagrs) -> AirbyteTracedException:
         raise ShopifyBulkExceptions.BulkJobAccessDenied(
             f"The BULK Job: `{self._job_id}` exited with {self._job_state}, please check your PERMISSION to fetch the data for this stream.",
         )
 
     def _on_job_with_errors(self, errors: List[Mapping[str, Any]]) -> AirbyteTracedException:
-        raise ShopifyBulkExceptions.BulkJobUnknownError(
-            f"Could not validate the status of the BULK Job `{self._job_id}`. Errors: {errors}."
-        )
+        raise ShopifyBulkExceptions.BulkJobError(f"Could not validate the status of the BULK Job `{self._job_id}`. Errors: {errors}.")
 
-    def _job_check_for_errors(self, response: requests.Response) -> Optional[Iterable[Mapping[str, Any]]]:
-        try:
+    def _on_non_handable_job_error(self, errors: List[Mapping[str, Any]]) -> AirbyteTracedException:
+        raise ShopifyBulkExceptions.BulkJobNonHandableError(f"The Stream: `{self.stream_name}`, Non-handable error occured: {errors}")
 
-            return response.json().get("errors") or response.json().get("data", {}).get("bulkOperationRunQuery", {}).get("userErrors", [])
+    def _collect_bulk_errors(self, response: requests.Response) -> List[Optional[dict]]:
+        try:
+            server_errors = response.json().get("errors", [])
+            user_errors = response.json().get("data", {}).get("bulkOperationRunQuery", {}).get("userErrors", [])
+            errors = server_errors + user_errors
+            return errors
         except (Exception, JSONDecodeError) as e:
             raise ShopifyBulkExceptions.BulkJobBadResponse(
                 f"Couldn't check the `response` for `errors`, status: {response.status_code}, response: `{response.text}`. Trace: {repr(e)}."
             )
 
+    def _job_healthcheck(self, response: requests.Response) -> Optional[Exception]:
+        try:
+            # save the latest request to retry
+            self._save_latest_request(response)
+
+            # get the errors, if occured
+            errors = self._collect_bulk_errors(response)
+
+            # when the concurrent job takes place,
+            # another job could not be created
+            # we typically need to wait and retry, but no longer than 10 min.
+            if self._has_running_concurrent_job(errors):
+                return self._job_retry_on_concurrency()
+
+            # when the job was already created and the error appears in the middle
+            if self._job_state and errors:
+                self._on_job_with_errors(errors)
+
+            # when the job was not created because of some errors
+            if not self._job_state and errors:
+                self._on_non_handable_job_error(errors)
+
+        except (ShopifyBulkExceptions.BulkJobBadResponse, ShopifyBulkExceptions.BulkJobError) as e:
+            raise e
+
     def _job_send_state_request(self) -> requests.Response:
         with self.session as job_state_request:
             status_args = self._job_get_request_args(ShopifyBulkTemplates.status)
             self._request = requests.Request(**status_args, auth=self.session.auth).prepare()
             return job_state_request.send(self._request)
 
     def _job_track_running(self) -> None:
         job_state_response = self._job_send_state_request()
-        errors = self._job_check_for_errors(job_state_response)
-        if errors:
-            # the exception raised when there are job-related errors, and the Job cannot be run futher.
-            self._on_job_with_errors(errors)
-
+        self._job_healthcheck(job_state_response)
         self._job_update_state(job_state_response)
         self._job_state_to_fn_map.get(self._job_state)(response=job_state_response)
 
     def _has_running_concurrent_job(self, errors: Optional[Iterable[Mapping[str, Any]]] = None) -> bool:
         """
         When concurent BULK Job is already running for the same SHOP we receive:
         Error example:
@@ -344,66 +368,56 @@
     def _job_retry_concurrent(self) -> Optional[requests.Response]:
         self._concurrent_attempt += 1
         self.logger.warning(
             f"Stream: `{self.stream_name}`, the BULK concurrency limit has reached. Waiting {self._concurrent_interval} sec before retry, atttempt: {self._concurrent_attempt}.",
         )
         sleep(self._concurrent_interval)
         retried_response = self._job_retry_request()
-        return self._job_healthcheck(retried_response)
+        return self.job_process_created(retried_response)
 
     def _job_retry_on_concurrency(self) -> Optional[requests.Response]:
         if self._has_reached_max_concurrency():
             # indicate we're out of attempts to retry with job creation
             message = f"The BULK Job couldn't be created at this time, since another job is running."
             self.logger.error(message)
             # raise AibyteTracebackException with `INCOMPLETE` status
             raise ShopifyBulkExceptions.BulkJobConcurrentError(message)
         else:
             return self._job_retry_concurrent()
 
-    def _job_healthcheck(self, response: requests.Response) -> Optional[requests.Response]:
-        # save the latest request to retry
-        self._save_latest_request(response)
-        # check for query errors
-        errors = self._job_check_for_errors(response)
-        # when the concurrent job takes place, we typically need to wait and retry, but no longer than 10 min.
-        if self._has_running_concurrent_job(errors):
-            return self._job_retry_on_concurrency()
-
-        return response if not errors else None
-
     @bulk_retry_on_exception(logger)
     def _job_check_state(self) -> Optional[str]:
         while not self._job_completed():
             if self._job_canceled():
                 break
             else:
                 self._job_track_running()
 
     # external method to be used within other components
 
+    @bulk_retry_on_exception(logger)
     def job_process_created(self, response: requests.Response) -> None:
         """
         The Bulk Job with CREATED status, should be processed, before we move forward with Job Status Checks.
         """
-        response = self._job_healthcheck(response)
-        bulk_response = response.json().get("data", {}).get("bulkOperationRunQuery", {}).get("bulkOperation", {})
+        self._job_healthcheck(response)
+        bulk_response = response.json().get("data", {}).get("bulkOperationRunQuery", {}).get("bulkOperation", {}) if response else None
         if bulk_response and bulk_response.get("status") == ShopifyBulkJobStatus.CREATED.value:
             self._job_id = bulk_response.get("id")
             self._job_created_at = bulk_response.get("createdAt")
             self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self._job_id}` is {ShopifyBulkJobStatus.CREATED.value}")
 
     def job_size_normalize(self, start: datetime, end: datetime) -> datetime:
         # adjust slice size when it's bigger than the loop point when it should end,
         # to preserve correct job size adjustments when this is the only job we need to run, based on STATE provided
         requested_slice_size = (end - start).total_days()
-        self._job_size = requested_slice_size if requested_slice_size < self._job_size else self._job_size
+        self.job_size = requested_slice_size if requested_slice_size < self.job_size else self.job_size
 
     def get_adjusted_job_start(self, slice_start: datetime) -> datetime:
-        step = self._job_size if self._job_size else self._job_size_min
+        step = self.job_size if self.job_size else self._job_size_min
         return slice_start.add(days=step)
 
     def get_adjusted_job_end(self, slice_start: datetime, slice_end: datetime) -> datetime:
         if self._is_long_running_job:
             self._job_size_reduce_next()
             return slice_start
         else:
@@ -411,27 +425,27 @@
 
     @limiter.balance_rate_limit(api_type=ApiTypeEnum.graphql.value)
     def job_check_for_completion(self) -> Optional[str]:
         """
         This method checks the status for the `CREATED` Shopify BULK Job, using it's `ID`.
         The time spent for the Job execution is tracked to understand the effort.
         """
-        # track created job until it's COMPLETED
+
         job_started = time()
         try:
+            # track created job until it's COMPLETED
             self._job_check_state()
             return self._job_result_filename
         except (
-            ShopifyBulkExceptions.BulkJobCanceled,
             ShopifyBulkExceptions.BulkJobFailed,
             ShopifyBulkExceptions.BulkJobTimout,
             ShopifyBulkExceptions.BulkJobAccessDenied,
-            # this one is retryable, but stil needs to be raised,
-            # if the max attempts value is reached.
-            ShopifyBulkExceptions.BulkJobUnknownError,
+            # when the job is canceled by non-source actions,
+            # we should raise the system_error
+            ShopifyBulkExceptions.BulkJobCanceled,
         ) as bulk_job_error:
             raise bulk_job_error
         finally:
             job_current_elapsed_time = round((time() - job_started), 3)
             self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self._job_id}` time elapsed: {job_current_elapsed_time} sec.")
             # check whether or not we should expand or reduce the size of the slice
             self.__adjust_job_size(job_current_elapsed_time)
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         """
         Default query resolver from type(Operation) > type(str).
         Overide this method to build multiple queries in one, if needed.
         """
         # return the constructed query operation
         return Operation(type="", queries=[query]).render()
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components, default `as is`.
         """
         yield record
 
 
 class MetafieldType(Enum):
@@ -277,15 +277,15 @@
         metafield_node = self.get_edge_node("metafields", self.metafield_fields)
 
         if isinstance(self.type.value, list):
             return ["__typename", "id", self.get_edge_node(self.type.value[1], ["__typename", "id", metafield_node])]
         elif isinstance(self.type.value, str):
             return ["__typename", "id", metafield_node]
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         # resolve parent id from `str` to `int`
         record["owner_id"] = self.tools.resolve_str_id(record.get(BULK_PARENT_KEY))
         # add `owner_resource` field
         record["owner_resource"] = self.tools.camel_to_snake(record.get(BULK_PARENT_KEY, "").split("/")[3])
         # remove `__parentId` from record
         record.pop(BULK_PARENT_KEY, None)
         # convert dates from ISO-8601 to RFC-3339
@@ -666,15 +666,15 @@
 
     record_composition = {
         "new_record": "DiscountCodeNode",
         # each DiscountCodeNode has `DiscountRedeemCode`
         "record_components": ["DiscountRedeemCode"],
     }
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Optional[Iterable[MutableMapping[str, Any]]]:
         """
         Defines how to process collected components.
         """
 
         record_components = record.get("record_components", {})
         if record_components:
             discounts = record_components.get("DiscountRedeemCode", [])
@@ -747,15 +747,15 @@
 
     record_composition = {
         "new_record": "Collection",
         # each collection has `publications`
         "record_components": ["CollectionPublication"],
     }
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components.
         """
         record_components = record.get("record_components", {})
         if record_components:
             publications = record_components.get("CollectionPublication", [])
             if len(publications) > 0:
@@ -830,15 +830,17 @@
         "updatedAt",
     ]
 
     record_composition = {
         "new_record": "Customer",
     }
 
-    def set_default_address(self, record: MutableMapping[str, Any], address_record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def set_default_address(
+        self, record: MutableMapping[str, Any], address_record: MutableMapping[str, Any]
+    ) -> Iterable[MutableMapping[str, Any]]:
         default_address = record.get("defaultAddress", {})
         # the default_address could be literal `None`, additional check is required
         if default_address:
             if address_record.get("id") == record.get("defaultAddress", {}).get("id"):
                 address_record["default"] = True
         return address_record
 
@@ -920,15 +922,15 @@
         Field(name="requiresShipping"),
     ]
 
     record_composition = {
         "new_record": "InventoryItem",
     }
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components.
         """
 
         # resolve `cost` to root lvl as `number`
         unit_cost = record.get("unitCost", {})
         if unit_cost:
@@ -1002,15 +1004,15 @@
         return self.build(
             name=self.query_name,
             edges=self.query_nodes + inventory_levels,
             # passing more query args for `locations` query
             additional_query_args=self.locations_query_args,
         )
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components.
         """
 
         # resolve `inventory_item_id` to root lvl +  resolve to int
         record["inventory_item_id"] = self.tools.resolve_str_id(record.get("item", {}).get("inventory_item_id"))
         # add `location_id` from `__parentId`
@@ -1306,15 +1308,15 @@
         record.pop(BULK_PARENT_KEY)
         # resolve ids from `str` to `int`
         record["id"] = self.tools.resolve_str_id(record.get("id"))
         # field names to snake case
         record = self.tools.fields_names_to_snake_case(record)
         return record
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components.
         """
 
         record = self.process_fulfillment_order(record, self.shop_id)
         record_components = record.get("record_components", {})
         if record_components:
@@ -1498,7 +1500,479 @@
             transactions = record.get("transactions")
             if len(transactions) > 0:
                 for transaction in transactions:
                     # populate parent record keys
                     transaction["order_id"] = record.get("id")
                     transaction["currency"] = record.get("currency")
                     yield self.process_transaction(transaction)
+
+
+class Product(ShopifyBulkQuery):
+    """
+    {
+        products(query: "updated_at:>='2020-01-20T00:00:00+00:00' AND updated_at:<'2024-04-25T00:00:00+00:00'", sortKey:UPDATED_AT) {
+            edges {
+                node {
+                    __typename
+                    id
+                    publishedAt
+                    createdAt
+                    status
+                    vendor
+                    updatedAt
+                    bodyHtml
+                    productType
+                    tags
+                    options {
+                        __typename
+                        id
+                        values
+                        position
+                    }
+                    handle
+                    images {
+                        edges {
+                            node {
+                                __typename
+                                id
+                            }
+                        }
+
+                    }
+                    templateSuffix
+                    title
+                    variants {
+                        edges {
+                            node {
+                                __typename
+                                id
+                            }
+                        }
+                    }
+                }
+            }
+        }
+    }
+    """
+
+    query_name = "products"
+    sort_key = "UPDATED_AT"
+    # images property fields
+    images_fields: List[Field] = [Field(name="edges", fields=[Field(name="node", fields=["__typename", "id"])])]
+    # variants property fields, we re-use the same field names as for the `images` property
+    variants_fields: List[Field] = images_fields
+    # main query
+    query_nodes: List[Field] = [
+        "__typename",
+        "id",
+        "publishedAt",
+        "createdAt",
+        "status",
+        "vendor",
+        "updatedAt",
+        "bodyHtml",
+        "productType",
+        "tags",
+        "handle",
+        "templateSuffix",
+        "title",
+        Field(name="options", fields=["id", "name", "values", "position"]),
+        Field(name="images", fields=images_fields),
+        Field(name="variants", fields=variants_fields),
+    ]
+
+    record_composition = {
+        "new_record": "Product",
+        # each product could have `Image` and `ProductVariant` associated with the product
+        "record_components": ["Image", "ProductVariant"],
+    }
+
+    def _process_component(self, entity: List[dict]) -> List[dict]:
+        for item in entity:
+            # remove the `__parentId` from the object
+            if BULK_PARENT_KEY in item:
+                item.pop(BULK_PARENT_KEY)
+            # resolve the id from string
+            item["id"] = self.tools.resolve_str_id(item.get("id"))
+        return entity
+
+    def _process_options(self, options: List[dict], product_id: Optional[int] = None) -> List[dict]:
+        for option in options:
+            # add product_id to each option
+            option["product_id"] = product_id if product_id else None
+        return options
+
+    def _unnest_tags(self, record: MutableMapping[str, Any]) -> str:
+        # we keep supporting 1 tag only, as it was for the REST stream,
+        # to avoid breaking change.
+        tags = record.get("tags", [])
+        return tags[0] if len(tags) > 0 else None
+
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
+        """
+        Defines how to process collected components.
+        """
+        # get the joined record components collected for the record
+        record_components = record.get("record_components", {})
+
+        # process record components
+        if record_components:
+            record["images"] = self._process_component(record_components.get("Image", []))
+            record["variants"] = self._process_component(record_components.get("ProductVariant", []))
+            record["options"] = self._process_component(record.get("options", []))
+            # add the product_id to the `options`
+            product_id = record.get("id")
+            record["options"] = self._process_options(record.get("options", []), product_id)
+            record.pop("record_components")
+        # unnest the `tags` (the list of 1)
+        record["tags"] = self._unnest_tags(record)
+        # convert dates from ISO-8601 to RFC-3339
+        record["published_at"] = self.tools.from_iso8601_to_rfc3339(record, "publishedAt")
+        record["updatedAt"] = self.tools.from_iso8601_to_rfc3339(record, "updatedAt")
+        record["createdAt"] = self.tools.from_iso8601_to_rfc3339(record, "createdAt")
+
+        yield record
+
+
+class ProductImage(ShopifyBulkQuery):
+    """
+    {
+        products(
+            query: "updated_at:>='2019-04-13T00:00:00+00:00' AND updated_at:<='2024-04-30T12:16:17.273363+00:00'"
+            sortKey: UPDATED_AT
+        ) {
+            edges {
+                node {
+                    __typename
+                    id
+                    # THE MEDIA NODE IS NEEDED TO PROVIDE THE CURSORS
+                    media {
+                        edges {
+                            node {
+                            ... on MediaImage {
+                                    __typename
+                                    createdAt
+                                    updatedAt
+                                    image {
+                                        url
+                                    }
+                                }
+                            }
+                        }
+                    }
+                    # THIS IS THE MAIN NODE WE WANT TO GET
+                    images {
+                        edges {
+                            node {
+                                __typename
+                                id
+                                height
+                                alt: altText
+                                src
+                                url
+                                width
+                            }
+                        }
+                    }
+                }
+            }
+        }
+    }
+    """
+
+    query_name = "products"
+    sort_key = "UPDATED_AT"
+
+    # images property fields
+    images_fields: List[Field] = [
+        Field(
+            name="edges",
+            fields=[
+                Field(
+                    name="node",
+                    fields=[
+                        "__typename",
+                        "id",
+                        "height",
+                        Field(name="altText", alias="alt"),
+                        "src",
+                        "url",
+                        "width",
+                    ],
+                )
+            ],
+        )
+    ]
+
+    # media fragment, contains the info about when the Image was created or updated.
+    media_fragment: List[InlineFragment] = [
+        InlineFragment(
+            type="MediaImage",
+            fields=[
+                "__typename",
+                "createdAt",
+                "updatedAt",
+                # fetch the `url` as the key for the later join
+                Field(name="image", fields=["url"]),
+            ],
+        ),
+    ]
+
+    # media property fields
+    media_fields: List[Field] = [Field(name="edges", fields=[Field(name="node", fields=media_fragment)])]
+
+    # main query
+    query_nodes: List[Field] = [
+        "__typename",
+        "id",
+        Field(name="media", fields=media_fields),
+        Field(name="images", fields=images_fields),
+    ]
+
+    record_composition = {
+        "new_record": "Product",
+        # each product could have `MediaImage` associated with the product,
+        # each product could have `Image` assiciated with the product and the related `MediaImage`,
+        # there could be multiple `MediaImage` and `Image` assigned to the product.
+        "record_components": ["MediaImage", "Image"],
+    }
+
+    def _process_component(self, entity: List[dict]) -> List[dict]:
+        for item in entity:
+            # remove the `__parentId` from the object
+            if BULK_PARENT_KEY in item:
+                item.pop(BULK_PARENT_KEY)
+            # resolve the id from string
+            item["admin_graphql_api_id"] = item.get("id")
+            item["id"] = self.tools.resolve_str_id(item.get("id"))
+        return entity
+
+    def _add_product_id(self, options: List[dict], product_id: Optional[int] = None) -> List[dict]:
+        for option in options:
+            # add product_id to each option
+            option["product_id"] = product_id if product_id else None
+        return options
+
+    def _merge_with_media(self, record_components: List[dict]) -> Optional[Iterable[MutableMapping[str, Any]]]:
+        media = record_components.get("MediaImage", [])
+        images = record_components.get("Image", [])
+
+        # Create a dictionary to map the 'url' key in images
+        url_map = {item["url"]: item for item in images}
+
+        # Merge images with data from media when 'image.url' matches 'url'
+        for item in media:
+            # remove the `__parentId` from Media
+            if BULK_PARENT_KEY in item:
+                item.pop(BULK_PARENT_KEY)
+
+            image_url = item.get("image", {}).get("url")
+            if image_url in url_map:
+                # Merge images into media
+                item.update(url_map.get(image_url))
+                # remove lefovers
+                item.pop("image", None)
+                item.pop("url", None)
+                # make the `alt` None, if it's an empty str, since server sends the "" instead of Null
+                alt = item.get("alt")
+                item["alt"] = None if not alt else alt
+
+        # return merged list of images
+        return media
+
+    def _convert_datetime_to_rfc3339(self, images: List[dict]) -> MutableMapping[str, Any]:
+        for image in images:
+            image["createdAt"] = self.tools.from_iso8601_to_rfc3339(image, "createdAt")
+            image["updatedAt"] = self.tools.from_iso8601_to_rfc3339(image, "updatedAt")
+        return images
+
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
+        """
+        Defines how to process collected components.
+        """
+        # get the joined record components collected for the record
+        record_components = record.get("record_components", {})
+
+        # process record components
+        if record_components:
+            record["images"] = self._process_component(record_components.get("Image", []))
+            # add the product_id to each `Image`
+            record["images"] = self._add_product_id(record.get("images", []), record.get("id"))
+            record["images"] = self._merge_with_media(record_components)
+            record.pop("record_components")
+            # produce images records
+            if len(record.get("images", [])) > 0:
+                # convert dates from ISO-8601 to RFC-3339
+                record["images"] = self._convert_datetime_to_rfc3339(record.get("images", []))
+                yield from record.get("images", [])
+
+
+class ProductVariant(ShopifyBulkQuery):
+    """
+    {
+        productVariants(
+            query: "updated_at:>='2019-04-13T00:00:00+00:00' AND updated_at:<='2024-04-30T12:16:17.273363+00:00'"
+            sortKey: UPDATED_AT
+        ) {
+            edges {
+                node {
+                    __typename
+                    id
+                    product {
+                        product_id: id
+                    }
+                    title
+                    price
+                    sku
+                    position
+                    inventoryPolicy
+                    compareAtPrice
+                    fulfillmentService {
+                        fulfillment_service: handle
+                    }
+                    inventoryManagement
+                    createdAt
+                    updatedAt
+                    taxable
+                    barcode
+                    grams: weight
+                    weight
+                    weightUnit
+                    inventoryItem {
+                        inventory_item_id: id
+                    }
+                    inventoryQuantity
+                    old_inventory_quantity: inventoryQuantity
+                    presentmentPrices {
+                        edges {
+                            node {
+                                __typename
+                                price {
+                                    amount
+                                    currencyCode
+                                }
+                                compareAtPrice {
+                                    amount
+                                    currencyCode
+                                }
+                            }
+                        }
+                    }
+                    requiresShipping
+                    image {
+                        image_id: id
+                    }
+                }
+            }
+        }
+    }
+    """
+
+    query_name = "productVariants"
+    sort_key = "ID"
+
+    prices_fields: List[str] = ["amount", "currencyCode"]
+    presentment_prices_fields: List[Field] = [
+        Field(
+            name="edges",
+            fields=[
+                Field(
+                    name="node",
+                    fields=["__typename", Field(name="price", fields=prices_fields), Field(name="compareAtPrice", fields=prices_fields)],
+                )
+            ],
+        )
+    ]
+
+    # main query
+    query_nodes: List[Field] = [
+        "__typename",
+        "id",
+        "title",
+        "price",
+        "sku",
+        "position",
+        "inventoryPolicy",
+        "compareAtPrice",
+        "inventoryManagement",
+        "createdAt",
+        "updatedAt",
+        "taxable",
+        "barcode",
+        "weight",
+        "weightUnit",
+        "inventoryQuantity",
+        "requiresShipping",
+        Field(name="weight", alias="grams"),
+        Field(name="image", fields=[Field(name="id", alias="image_id")]),
+        Field(name="inventoryQuantity", alias="old_inventory_quantity"),
+        Field(name="product", fields=[Field(name="id", alias="product_id")]),
+        Field(name="fulfillmentService", fields=[Field(name="handle", alias="fulfillment_service")]),
+        Field(name="inventoryItem", fields=[Field(name="id", alias="inventory_item_id")]),
+        Field(name="presentmentPrices", fields=presentment_prices_fields),
+    ]
+
+    record_composition = {
+        "new_record": "ProductVariant",
+        # each `ProductVariant` could have `ProductVariantPricePair` associated with the product variant.
+        "record_components": ["ProductVariantPricePair"],
+    }
+
+    def _process_presentment_prices(self, entity: List[dict]) -> List[dict]:
+        for item in entity:
+            # remove the `__parentId` from the object
+            if BULK_PARENT_KEY in item:
+                item.pop(BULK_PARENT_KEY)
+
+            # these objects could be literally `Null/None` from the response,
+            # this is treated like a real value, so we need to assigne the correct values instead
+            price: Optional[Mapping[str, Any]] = item.get("price", {})
+            if not price:
+                price = {}
+            # get the amount values
+            price_amount = price.get("amount") if price else None
+            # make the nested object's values up to the schema, (cast the `str` > `float`)
+            item["price"]["amount"] = float(price_amount) if price_amount else None
+            # convert field names to snake case
+            item["price"] = self.tools.fields_names_to_snake_case(item.get("price"))
+
+            compare_at_price: Optional[Mapping[str, Any]] = item.get("compareAtPrice", {})
+            if not compare_at_price:
+                compare_at_price = {}
+                # assign the correct value, if there is no object from response
+                item["compareAtPrice"] = compare_at_price
+            compare_at_price_amount = compare_at_price.get("amount") if compare_at_price else None
+            item["compareAtPrice"]["amount"] = float(compare_at_price_amount) if compare_at_price_amount else None
+            item["compare_at_price"] = self.tools.fields_names_to_snake_case(item["compareAtPrice"])
+            # remove leftovers
+            item.pop("compareAtPrice", None)
+
+        return entity
+
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
+        """
+        Defines how to process collected components.
+        """
+
+        # get the joined record components collected for the record
+        record_components = record.get("record_components", {})
+        # process record components
+        if record_components:
+            record["presentment_prices"] = self._process_presentment_prices(record_components.get("ProductVariantPricePair", []))
+            record.pop("record_components")
+
+        # unnest mandatory fields from their placeholders
+        record["product_id"] = self.tools.resolve_str_id(record.get("product", {}).get("product_id"))
+        record["fulfillment_service"] = record.get("fulfillmentService", {}).get("fulfillment_service")
+        record["inventory_item_id"] = self.tools.resolve_str_id(record.get("inventoryItem", {}).get("inventory_item_id"))
+        record["grams"] = int(record.get("grams", 0))
+        # cast the the `price` to number, could be literally `None`
+        price = record.get("price")
+        record["price"] = float(price) if price else None
+        # convert date-time cursors
+        record["createdAt"] = self.tools.from_iso8601_to_rfc3339(record, "createdAt")
+        record["updatedAt"] = self.tools.from_iso8601_to_rfc3339(record, "updatedAt")
+        # clean up the leftovers
+        record.pop("product", None)
+        record.pop("inventoryItem", None)
+
+        yield record
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/retry.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/retry.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from airbyte_cdk import AirbyteLogger
 
 from .exceptions import ShopifyBulkExceptions
 
 BULK_RETRY_ERRORS: Final[Tuple] = (
     ShopifyBulkExceptions.BulkJobBadResponse,
-    ShopifyBulkExceptions.BulkJobUnknownError,
+    ShopifyBulkExceptions.BulkJobError,
 )
 
 
 def bulk_retry_on_exception(logger: AirbyteLogger, more_exceptions: Optional[Tuple[Type[Exception], ...]] = None) -> Callable:
     """
     A decorator to retry a function when specified exceptions are raised.
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/source.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/spec.json` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/base_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,15 +744,15 @@
         if stream_state:
             return self.get_stream_state_value(stream_state)
         else:
             # for majority of cases we fallback to start_date, otherwise.
             return self.config.get("start_date")
 
     def emit_slice_message(self, slice_start: datetime, slice_end: datetime) -> None:
-        slice_size_message = f"Slice size: `P{round(self.job_manager._job_size, 1)}D`"
+        slice_size_message = f"Slice size: `P{round(self.job_manager.job_size, 1)}D`"
         self.logger.info(f"Stream: `{self.name}` requesting BULK Job for period: {slice_start} -- {slice_end}. {slice_size_message}")
 
     @stream_state_cache.cache_stream_state
     def stream_slices(self, stream_state: Optional[Mapping[str, Any]] = None, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
         if self.filter_field:
             state = self.get_state_value(stream_state)
             start = pdm.parse(state)
@@ -768,15 +768,15 @@
             # for the streams that don't support filtering
             yield {"query": self.query.get()}
 
     def process_bulk_results(
         self,
         response: requests.Response,
         stream_state: Optional[Mapping[str, Any]] = None,
-    ) -> Iterable[Mapping[str, Any]]:
+    ) -> Optional[Iterable[Mapping[str, Any]]]:
         # process the CREATED Job prior to other actions
         self.job_manager.job_process_created(response)
         # get results fetched from COMPLETED BULK Job
         filename = self.job_manager.job_check_for_completion()
         # the `filename` could be `None`, meaning there are no data available for the slice period.
         if filename:
             # add `shop_url` field to each record produced
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/streams.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     MetafieldCustomer,
     MetafieldDraftOrder,
     MetafieldLocation,
     MetafieldOrder,
     MetafieldProduct,
     MetafieldProductImage,
     MetafieldProductVariant,
+    Product,
+    ProductImage,
+    ProductVariant,
     Transaction,
 )
 from source_shopify.shopify_graphql.graphql import get_query_products
 from source_shopify.utils import ApiTypeEnum
 from source_shopify.utils import ShopifyRateLimiter as limiter
 
 from .base_streams import (
@@ -104,18 +107,16 @@
     data_field = "draft_orders"
 
 
 class MetafieldDraftOrders(IncrementalShopifyGraphQlBulkStream):
     bulk_query: MetafieldDraftOrder = MetafieldDraftOrder
 
 
-class Products(IncrementalShopifyStreamWithDeletedEvents):
-    use_cache = True
-    data_field = "products"
-    deleted_events_api_name = "Product"
+class Products(IncrementalShopifyGraphQlBulkStream):
+    bulk_query: Product = Product
 
 
 class ProductsGraphQl(IncrementalShopifyStream):
     filter_field = "updatedAt"
     cursor_field = "updatedAt"
     data_field = "graphql"
     http_method = "POST"
@@ -163,30 +164,24 @@
                 self.logger.warning(f"Unexpected error in `parse_ersponse`: {e}, the actual response data: {response.text}")
 
 
 class MetafieldProducts(IncrementalShopifyGraphQlBulkStream):
     bulk_query: MetafieldProduct = MetafieldProduct
 
 
-class ProductImages(IncrementalShopifyNestedStream):
-    parent_stream_class = Products
-    nested_entity = "images"
-    # add `product_id` to each nested subrecord
-    mutation_map = {"product_id": "id"}
+class ProductImages(IncrementalShopifyGraphQlBulkStream):
+    bulk_query: ProductImage = ProductImage
 
 
 class MetafieldProductImages(IncrementalShopifyGraphQlBulkStream):
     bulk_query: MetafieldProductImage = MetafieldProductImage
 
 
-class ProductVariants(IncrementalShopifyNestedStream):
-    parent_stream_class = Products
-    nested_entity = "variants"
-    # add `product_id` to each nested subrecord
-    mutation_map = {"product_id": "id"}
+class ProductVariants(IncrementalShopifyGraphQlBulkStream):
+    bulk_query: ProductVariant = ProductVariant
 
 
 class MetafieldProductVariants(IncrementalShopifyGraphQlBulkStream):
     bulk_query: MetafieldProductVariant = MetafieldProductVariant
 
 
 class AbandonedCheckouts(IncrementalShopifyStream):
```

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/transform.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/source_shopify/utils.py` & `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.8/PKG-INFO` & `airbyte_source_shopify-2.1.0.dev202405090807/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.8
+Version: 2.1.0.dev202405090807
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
@@ -17,96 +17,110 @@
 Requires-Dist: sgqlc (==16.3)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/shopify
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Shopify source connector
 
-
 This is the repository for the Shopify source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/shopify).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/shopify)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_shopify/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-shopify spec
 poetry run source-shopify check --config secrets/config.json
 poetry run source-shopify discover --config secrets/config.json
 poetry run source-shopify read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-shopify build
 ```
 
 An image will be available on your host with the tag `airbyte/source-shopify:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-shopify:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-shopify:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-shopify:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-shopify:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-shopify test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-shopify test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/shopify.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```


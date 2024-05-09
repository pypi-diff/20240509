# Comparing `tmp/airbyte_source_amazon_seller_partner-4.2.2.tar.gz` & `tmp/airbyte_source_amazon_seller_partner-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.2.tar", max compression
+gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.3.tar", max compression
```

## Comparing `airbyte_source_amazon_seller_partner-4.2.2.tar` & `airbyte_source_amazon_seller_partner-4.2.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4765 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/README.md
--rw-r--r--   0        0        0      899 2024-05-07 12:17:53.700421 airbyte_source_amazon_seller_partner-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     1191 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/__init__.py
--rw-r--r--   0        0        0      638 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/auth.py
--rw-r--r--   0        0        0     6322 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/config_migrations.py
--rw-r--r--   0        0        0     3387 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/constants.py
--rw-r--r--   0        0        0      479 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/run.py
--rw-r--r--   0        0        0     1291 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
--rw-r--r--   0        0        0     1221 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
--rw-r--r--   0        0        0     6635 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
--rw-r--r--   0        0        0     1441 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
--rw-r--r--   0        0        0     2173 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
--rw-r--r--   0        0        0     1729 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
--rw-r--r--   0        0        0     5029 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
--rw-r--r--   0        0        0     2159 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
--rw-r--r--   0        0        0     1613 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
--rw-r--r--   0        0        0     2036 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
--rw-r--r--   0        0        0     2446 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
--rw-r--r--   0        0        0     1802 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
--rw-r--r--   0        0        0    11885 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
--rw-r--r--   0        0        0     3678 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
--rw-r--r--   0        0        0     2965 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
--rw-r--r--   0        0        0     3066 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
--rw-r--r--   0        0        0     3349 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
--rw-r--r--   0        0        0     4645 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
--rw-r--r--   0        0        0     3699 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
--rw-r--r--   0        0        0     4684 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
--rw-r--r--   0        0        0     4819 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     4125 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
--rw-r--r--   0        0        0     3434 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
--rw-r--r--   0        0        0     4629 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
--rw-r--r--   0        0        0     2193 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
--rw-r--r--   0        0        0     2823 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
--rw-r--r--   0        0        0     1381 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
--rw-r--r--   0        0        0     6146 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
--rw-r--r--   0        0        0     3884 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
--rw-r--r--   0        0        0     6479 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
--rw-r--r--   0        0        0     6472 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
--rw-r--r--   0        0        0     3988 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
--rw-r--r--   0        0        0     8105 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
--rw-r--r--   0        0        0     4129 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
--rw-r--r--   0        0        0     4223 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0     1185 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
--rw-r--r--   0        0        0     2709 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
--rw-r--r--   0        0        0     5477 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
--rw-r--r--   0        0        0      387 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
--rw-r--r--   0        0        0      388 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
--rw-r--r--   0        0        0     4217 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
--rw-r--r--   0        0        0     1550 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
--rw-r--r--   0        0        0     1313 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
--rw-r--r--   0        0        0     2411 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
--rw-r--r--   0        0        0     1384 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0     4860 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     3786 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
--rw-r--r--   0        0        0     2970 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
--rw-r--r--   0        0        0    44785 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/ListFinancialEvents.json
--rw-r--r--   0        0        0    11058 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/OrderItems.json
--rw-r--r--   0        0        0     7150 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/Orders.json
--rw-r--r--   0        0        0     9967 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
--rw-r--r--   0        0        0    16089 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/VendorOrders.json
--rw-r--r--   0        0        0      605 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
--rw-r--r--   0        0        0    10019 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/source.py
--rw-r--r--   0        0        0     8913 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/spec.json
--rw-r--r--   0        0        0    56375 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/streams.py
--rw-r--r--   0        0        0      403 2024-05-07 10:12:33.000000 airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/utils.py
--rw-r--r--   0        0        0     5589 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4775 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/README.md
+-rw-r--r--   0        0        0      899 2024-05-09 12:13:16.822048 airbyte_source_amazon_seller_partner-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1191 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/auth.py
+-rw-r--r--   0        0        0     6322 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/config_migrations.py
+-rw-r--r--   0        0        0     3387 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/constants.py
+-rw-r--r--   0        0        0      479 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/run.py
+-rw-r--r--   0        0        0     1291 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     1221 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
+-rw-r--r--   0        0        0     6635 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
+-rw-r--r--   0        0        0     1441 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
+-rw-r--r--   0        0        0     2173 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
+-rw-r--r--   0        0        0     1729 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
+-rw-r--r--   0        0        0     5029 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
+-rw-r--r--   0        0        0     2159 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
+-rw-r--r--   0        0        0     1613 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
+-rw-r--r--   0        0        0     2036 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
+-rw-r--r--   0        0        0     2446 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
+-rw-r--r--   0        0        0     1802 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
+-rw-r--r--   0        0        0    11885 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
+-rw-r--r--   0        0        0     3678 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     2965 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
+-rw-r--r--   0        0        0     3066 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
+-rw-r--r--   0        0        0     3349 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
+-rw-r--r--   0        0        0     4645 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
+-rw-r--r--   0        0        0     3699 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     4684 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
+-rw-r--r--   0        0        0     4819 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     4125 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
+-rw-r--r--   0        0        0     3434 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     4629 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
+-rw-r--r--   0        0        0     2193 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
+-rw-r--r--   0        0        0     2823 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
+-rw-r--r--   0        0        0     1381 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
+-rw-r--r--   0        0        0     6146 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     3884 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
+-rw-r--r--   0        0        0     6479 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     6472 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
+-rw-r--r--   0        0        0     3988 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
+-rw-r--r--   0        0        0     8105 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     4129 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
+-rw-r--r--   0        0        0     4223 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     1185 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
+-rw-r--r--   0        0        0     2709 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
+-rw-r--r--   0        0        0     5477 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
+-rw-r--r--   0        0        0      387 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
+-rw-r--r--   0        0        0      388 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
+-rw-r--r--   0        0        0     4217 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     1550 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
+-rw-r--r--   0        0        0     1313 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     2411 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
+-rw-r--r--   0        0        0     1384 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     4860 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     3786 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
+-rw-r--r--   0        0        0     2970 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
+-rw-r--r--   0        0        0    44785 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEvents.json
+-rw-r--r--   0        0        0    11058 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/OrderItems.json
+-rw-r--r--   0        0        0     7150 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/Orders.json
+-rw-r--r--   0        0        0     9967 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
+-rw-r--r--   0        0        0    16089 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorOrders.json
+-rw-r--r--   0        0        0      605 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
+-rw-r--r--   0        0        0    10892 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/source.py
+-rw-r--r--   0        0        0     8488 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/spec.json
+-rw-r--r--   0        0        0    56375 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/streams.py
+-rw-r--r--   0        0        0      403 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/utils.py
+-rw-r--r--   0        0        0     5599 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.3/PKG-INFO
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/README.md` & `airbyte_source_amazon_seller_partner-4.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Amazon Seller Partner Source
 
-
 This is the repository for the Amazon Seller-Partner source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/amazon-seller-partner).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/amazon-seller-partner)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_amazon_seller_partner/spec.json` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-amazon-seller-partner spec
 poetry run source-amazon-seller-partner check --config secrets/config.json
 poetry run source-amazon-seller-partner discover --config secrets/config.json
 poetry run source-amazon-seller-partner read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-amazon-seller-partner build
 ```
 
 An image will be available on your host with the tag `airbyte/source-amazon-seller-partner:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-amazon-seller-partner:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-amazon-seller-partner:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-amazon-seller-partner:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-amazon-seller-partner:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-amazon-seller-partner test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-amazon-seller-partner test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/amazon-seller-partner.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/pyproject.toml` & `airbyte_source_amazon_seller_partner-4.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.2.2"
+version = "4.2.3"
 name = "airbyte-source-amazon-seller-partner"
 description = "Source implementation for Amazon Seller Partner."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/__init__.py` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/auth.py` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/config_migrations.py` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/constants.py` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/constants.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/ListFinancialEvents.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEvents.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/OrderItems.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/OrderItems.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/Orders.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/Orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/VendorOrders.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorOrders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/source.py` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
-
-from os import getenv
+from logging import Logger
 from typing import Any, List, Mapping, Optional, Tuple
 
 import pendulum
 from airbyte_cdk.logger import AirbyteLogger
 from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
-from airbyte_cdk.utils import AirbyteTracedException
+from airbyte_cdk.utils import AirbyteTracedException, is_cloud_environment
+from airbyte_protocol.models import ConnectorSpecification
 from requests import HTTPError
 from source_amazon_seller_partner.auth import AWSAuthenticator
 from source_amazon_seller_partner.constants import get_marketplaces
 from source_amazon_seller_partner.streams import (
     BrandAnalyticsMarketBasketReports,
     BrandAnalyticsRepeatPurchaseReports,
     BrandAnalyticsSearchTermsReports,
@@ -186,15 +186,15 @@
             FbaReimbursementsReports,
             VendorOrders,
             VendorForecastingFreshReport,
             VendorForecastingRetailReport,
         ]
 
         # TODO: Remove after Brand Analytics will be enabled in CLOUD: https://github.com/airbytehq/airbyte/issues/32353
-        if getenv("DEPLOYMENT_MODE", "").upper() != "CLOUD":
+        if not is_cloud_environment():
             brand_analytics_reports = [
                 BrandAnalyticsMarketBasketReports,
                 BrandAnalyticsSearchTermsReports,
                 BrandAnalyticsRepeatPurchaseReports,
                 SellerAnalyticsSalesAndTrafficReports,
                 VendorSalesReports,
                 VendorInventoryReports,
@@ -204,14 +204,33 @@
             ]
             stream_list += brand_analytics_reports
 
         for stream in stream_list:
             streams.append(stream(**stream_kwargs, report_options=self.get_stream_report_options_list(stream.name, config)))
         return streams
 
+    def spec(self, logger: Logger) -> ConnectorSpecification:
+        spec = super().spec(logger)
+        if not is_cloud_environment():
+            oss_only_streams = [
+                "GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT",
+                "GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT",
+                "GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT",
+                "GET_SALES_AND_TRAFFIC_REPORT",
+                "GET_VENDOR_SALES_REPORT",
+                "GET_VENDOR_INVENTORY_REPORT",
+                "GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT",
+                "GET_VENDOR_TRAFFIC_REPORT",
+            ]
+            spec.connectionSpecification["properties"]["report_options_list"]["items"]["properties"]["stream_name"]["enum"].extend(
+                oss_only_streams
+            )
+
+        return spec
+
     @staticmethod
     def validate_replication_dates(config: Mapping[str, Any]) -> None:
         if (
             "replication_start_date" in config
             and "replication_end_date" in config
             and config["replication_end_date"] < config["replication_start_date"]
         ):
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/spec.json` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/spec.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999596461777%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'report_options_list': {'items': {'properties': "*

 * *                              "{'stream_name': {'enum': {delete: [41, 40, 39, 38, 34, 5, 4, "*

 * *                              '3]}}}}}}}'}*

```diff
@@ -210,17 +210,14 @@
                             "type": "array"
                         },
                         "stream_name": {
                             "enum": [
                                 "GET_AFN_INVENTORY_DATA",
                                 "GET_AFN_INVENTORY_DATA_BY_COUNTRY",
                                 "GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL",
-                                "GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT",
-                                "GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT",
-                                "GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT",
                                 "GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA",
                                 "GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA",
                                 "GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA",
                                 "GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA",
                                 "GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA",
                                 "GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA",
                                 "GET_FBA_INVENTORY_PLANNING_DATA",
@@ -241,22 +238,17 @@
                                 "GET_MERCHANT_LISTINGS_ALL_DATA",
                                 "GET_MERCHANT_LISTINGS_DATA",
                                 "GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT",
                                 "GET_MERCHANT_LISTINGS_INACTIVE_DATA",
                                 "GET_MERCHANTS_LISTINGS_FYP_REPORT",
                                 "GET_ORDER_REPORT_DATA_SHIPPING",
                                 "GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT",
-                                "GET_SALES_AND_TRAFFIC_REPORT",
                                 "GET_SELLER_FEEDBACK_DATA",
                                 "GET_STRANDED_INVENTORY_UI_DATA",
                                 "GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE",
-                                "GET_VENDOR_INVENTORY_REPORT",
-                                "GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT",
-                                "GET_VENDOR_TRAFFIC_REPORT",
-                                "GET_VENDOR_SALES_REPORT",
                                 "GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL",
                                 "GET_XML_BROWSE_TREE_DATA"
                             ],
                             "order": 0,
                             "title": "Stream Name",
                             "type": "string"
                         }
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/source_amazon_seller_partner/streams.py` & `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.2/PKG-INFO` & `airbyte_source_amazon_seller_partner-4.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-amazon-seller-partner
-Version: 4.2.2
+Version: 4.2.3
 Summary: Source implementation for Amazon Seller Partner.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -17,96 +17,110 @@
 Requires-Dist: xmltodict (>=0.12,<1.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/amazon-seller-partner
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Amazon Seller Partner Source
 
-
 This is the repository for the Amazon Seller-Partner source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/amazon-seller-partner).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/amazon-seller-partner)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_amazon_seller_partner/spec.json` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-amazon-seller-partner spec
 poetry run source-amazon-seller-partner check --config secrets/config.json
 poetry run source-amazon-seller-partner discover --config secrets/config.json
 poetry run source-amazon-seller-partner read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-amazon-seller-partner build
 ```
 
 An image will be available on your host with the tag `airbyte/source-amazon-seller-partner:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-amazon-seller-partner:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-amazon-seller-partner:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-amazon-seller-partner:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-amazon-seller-partner:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-amazon-seller-partner test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-amazon-seller-partner test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/amazon-seller-partner.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```


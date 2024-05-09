# Comparing `tmp/rapyd_sdk-1.0.1.tar.gz` & `tmp/rapyd_sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyd_sdk-1.0.1.tar", last modified: Thu May  2 12:44:12 2024, max compression
+gzip compressed data, was "rapyd_sdk-1.0.5.tar", last modified: Thu May  9 09:45:40 2024, max compression
```

## Comparing `rapyd_sdk-1.0.1.tar` & `rapyd_sdk-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,313 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:44:12.737757 rapyd_sdk-1.0.1/
--rw-rw-rw-   0        0        0     1061 2024-05-01 09:31:52.000000 rapyd_sdk-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      384 2024-05-02 12:44:12.735741 rapyd_sdk-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-02 12:43:32.000000 rapyd_sdk-1.0.1/README.md
--rw-rw-rw-   0        0        0      392 2024-05-02 12:43:37.000000 rapyd_sdk-1.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-02 12:44:12.733373 rapyd_sdk-1.0.1/rapyd_sdk.egg-info/
--rw-rw-rw-   0        0        0      384 2024-05-02 12:44:12.000000 rapyd_sdk-1.0.1/rapyd_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-05-02 12:44:12.000000 rapyd_sdk-1.0.1/rapyd_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:44:12.000000 rapyd_sdk-1.0.1/rapyd_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-02 12:44:12.000000 rapyd_sdk-1.0.1/rapyd_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-02 12:44:12.000000 rapyd_sdk-1.0.1/rapyd_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 12:44:12.727373 rapyd_sdk-1.0.1/sdk/
--rw-rw-rw-   0        0        0        0 2024-05-02 12:36:58.000000 rapyd_sdk-1.0.1/sdk/__init__.py
--rw-rw-rw-   0        0        0      546 2024-05-02 12:37:43.000000 rapyd_sdk-1.0.1/sdk/main.py
--rw-rw-rw-   0        0        0       42 2024-05-02 12:44:12.737757 rapyd_sdk-1.0.1/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.904193 rapyd_sdk-1.0.5/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1043 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/LICENSE
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   159492 2024-05-09 09:45:40.904193 rapyd_sdk-1.0.5/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   159152 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/README.md
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      371 2024-05-09 09:45:34.000000 rapyd_sdk-1.0.5/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       38 2024-05-09 09:45:40.904193 rapyd_sdk-1.0.5/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.784192 rapyd_sdk-1.0.5/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.904193 rapyd_sdk-1.0.5/src/rapyd_sdk.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   159492 2024-05-09 09:45:40.000000 rapyd_sdk-1.0.5/src/rapyd_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13736 2024-05-09 09:45:40.000000 rapyd_sdk-1.0.5/src/rapyd_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-05-09 09:45:40.000000 rapyd_sdk-1.0.5/src/rapyd_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       50 2024-05-09 09:45:40.000000 rapyd_sdk-1.0.5/src/rapyd_sdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2024-05-09 09:45:40.000000 rapyd_sdk-1.0.5/src/rapyd_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.792192 rapyd_sdk-1.0.5/src/rapydsdk/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       67 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.792192 rapyd_sdk-1.0.5/src/rapydsdk/hooks/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/hooks/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4145 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/hooks/hook.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.888193 rapyd_sdk-1.0.5/src/rapydsdk/models/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1681 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Account.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      409 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ActivateCard200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      176 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ActivateCardRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1690 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Address.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1581 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/AddressRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      415 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/AllRefunds200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      486 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/AttemptItem.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7528 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Beneficiary.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1246 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/BinDetails.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      418 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CancelPayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      413 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CancelPayout200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      443 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CancelSubscription200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1198 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CardIssuing.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1681 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CardIssuingMasked.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3361 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CardTransaction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      325 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Category.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6088 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CheckoutPageResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1237 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ClientDetailsObject.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      516 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CloseIssuing200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      665 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Condition.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      414 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ConfirmPayout200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5938 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Contact.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2007 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ContactBusiness.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      688 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CountryObject.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2522 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Coupon.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      394 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateAddress200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1573 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateAddressRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      414 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateBeneficiary200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2644 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateBeneficiaryRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      389 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateCoupon200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5049 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateCouponRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      688 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateCustomer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      490 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateCustomerPaymentMethod200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      360 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateCustomerPaymentMethodRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1564 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateCustomerRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateEwalletContact200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1758 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateEwalletContactRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      473 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateHostedApplicationToken200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      769 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateHostedApplicationTokenRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1372 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateIssuing200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      649 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateIssuingRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      440 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateOrder200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2426 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateOrderRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      418 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreatePayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8121 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreatePaymentRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      413 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreatePayout200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10801 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreatePayoutRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      403 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreatePlan200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1166 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreatePlanRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      418 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateProduct200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1618 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateProductRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      389 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSender200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2278 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSenderRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      374 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSku200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2727 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSkuRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      443 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSubscription200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      463 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSubscriptionItem200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      550 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSubscriptionItemRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      728 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSubscriptionItemUsageRecord200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      416 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSubscriptionItemUsageRecordRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2046 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateSubscriptionRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      415 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateUser200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1060 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CreateUserRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      515 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CurrencyObject.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2091 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Customer.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2392 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CustomerDetailsPmt.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      730 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CustomerDiscount.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4171 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CustomerPaymentMethod.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1569 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/CustomerRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DailyRate.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      521 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteBeneficiary200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      510 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteCoupon200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      515 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteCustomer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      523 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteCustomerDiscount200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      528 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteCustomerPaymentMethod200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      518 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteEwalletContact200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      517 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteInvoice200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      515 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeletePayer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      514 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeletePlan200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      517 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteProduct200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      513 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteSku200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      530 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteSubscriptionDiscount200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      526 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteSubscriptionItem200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      285 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/DeleteUser200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4173 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Dispute.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      217 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/EWalletsStatus.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      197 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/EntityType.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      351 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/EntityTypeVerify.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2469 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Ewallet.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2726 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/EwalletTransaction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3342 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/EwalletTransactionDetails.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      452 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/FinalizeInvoice200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      398 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/FundsTransfer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      567 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/FundsTransferRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      232 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/FxFee.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      471 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateCardIssuingPage200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      436 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateCardIssuingPageRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      476 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateCardTokenizationPage200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2505 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateCardTokenizationPageRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      482 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateHostedPagePayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4834 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateHostedPagePaymentRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2918 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateIdvPage200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1240 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GenerateIdvPageRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      763 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetApplicationStatus200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1635 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetApplicationTypesByCountry200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      411 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetBeneficiary200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      685 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCardIssuingDetails200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      712 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCardIssuingList200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCardIssuingTransaction200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      467 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCardIssuingTransactions200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      445 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCountries200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      450 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCurrencies200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      487 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCustomerPaymentMethod200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      518 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetCustomerPaymentMethods200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetDailyRate200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      391 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetDispute200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      431 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetDisputesListByOrgId200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      398 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetEwalletContact200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1012 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetEwalletContactComplianceLevels200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      427 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetEwalletContacts200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3688 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetHostedApplicationByToken200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      477 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetHostedPagePayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      868 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetKycIdVerificationSupportedDocTypes200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      385 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetPayer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      549 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetPaymentMethodTypeRequiredFields200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      480 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetPaymentMethodsTypesByCountry200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      410 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetPayout200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      465 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetPayoutMethodTypes200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      496 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetPayoutMethodTypesDetails200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      415 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetProduct200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      424 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetProductsList200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      440 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetSubscription200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      460 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetSubscriptionDiscountById200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      448 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetSubscriptionList200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      412 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetUser200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      424 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetUserAccounts200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      572 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetUserTransactionDetails200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      610 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetUserTransactions200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      417 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetUsers200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      422 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetWebhookByToken200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      420 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/GetWebhooks200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6337 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/HostedPageResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      203 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/HostedPageStatus.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2191 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/InvoiceItem.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3593 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/InvoiceResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      673 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/IssueCard200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      592 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/IssueCardRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Limit.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      415 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListCoupon200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      425 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListCustomer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      453 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListInvoices200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      442 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListOrder200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      480 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListOrderReturn200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      421 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListPayments200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      416 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListPayouts200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      406 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListPlans200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      400 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListSku200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      465 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ListSubscriptionItem200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      414 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/MerchantCustomerSupport.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      407 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ModifyCard200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      243 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ModifyCardRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      313 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/NextAction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1362 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/OrderItemResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2449 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/OrderResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1372 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/OrderReturnedItemResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1571 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/OrderReturnedResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2058 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Outcome.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      447 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayInvoice200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      211 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayInvoiceRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      437 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayOrder200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      334 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayOrderRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8438 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Payment.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1218 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentAmountRangePerCurrency.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      702 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentFee.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3970 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentFields.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3937 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentMethodType.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      977 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentMethodTypeField.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1086 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentMethodTypeRequiredFields.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      307 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentParams.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      293 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PaymentStatus.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6940 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Payout.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1252 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayoutAmountRangePerCurrency.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      604 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayoutFees.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3744 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayoutMethodType.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5969 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayoutMethodTypeDetails.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      924 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayoutRequiredFields.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      355 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PayoutStatus.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      545 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PerformIdentityVerification200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1836 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/PerformIdentityVerificationRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4736 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Plan.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1934 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Product.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2717 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Refund.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      414 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RefundByToken200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1364 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RefundGroupPayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      260 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RefundGroupPaymentRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      427 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RemoveAccountLimit200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      316 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RemoveAccountLimitRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      425 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RequestTotalCreateRefund200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      658 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RequestTotalCreateRefundRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      425 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ResendWebhookByToken200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      396 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveAddress200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      391 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveCoupon200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      690 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveCustomer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      452 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveInvoice200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2202 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveIssuingByRapydToken200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      525 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveIssuingTransaction200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      442 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveOrder200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      480 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveOrderReturn200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      420 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrievePayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      405 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrievePlan200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      376 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveSku200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      465 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/RetrieveSubscriptionItem200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      473 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ReturnsOrder200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1101 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ReturnsOrderRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4810 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Sender.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      424 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SetAccountLimit200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      348 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SetAccountLimitRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      409 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SetFundsTransferResponse200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      280 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SetFundsTransferResponseRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2969 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SimulateCompleteBankAccountIssuingTransaction200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      344 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SimulateCompleteBankAccountIssuingTransactionRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      423 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SimulateCompletePayout200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      423 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SimulateCompleteRefund200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      189 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SimulateCompleteRefundRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2137 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Sku.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      481 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3408 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Subscription.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      671 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SubscriptionDiscount.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      598 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SubscriptionItem.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      552 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SubscriptionItems.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1125 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/SubscriptionRetryOptions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      310 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/TransactionFee.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1650 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Transfer.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      394 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateAddress200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      413 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateCardStatus200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      295 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateCardStatusRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      389 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateCoupon200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      688 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateCustomer200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      490 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateCustomerPaymentMethod200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateEwalletContact200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      294 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateEwalletStatus200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      450 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateInvoice200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      693 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateInvoiceRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      440 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateOrder200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      784 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateOrderRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      418 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatePayment200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      766 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatePaymentRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      413 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatePayout200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      260 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatePayoutRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      403 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatePlan200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      249 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatePlanRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      418 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateProduct200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1084 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateProductRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1871 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateReceivingCurrency200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1085 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateReceivingCurrencyRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      413 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateRefund200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      196 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateRefundRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      374 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateSku200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2834 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateSkuRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      443 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateSubscription200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      463 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateSubscriptionItem200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateSubscriptionItemRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1767 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdateSubscriptionRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      416 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatedUser200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      452 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UpdatedUserRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      743 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/UsageRecordSummaries200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      635 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ValidateBeneficiary200Response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2617 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/ValidateBeneficiaryRequest.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2306 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/VerifyHostedAppResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1698 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/VirtualAccountTransactionResponse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      823 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/Webhook.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    16849 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7812 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.888193 rapyd_sdk-1.0.5/src/rapydsdk/models/utils/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2519 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/models/utils/JsonMap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.896193 rapyd_sdk-1.0.5/src/rapydsdk/net/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/net/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      333 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/net/environment.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13556 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/net/http_client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1266 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/net/http_content_types.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2539 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/net/query_serializer.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1716 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/net/utils.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1893 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/sdk.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:40.900193 rapyd_sdk-1.0.5/src/rapydsdk/services/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        0 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1938 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/base.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   116239 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/collect.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    32244 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/disburse.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    31835 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/e_wallets.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9430 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/general_resources.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3767 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/hosted.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22332 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/issuing.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8771 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/services/verify.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      186 2024-05-09 09:45:08.000000 rapyd_sdk-1.0.5/src/rapydsdk/setup.py
```

### Comparing `rapyd_sdk-1.0.1/LICENSE` & `rapyd_sdk-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2024 
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
-DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
+Copyright (c) 2024 
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 OR OTHER DEALINGS IN THE SOFTWARE.
```


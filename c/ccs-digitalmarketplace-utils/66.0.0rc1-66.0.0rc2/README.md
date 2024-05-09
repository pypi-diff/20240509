# Comparing `tmp/ccs-digitalmarketplace-utils-66.0.0rc1.tar.gz` & `tmp/ccs-digitalmarketplace-utils-66.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-utils-66.0.0rc1.tar", last modified: Tue Feb 20 09:56:38 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-utils-66.0.0rc2.tar", last modified: Thu May  9 08:33:17 2024, max compression
```

## Comparing `ccs-digitalmarketplace-utils-66.0.0rc1.tar` & `ccs-digitalmarketplace-utils-66.0.0rc2.tar`

### file list

```diff
@@ -1,69 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.721275 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.725276 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/asset_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cloudfoundry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cookie_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/csv_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/direct_plus_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/dmp_so_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.725276 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/user_account_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/env_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.725276 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/jinja2_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/ods.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/proxy_fix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/repoutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/repoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/service_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.750834 ccs-digitalmarketplace-utils-66.0.0rc2/ccs_digitalmarketplace_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 08:33:17.000000 ccs-digitalmarketplace-utils-66.0.0rc2/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-09 08:33:17.000000 ccs-digitalmarketplace-utils-66.0.0rc2/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:33:17.000000 ccs-digitalmarketplace-utils-66.0.0rc2/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-09 08:33:17.000000 ccs-digitalmarketplace-utils-66.0.0rc2/ccs_digitalmarketplace_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 08:33:17.000000 ccs-digitalmarketplace-utils-66.0.0rc2/ccs_digitalmarketplace_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.758834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/asset_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/cloudfoundry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/compliance_communications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/cookie_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/csv_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/direct_plus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/dmp_so_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.758834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/dm_mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/dm_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/user_account_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/env_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.758834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/errors/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/errors/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/flask_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/jinja2_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/ods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/presenters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/presenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/presenters/compliance_communications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/presenters/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/proxy_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/repoutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/repoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/service_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/view_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/view_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/view_helpers/compliance_communications.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/view_helpers/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/view_helpers/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:33:17.762834 ccs-digitalmarketplace-utils-66.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-09 08:33:03.000000 ccs-digitalmarketplace-utils-66.0.0rc2/setup.py
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/LICENCE` & `ccs-digitalmarketplace-utils-66.0.0rc2/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/README.md` & `ccs-digitalmarketplace-utils-66.0.0rc2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Digital Marketplace utils
 =========================
 
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)
 
 ## What's in here?
 
 * Digital Marketplace API clients
 * Formatting utilities for Digital Marketplace
 * Digital Marketplace logging for Flask using JSON Logging
 * Utility functions/libraries for Amazon S3, Mailchimp, Notify, Cloudwatch
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/access_control.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/access_control.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/asset_fingerprint.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/asset_fingerprint.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/authentication.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/authentication.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cloudfoundry.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/config.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,20 @@
             elif isinstance(value, int):
                 app.config[key] = _convert_to_int_or_fail(key, os.environ[key])
             else:
                 app.config[key] = os.environ[key]
     app.config['DM_ENVIRONMENT'] = os.environ.get('DM_ENVIRONMENT',
                                                   'development')
 
-    # From Flask 2.2 onwards, ENV is no longer uses.
-    # To run in debug mode we need to pass the debug flag into the flask command to run the app
-    # See https://flask.palletsprojects.com/en/2.2.x/config/#debug-mode
+    # From Flask 1.0 onwards, ENV is set to either 'production' (default) or 'development'.
+    # If set as 'development' then debug mode will be enabled.
+    # If left as 'production' when running a local development server, it gives an unsettling warning message.
+    # See http://flask.pocoo.org/docs/1.0/config/#environment-and-debug-features
+    if app.config['DM_ENVIRONMENT'] == 'development':
+        app.config['ENV'] = 'development'
 
 
 def _convert_to_boolean_or_fail(key, value):
     result = convert_to_boolean(value)
     if not isinstance(result, bool):
         raise ValueError("{} must be boolean".format(key))
     return result
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cookie_probe.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/cookie_probe.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/csv_generator.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/csv_generator.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/dates.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/dates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from workdays import workday
 
 from .formats import dateformat, utctoshorttimelongdateformat
 
 
 def get_publishing_dates(brief):
     APPLICATION_OPEN_DAYS = {'1 week': 7, '2 weeks': 14}
@@ -41,15 +41,15 @@
 
 def _get_start_date_from_published_frontend_brief(brief):
     return datetime.strptime(brief['publishedAt'][0:10], '%Y-%m-%d') \
         .replace(hour=23, minute=59, second=59, microsecond=0)
 
 
 def _get_todays_date():
-    return datetime.utcnow().replace(hour=23, minute=59, second=59, microsecond=0)
+    return datetime.now(timezone.utc).replace(hour=23, minute=59, second=59, microsecond=0)
 
 
 def _get_length_of_brief(brief):
     return brief['requirementsLength'] if brief.get('requirementsLength') else '2 weeks'
 
 
 def update_framework_with_formatted_dates(framework):
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/deprecation.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/deprecation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from functools import wraps
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 from flask import current_app
 
 
 def deprecated(dies_at):
     """Mark a flask view as deprecated
 
     Usage:
     @deprecated(dies_at=datetime(2015, 8, 1))
     """
     def decorator(view):
         @wraps(view)
         def func(*args, **kwargs):
             message = "Calling deprecated view '{view_name}'. Dies in {time_left}."
-            time_left = dies_at - datetime.utcnow()
+            time_left = dies_at - datetime.now(timezone.utc)
             extra = {'view_name': view.__name__, 'time_left': time_left}
             if time_left < timedelta(days=7):
                 current_app.logger.error(message, extra=extra)
             else:
                 current_app.logger.warning(message, extra=extra)
             response = view(*args, **kwargs)
             response.headers['DM-Deprecated'] = "Dies in {}".format(time_left)
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/direct_plus_client.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/direct_plus_client.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/documents.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         ID_TO_FILE_NAME_SUFFIX[field],
         suffix,
         get_extension(filename)
     )
 
 
 def default_file_suffix():
-    return datetime.datetime.utcnow().strftime("%Y-%m-%d-%H%M")
+    return datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d-%H%M")
 
 
 def get_signed_url(bucket, path, base_url):
     url = bucket.get_signed_url(path)
     if url is not None:
         if base_url is not None:
             url = urlparse.urlparse(url)
@@ -329,15 +329,15 @@
         document_name
     )
 
 
 def generate_timestamped_document_upload_path(framework_slug, supplier_id, bucket_category, doc_name):
     """Generates a file path with a timestamp inserted before the file extension"""
     file_name, file_extension = os.path.splitext(doc_name)
-    timestamped_file_name = file_name + '-' + datetime.datetime.utcnow().strftime("%Y-%m-%d-%H%M%S")
+    timestamped_file_name = file_name + '-' + datetime.datetime.now(datetime.timezone.utc).strftime("%Y-%m-%d-%H%M%S")
     timestamped_doc_name = timestamped_file_name + file_extension
 
     return get_document_path(framework_slug, supplier_id, bucket_category, timestamped_doc_name)
 
 
 def degenerate_document_path_and_return_doc_name(document_path):
     """Takes a document path and returns just the generic document name
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_mailchimp.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/dm_mailchimp.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_notify.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/dm_notify.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/tokens.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 import struct
 from warnings import warn
 
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 from cryptography import fernet
 from flask import current_app
 
 from dmutils.formats import DATETIME_FORMAT
 from dmutils.email.helpers import hash_string
 
@@ -55,15 +55,15 @@
     decoded = base64.urlsafe_b64decode(ciphertext)
 
     try:
         epoch_timestamp = struct.unpack('>Q', decoded[1:9])[0]
     except struct.error as e:
         raise fernet.InvalidToken(e.message)
 
-    return datetime.utcfromtimestamp(epoch_timestamp)
+    return datetime.fromtimestamp(epoch_timestamp, timezone.utc)
 
 
 def decode_token(encrypted_data, secret_key, namespace, max_age_in_seconds=ONE_DAY_IN_SECONDS):
     """
     Decrypt data using a provided secret_key, namespace, and TTL (max_age_in_seconds).
 
     The process is as follows:
@@ -113,27 +113,27 @@
         current_app.logger.info("Error changing password: {error}", extra={'error': str(e)})
         return {'error': 'token_invalid'}
 
     user = data_api_client.get_user(decoded["user"])
     user_last_changed_password_at = datetime.strptime(
         user['users']['passwordChangedAt'],
         DATETIME_FORMAT
-    )
+    ).replace(tzinfo=timezone.utc)
 
     if not user["users"]["active"]:
         current_app.logger.info("Error changing password: target user is not active.")
         return {'error': 'user_inactive'}
 
     # Check if the token was created before the last password change
     # (allow 1 second leeway for reset tokens generated for the 'Your password was changed' email link)
     if token_timestamp + timedelta(seconds=1) < user_last_changed_password_at:
         current_app.logger.info("Error changing password: Token generated earlier than password was last changed.")
         return {'error': 'token_invalid'}
 
-    if token_timestamp > datetime.utcnow():
+    if token_timestamp > datetime.now(timezone.utc):
         current_app.logger.info("Error changing password: cannot use token generated in the future.")
         return {'error': 'token_invalid'}
 
     return {
         'user': user['users']['id'],
         'email': user['users']['emailAddress']
     }
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/user_account_email.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/email/user_account_email.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/env_helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/env_helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/api.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/errors/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     try:
         # initially we'll try and assume this is an HTTPException of some sort.  for the most part, the default
         # HTTPExceptions render themselves in the desired way if returned as a response. the only change we want to
         # make is to enclose the error description in json.
         response = e.get_response()
         response.set_data(json.dumps({"error": e.description}))
-        response.mimetype = current_app.json.mimetype
+        response.mimetype = current_app.config["JSONIFY_MIMETYPE"]
 
         return response
     except Exception:
         # either `e` wasn't an HTTPException or something went wrong in trying to jsonify it
         return jsonify(error="Internal error"), 500
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/frontend.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/errors/frontend.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/external.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/external.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 
 
 @external.route('/suppliers/supply')
 def become_a_supplier():
     raise NotImplementedError()
 
 
+@external.route('/suppliers/compliance-communication/<int:communication_id>')
+def supplier_view_compliance_communication(communication_id):
+    raise NotImplementedError()
+
+
 # Brief Responses frontend
 @external.route('/suppliers/opportunities/<brief_id>/responses/start')
 def start_brief_response(brief_id):
     raise NotImplementedError()
 
 
 @external.route('/suppliers/opportunities/<int:brief_id>/responses/result')
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/feature_flag.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/feature_flag.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/filters.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import unicode_literals
 
-from typing import Iterable, Any
+from typing import Iterable, Any, Optional
 
 import govuk_country_register
 import re
+from datetime import datetime
 from jinja2 import pass_eval_context
 from jinja2.nodes import EvalContext
 from markupsafe import Markup, escape
 
 
 def smartjoin(input: Iterable) -> str:
     list_to_join = list(input)
@@ -132,7 +133,15 @@
         return re.sub(
             r"country:(?P<country_code>[A-Z][A-Z])",
             replace_match_with_country_name,
             text
         )
     except TypeError:
         return text
+
+
+def parse_document_upload_time(document_name: str) -> Optional[datetime]:
+    match = re.search(r"(\d{4}-\d{2}-\d{2}-\d{2}\d{2})\..{2,4}$", document_name)
+    if match:
+        return datetime.strptime(match.group(1), "%Y-%m-%d-%H%M")
+
+    return None
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/flask.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask_init.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/flask_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     # Make filters accessible in templates.
     application.add_template_filter(filters.capitalize_first)
     application.add_template_filter(filters.format_links)
     application.add_template_filter(filters.nbsp)
     application.add_template_filter(filters.smartjoin)
     application.add_template_filter(filters.preserve_line_breaks)
     application.add_template_filter(filters.sub_country_codes)
+    application.add_template_filter(filters.parse_document_upload_time)
     # Make select formats available in templates.
     application.add_template_filter(formats.dateformat)
     application.add_template_filter(formats.datetimeformat)
     application.add_template_filter(formats.datetodatetimeformat)
     application.add_template_filter(formats.displaytimeformat)
     application.add_template_filter(formats.shortdateformat)
     application.add_template_filter(formats.timeformat)
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/formats.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/formats.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/errors.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/fields.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,17 +34,27 @@
     DMUnitInput,
 )
 
 from .filters import strip_whitespace
 from .validators import EmailValidator
 
 
-__all__ = ['DMBooleanField', 'DMDecimalField', 'DMHiddenField', 'DMIntegerField',
-           'DMRadioField', 'DMStringField', 'DMEmailField', 'DMStripWhitespaceStringField',
-           'DMDateField']
+__all__ = [
+    'DMBooleanField',
+    'DMDecimalField',
+    'DMHiddenField',
+    'DMIntegerField',
+    'DMRadioField',
+    'DMCheckboxesField',
+    'DMStringField',
+    'DMEmailField',
+    'DMStripWhitespaceStringField',
+    'DMDateField',
+    'DMFileField',
+]
 
 
 class DMBooleanField(DMFieldMixin, wtforms.fields.BooleanField):
     widget = DMCheckboxInput(hide_question=True)
 
     @property
     def href(self):
@@ -83,14 +93,18 @@
     pass
 
 
 class DMRadioField(DMSelectFieldMixin, DMFieldMixin, wtforms.fields.RadioField):
     widget = DMRadioInput()
 
 
+class DMCheckboxesField(DMSelectFieldMixin, DMFieldMixin, wtforms.fields.SelectMultipleField):
+    pass
+
+
 class DMStringField(DMFieldMixin, wtforms.fields.StringField):
     widget = DMTextInput()
 
 
 class DMStripWhitespaceStringField(DMFieldMixin, wtforms.fields.StringField):
     widget = DMTextInput()
 
@@ -245,7 +259,11 @@
         # year}.errors.  In the case where the validator chain hasn't added
         # errors to any of day month or year, we will add the errors to all the
         # fields so that all inputs get highlighted.
         if self.errors and not any((self.year.errors, self.month.errors, self.day.errors)):
             self.year.errors = self.errors
             self.month.errors = self.errors
             self.day.errors = self.errors
+
+
+class DMFileField(DMFieldMixin, wtforms.fields.FileField):
+    pass
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/mixins.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/validators.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/validators.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/widgets.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/jinja2_environment.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/jinja2_environment.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/logging.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/logging.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/ods.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/ods.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/proxy_fix.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/request_id.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/request_id.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/s3.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 default_region = "eu-west-2"
 
 
 class S3(object):
     def __init__(self, bucket_name, region_name=default_region, **kwargs):
         if flask.current_app:
             app = flask.current_app
-            if app.debug and app.config.get("DM_S3_ENDPOINT_URL"):
+            if app.env == "development" and app.config.get("DM_S3_ENDPOINT_URL"):
                 kwargs.setdefault("endpoint_url", app.config["DM_S3_ENDPOINT_URL"])
         self._resource = boto3.resource("s3", region_name=region_name, **kwargs)
         self._bucket = self._resource.Bucket(bucket_name)
 
     @property
     def bucket_name(self):
         return self._bucket.name
@@ -49,15 +49,15 @@
         :param timestamp:         Timestamp to set for this file rather than using utcnow
         :param download_filename: Suggested name for a browser to download, part of Content-Disposition header
         :param disposition_type:  Content-Disposition type - e.g. "attachment" or "inline"
 
         :return: S3 Key
         """
         path = self._normalize_path(path)
-        timestamp = timestamp or datetime.datetime.utcnow()
+        timestamp = timestamp or datetime.datetime.now(datetime.timezone.utc)
         filesize = get_file_size(file_)
 
         obj = self._bucket.Object(path)
         extra_kwargs = {}
         if download_filename:
             extra_kwargs["ContentDisposition"] = u'{}; filename="{}"'.format(
                 disposition_type,
@@ -136,38 +136,39 @@
         """
         path = self._normalize_path(path)
         if self.path_exists(path):
             # Because we are using cloudfront as a load balancer for the assets
             # the URL we generate needs to include the region.
             # However boto3 does not do this so we are having to make use of
             # the AWS CLI to create this URL.
-            if os.getenv("DM_ENVIRONMENT", None) == "native-aws":
-                result = subprocess.run(
-                    [
-                        'aws',
-                        's3',
-                        'presign',
-                        f's3://{self._bucket.name}/{path}',
-                        '--expires-in',
-                        str(expires_in)
-                    ],
-                    stdout=subprocess.PIPE,
-                    check=True,
-                )
-
-                return result.stdout.decode()
-            else:
-                return self._resource.meta.client.generate_presigned_url(
-                    "get_object",
-                    Params={
-                        "Bucket": self._bucket.name,
-                        "Key": path,
-                    },
-                    ExpiresIn=expires_in,
-                )
+            result = subprocess.run(
+                [
+                    'aws',
+                    's3',
+                    'presign',
+                    f's3://{self._bucket.name}/{path}',
+                    '--expires-in',
+                    str(expires_in)
+                ],
+                stdout=subprocess.PIPE,
+                check=True,
+            )
+
+            return result.stdout.decode()
+
+            # If we were not using cloudfront as the load balanacer then
+            # the following code would work
+            # return self._resource.meta.client.generate_presigned_url(
+            #     "get_object",
+            #     Params={
+            #         "Bucket": self._bucket.name,
+            #         "Key": path,
+            #     },
+            #     ExpiresIn=expires_in,
+            # )
 
     def _get_key(self, path):
         path = self._normalize_path(path)
         try:
             obj = self._bucket.Object(path)
             obj.load()
         except S3ResponseError:
```

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/service_attribute.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/service_attribute.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/session.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/session.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/status.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/status.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/timing.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/timing.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/urls.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/urls.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/user.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/user.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/views.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/dmutils/views.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-66.0.0rc1/setup.py` & `ccs-digitalmarketplace-utils-66.0.0rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,30 @@
     description='Common utils for Digital Marketplace apps.',
     long_description=__doc__,
     packages=find_packages(),
     package_data={'dmutils': ['py.typed']},
     include_package_data=True,
     install_requires=[
         'Flask-WTF>=1.2.1',
-        'Flask>=2.3,<3',
+        'Flask>=2.1,<2.2',
         'Flask-gzip>=0.2',
-        'Flask-Login>=0.6.3',
-        'Flask-Session<0.6.0,>=0.5.0',
+        'Flask-Login>=0.6.2',
+        'Flask-Session<0.5.0,>=0.4.1',
         'boto3<2,>=1.7.83',
         'contextlib2>=21.6.0',
         'cryptography>=41.0.4',
         'ccs-digitalmarketplace-apiclient>=25.0.0',
         'govuk-country-register>=0.5.0',
         'mailchimp3==3.0.21',
         'requests>=2.22.0,<3',
         'redis>=5.0.1',
         'fleep<1.1,>=1.0.1',
         'notifications-python-client>=8.1.0,<9.0.0',
         'odfpy>=1.4.1',
         'python-json-logger>=2.0.7,<3.0.0',
         'pytz',
         'unicodecsv>=0.14.1',
-        'werkzeug>=2.3,<3',
+        'werkzeug>=2.1,<2.2',
         'workdays>=1.4',
     ],
-    python_requires=">=3.9,<3.12",
+    python_requires=">=3.9,<3.13",
 )
```


# Comparing `tmp/zscaler_sdk_python-0.1.7.tar.gz` & `tmp/zscaler_sdk_python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_sdk_python-0.1.7.tar", max compression
+gzip compressed data, was "zscaler_sdk_python-0.1.8.tar", max compression
```

## Comparing `zscaler_sdk_python-0.1.7.tar` & `zscaler_sdk_python-0.1.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1113 2024-05-06 07:40:30.079598 zscaler_sdk_python-0.1.7/LICENSE.md
--rw-r--r--   0        0        0    15746 2024-05-06 07:40:30.079598 zscaler_sdk_python-0.1.7/README.md
--rw-r--r--   0        0        0     2292 2024-05-06 07:41:09.675720 zscaler_sdk_python-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1277 2024-05-06 07:41:09.679720 zscaler_sdk_python-0.1.7/zscaler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/__init__.py
--rw-r--r--   0        0        0     3195 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/cache.py
--rw-r--r--   0        0        0     1479 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/no_op_cache.py
--rw-r--r--   0        0        0     4967 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/cache/zscaler_cache.py
--rw-r--r--   0        0        0      738 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/constants.py
--rw-r--r--   0        0        0        0 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/__init__.py
--rw-r--r--   0        0        0      172 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/error.py
--rw-r--r--   0        0        0      638 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/http_error.py
--rw-r--r--   0        0        0      628 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/errors/zscaler_api_error.py
--rw-r--r--   0        0        0       63 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/exceptions/__init__.py
--rw-r--r--   0        0        0     2025 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/exceptions/exceptions.py
--rw-r--r--   0        0        0     2099 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/logger.py
--rw-r--r--   0        0        0        0 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0        0        0      639 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/user_agent.py
--rw-r--r--   0        0        0    19073 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/utils.py
--rw-r--r--   0        0        0    21568 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/__init__.py
--rw-r--r--   0        0        0     1534 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/activate.py
--rw-r--r--   0        0        0    14194 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0        0        0     2372 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/apptotal.py
--rw-r--r--   0        0        0     2992 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/audit_logs.py
--rw-r--r--   0        0        0     3140 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/authentication_settings.py
--rw-r--r--   0        0        0     2754 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/client.py
--rw-r--r--   0        0        0    18513 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/cloud_apps.py
--rw-r--r--   0        0        0     2872 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/device_management.py
--rw-r--r--   0        0        0    27473 2024-05-06 07:40:30.099598 zscaler_sdk_python-0.1.7/zscaler/zia/dlp.py
--rw-r--r--   0        0        0      794 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/errors.py
--rw-r--r--   0        0        0    39908 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/firewall.py
--rw-r--r--   0        0        0    11686 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/forwarding_control.py
--rw-r--r--   0        0        0     2909 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/isolation_profile.py
--rw-r--r--   0        0        0     5835 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/labels.py
--rw-r--r--   0        0        0    30762 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/locations.py
--rw-r--r--   0        0        0     6724 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/sandbox.py
--rw-r--r--   0        0        0     6792 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/security.py
--rw-r--r--   0        0        0     5298 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/ssl_inspection.py
--rw-r--r--   0        0        0    30729 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/traffic.py
--rw-r--r--   0        0        0    14484 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/url_categories.py
--rw-r--r--   0        0        0    14319 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/url_filtering.py
--rw-r--r--   0        0        0    13735 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/users.py
--rw-r--r--   0        0        0    12376 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/web_dlp.py
--rw-r--r--   0        0        0     1897 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/workload_groups.py
--rw-r--r--   0        0        0     6842 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zia/zpa_gateway.py
--rw-r--r--   0        0        0     2709 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/README.md
--rw-r--r--   0        0        0    24470 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/__init__.py
--rw-r--r--   0        0        0    13187 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments.py
--rw-r--r--   0        0        0    12445 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0        0        0    12019 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0        0        0     7942 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/certificates.py
--rw-r--r--   0        0        0     3844 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/client.py
--rw-r--r--   0        0        0     2667 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0        0        0    20849 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/connectors.py
--rw-r--r--   0        0        0     6189 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/emergency_access.py
--rw-r--r--   0        0        0      844 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/errors.py
--rw-r--r--   0        0        0     2764 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/idp.py
--rw-r--r--   0        0        0    34309 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/inspection.py
--rw-r--r--   0        0        0     3176 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/isolation_profile.py
--rw-r--r--   0        0        0    21697 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/lss.py
--rw-r--r--   0        0        0     2734 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/machine_groups.py
--rw-r--r--   0        0        0    31747 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/policies.py
--rw-r--r--   0        0        0     4317 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/posture_profiles.py
--rw-r--r--   0        0        0    32017 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0        0        0     9887 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/provisioning.py
--rw-r--r--   0        0        0     3632 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/saml_attributes.py
--rw-r--r--   0        0        0     4172 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/scim_attributes.py
--rw-r--r--   0        0        0     5041 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/scim_groups.py
--rw-r--r--   0        0        0     6103 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/segment_groups.py
--rw-r--r--   0        0        0     7776 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/server_groups.py
--rw-r--r--   0        0        0     6477 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/servers.py
--rw-r--r--   0        0        0    15428 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/service_edges.py
--rw-r--r--   0        0        0     4377 2024-05-06 07:40:30.103598 zscaler_sdk_python-0.1.7/zscaler/zpa/trusted_networks.py
--rw-r--r--   0        0        0    17518 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-05-09 20:16:57.159292 zscaler_sdk_python-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0    15746 2024-05-09 20:16:57.159292 zscaler_sdk_python-0.1.8/README.md
+-rw-r--r--   0        0        0     2292 2024-05-09 20:17:49.675310 zscaler_sdk_python-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1277 2024-05-09 20:17:49.679310 zscaler_sdk_python-0.1.8/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4967 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      738 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    24470 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    13187 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     7942 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3844 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20849 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    34309 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0     3176 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0        0        0    21697 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0    31713 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0     4317 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    31880 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     5041 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7776 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     4377 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17518 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.8/PKG-INFO
```

### Comparing `zscaler_sdk_python-0.1.7/LICENSE.md` & `zscaler_sdk_python-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/README.md` & `zscaler_sdk_python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/pyproject.toml` & `zscaler_sdk_python-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zscaler-sdk-python"
-version = "0.1.7"
+version = "0.1.8"
 description = "Official Python SDK for the Zscaler Products (Beta)"
 authors = ["Zscaler, Inc. <devrel@zscaler.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zscaler/zscaler-sdk-python"
 repository = "https://github.com/zscaler/zscaler-sdk-python"
 documentation = "https://zscaler-sdk-python.readthedocs.io"
```

### Comparing `zscaler_sdk_python-0.1.7/zscaler/__init__.py` & `zscaler_sdk_python-0.1.8/zscaler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler_sdk_python-0.1.7/zscaler/cache/cache.py` & `zscaler_sdk_python-0.1.8/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.1.8/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.1.8/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/constants.py` & `zscaler_sdk_python-0.1.8/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.1.8/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.1.8/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.1.8/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/logger.py` & `zscaler_sdk_python-0.1.8/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.1.8/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/user_agent.py` & `zscaler_sdk_python-0.1.8/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/utils.py` & `zscaler_sdk_python-0.1.8/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/activate.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/client.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/errors.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/labels.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/locations.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/security.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/users.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.1.8/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/README.md` & `zscaler_sdk_python-0.1.8/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/client.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/isolation_profile.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/machine_groups.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/policies.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                  |  ``client_forwarding``
                  |  ``isolation``
                  |  ``inspection``
                  |  ``redirection``
                  |  ``credential``
                  |  ``capabilities``
                  |  ``siem``
-                 
+
             rule_id (str): The unique identifier for the policy rule.
 
         Returns:
             :obj:`Box`: The resource record for the requested rule.
 
         Examples:
             >>> policy_rule = zpa.policies.get_rule(policy_id='99999',
@@ -251,15 +251,15 @@
                  |  ``client_forwarding``
                  |  ``isolation``
                  |  ``inspection``
                  |  ``redirection``
                  |  ``credential``
                  |  ``capabilities``
                  |  ``siem``
-                 
+
             rule_id (str):
                 The unique identifier for the policy rule.
 
         Returns:
             :obj:`int`: The response code for the operation.
 
         Examples:
```

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/privileged_remote_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,20 +121,21 @@
             "certificateId": certificate_id,
         }
 
         # Add optional parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        response = self.rest.post("/praPortal", json=payload)
+        response = self.rest.post("praPortal", json=payload)
         if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
-            if status_code > 299:
-                return None
-        return self.get_portal(response.get("id"))
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
 
     def update_portal(self, portal_id: str, **kwargs) -> Box:
         """
         Updates the specified pra portal.
 
         Args:
             portal_id (str):
@@ -471,20 +472,14 @@
             :obj:`Box`: The resource record for the pra credential.
 
         Examples:
             >>> pprint(zpa.privileged_remote_access.get_credential('99999'))
 
         """
         return self.rest.get(f"credential/{credential_id}")
-        # response = self.rest.get("/credential/%s" % (credential_id))
-        # if isinstance(response, Response):
-        #     status_code = response.status_code
-        #     if status_code != 200:
-        #         return None
-        # return response
 
     def add_credential(
         self,
         name: str,
         credential_type: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
```

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/zscaler/zpa/trusted_networks.py` & `zscaler_sdk_python-0.1.8/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.7/PKG-INFO` & `zscaler_sdk_python-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://github.com/zscaler/zscaler-sdk-python
 License: MIT
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Requires-Python: >=3.8,<4.0
```


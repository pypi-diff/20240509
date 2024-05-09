# Comparing `tmp/ambient_backend_api_client-0.1.0.tar.gz` & `tmp/ambient_backend_api_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_backend_api_client-0.1.0.tar", last modified: Thu May  9 02:27:07 2024, max compression
+gzip compressed data, was "ambient_backend_api_client-0.1.1.tar", last modified: Thu May  9 02:33:53 2024, max compression
```

## Comparing `ambient_backend_api_client-0.1.0.tar` & `ambient_backend_api_client-0.1.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:27:07.216222 ambient_backend_api_client-0.1.0/
--rw-r--r--   0 jose       (501) staff       (20)      582 2024-05-09 02:27:07.216167 ambient_backend_api_client-0.1.0/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)    10650 2024-05-09 02:16:18.000000 ambient_backend_api_client-0.1.0/README.md
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:27:07.196078 ambient_backend_api_client-0.1.0/ambient_backend_api_client/
--rw-r--r--   0 jose       (501) staff       (20)     4897 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/__init__.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:27:07.200951 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/
--rw-r--r--   0 jose       (501) staff       (20)      578 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)    71865 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/clusters_api.py
--rw-r--r--   0 jose       (501) staff       (20)    10046 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/health_api.py
--rw-r--r--   0 jose       (501) staff       (20)    81888 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/nodes_api.py
--rw-r--r--   0 jose       (501) staff       (20)    53254 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/notifications_api.py
--rw-r--r--   0 jose       (501) staff       (20)    19071 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/ping_api.py
--rw-r--r--   0 jose       (501) staff       (20)    21780 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/requests_api.py
--rw-r--r--   0 jose       (501) staff       (20)    42278 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/services_api.py
--rw-r--r--   0 jose       (501) staff       (20)    62218 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/users_api.py
--rw-r--r--   0 jose       (501) staff       (20)    26521 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api_client.py
--rw-r--r--   0 jose       (501) staff       (20)      652 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/api_response.py
--rw-r--r--   0 jose       (501) staff       (20)    14468 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/configuration.py
--rw-r--r--   0 jose       (501) staff       (20)     5972 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/exceptions.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:27:07.208632 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/
--rw-r--r--   0 jose       (501) staff       (20)     3715 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/__init__.py
--rw-r--r--   0 jose       (501) staff       (20)      806 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/account_type.py
--rw-r--r--   0 jose       (501) staff       (20)      757 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3064 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/auth0_device_code_response.py
--rw-r--r--   0 jose       (501) staff       (20)     5870 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/cluster.py
--rw-r--r--   0 jose       (501) staff       (20)     5710 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/cluster_create.py
--rw-r--r--   0 jose       (501) staff       (20)     3477 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/create_service_acct_request.py
--rw-r--r--   0 jose       (501) staff       (20)      765 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/creation_method.py
--rw-r--r--   0 jose       (501) staff       (20)     2995 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/http_validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)      989 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/interface_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     2786 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/list_results_response.py
--rw-r--r--   0 jose       (501) staff       (20)      936 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/models_cluster_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      853 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/models_node_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     4605 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/network_interface.py
--rw-r--r--   0 jose       (501) staff       (20)     6732 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node.py
--rw-r--r--   0 jose       (501) staff       (20)      769 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node_architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     6997 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node_create.py
--rw-r--r--   0 jose       (501) staff       (20)      751 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     5059 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification.py
--rw-r--r--   0 jose       (501) staff       (20)     3245 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification_list.py
--rw-r--r--   0 jose       (501) staff       (20)     3037 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification_request.py
--rw-r--r--   0 jose       (501) staff       (20)      803 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification_severity_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     5309 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/organization_create.py
--rw-r--r--   0 jose       (501) staff       (20)      812 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/owner_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3514 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/post_clusters_response.py
--rw-r--r--   0 jose       (501) staff       (20)     3510 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/post_service_response.py
--rw-r--r--   0 jose       (501) staff       (20)     5514 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/request.py
--rw-r--r--   0 jose       (501) staff       (20)      826 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/request_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1125 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/resource_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      731 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     5757 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service.py
--rw-r--r--   0 jose       (501) staff       (20)     6005 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_create.py
--rw-r--r--   0 jose       (501) staff       (20)     3205 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_list.py
--rw-r--r--   0 jose       (501) staff       (20)      788 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_state.py
--rw-r--r--   0 jose       (501) staff       (20)      836 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      838 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/status_enum_input.py
--rw-r--r--   0 jose       (501) staff       (20)      834 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/subscription_model_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3113 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/token_response.py
--rw-r--r--   0 jose       (501) staff       (20)     6441 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/user.py
--rw-r--r--   0 jose       (501) staff       (20)     2573 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/user_preferences.py
--rw-r--r--   0 jose       (501) staff       (20)      815 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/user_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     3096 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)     4885 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/validation_error_loc_inner.py
--rw-r--r--   0 jose       (501) staff       (20)        0 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/py.typed
--rw-r--r--   0 jose       (501) staff       (20)     6854 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client/rest.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:27:07.215956 ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/
--rw-r--r--   0 jose       (501) staff       (20)      582 2024-05-09 02:27:07.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/PKG-INFO
--rw-r--r--   0 jose       (501) staff       (20)     4806 2024-05-09 02:27:07.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 jose       (501) staff       (20)        1 2024-05-09 02:27:07.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 jose       (501) staff       (20)      112 2024-05-09 02:27:07.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/requires.txt
--rw-r--r--   0 jose       (501) staff       (20)       27 2024-05-09 02:27:07.000000 ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/top_level.txt
--rw-r--r--   0 jose       (501) staff       (20)     2018 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/pyproject.toml
--rw-r--r--   0 jose       (501) staff       (20)       69 2024-05-09 02:27:07.216427 ambient_backend_api_client-0.1.0/setup.cfg
--rw-r--r--   0 jose       (501) staff       (20)     1406 2024-05-09 02:13:20.000000 ambient_backend_api_client-0.1.0/setup.py
-drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:27:07.215664 ambient_backend_api_client-0.1.0/test/
--rw-r--r--   0 jose       (501) staff       (20)      702 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_account_type.py
--rw-r--r--   0 jose       (501) staff       (20)      737 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1908 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_auth0_device_code_response.py
--rw-r--r--   0 jose       (501) staff       (20)     2285 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_cluster.py
--rw-r--r--   0 jose       (501) staff       (20)     2288 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_cluster_create.py
--rw-r--r--   0 jose       (501) staff       (20)     1937 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_clusters_api.py
--rw-r--r--   0 jose       (501) staff       (20)     1681 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_create_service_acct_request.py
--rw-r--r--   0 jose       (501) staff       (20)      723 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_creation_method.py
--rw-r--r--   0 jose       (501) staff       (20)      764 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_health_api.py
--rw-r--r--   0 jose       (501) staff       (20)     1732 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_http_validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_interface_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1689 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_list_results_response.py
--rw-r--r--   0 jose       (501) staff       (20)      788 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_models_cluster_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      767 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_models_node_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1708 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_network_interface.py
--rw-r--r--   0 jose       (501) staff       (20)     2793 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_node.py
--rw-r--r--   0 jose       (501) staff       (20)      766 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_node_architecture_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     2797 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_node_create.py
--rw-r--r--   0 jose       (501) staff       (20)      710 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_node_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1982 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_nodes_api.py
--rw-r--r--   0 jose       (501) staff       (20)     2137 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_notification.py
--rw-r--r--   0 jose       (501) staff       (20)     3238 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_notification_list.py
--rw-r--r--   0 jose       (501) staff       (20)     1736 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_notification_request.py
--rw-r--r--   0 jose       (501) staff       (20)      794 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_notification_severity_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1678 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_notifications_api.py
--rw-r--r--   0 jose       (501) staff       (20)     2020 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_organization_create.py
--rw-r--r--   0 jose       (501) staff       (20)      717 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_owner_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      890 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_ping_api.py
--rw-r--r--   0 jose       (501) staff       (20)     3788 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_post_clusters_response.py
--rw-r--r--   0 jose       (501) staff       (20)     3726 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_post_service_response.py
--rw-r--r--   0 jose       (501) staff       (20)     2132 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_request.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_request_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      997 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_requests_api.py
--rw-r--r--   0 jose       (501) staff       (20)      738 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_resource_type_enum.py
--rw-r--r--   0 jose       (501) staff       (20)      681 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     2226 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_service.py
--rw-r--r--   0 jose       (501) staff       (20)     2264 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_service_create.py
--rw-r--r--   0 jose       (501) staff       (20)     3830 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_service_list.py
--rw-r--r--   0 jose       (501) staff       (20)      709 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_service_state.py
--rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_service_status_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1311 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_services_api.py
--rw-r--r--   0 jose       (501) staff       (20)      731 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_status_enum_input.py
--rw-r--r--   0 jose       (501) staff       (20)      773 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_subscription_model_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1657 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_token_response.py
--rw-r--r--   0 jose       (501) staff       (20)     2339 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_user.py
--rw-r--r--   0 jose       (501) staff       (20)     1410 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_user_preferences.py
--rw-r--r--   0 jose       (501) staff       (20)      710 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_user_role_enum.py
--rw-r--r--   0 jose       (501) staff       (20)     1623 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_users_api.py
--rw-r--r--   0 jose       (501) staff       (20)     1626 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_validation_error.py
--rw-r--r--   0 jose       (501) staff       (20)     1475 2024-05-09 02:10:11.000000 ambient_backend_api_client-0.1.0/test/test_validation_error_loc_inner.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:33:53.241070 ambient_backend_api_client-0.1.1/
+-rw-r--r--   0 jose       (501) staff       (20)      582 2024-05-09 02:33:53.241009 ambient_backend_api_client-0.1.1/PKG-INFO
+-rw-r--r--   0 jose       (501) staff       (20)    10650 2024-05-09 02:32:00.000000 ambient_backend_api_client-0.1.1/README.md
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:33:53.216968 ambient_backend_api_client-0.1.1/ambient_backend_api_client/
+-rw-r--r--   0 jose       (501) staff       (20)     4897 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/__init__.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:33:53.222595 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/
+-rw-r--r--   0 jose       (501) staff       (20)      578 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/__init__.py
+-rw-r--r--   0 jose       (501) staff       (20)    71865 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/clusters_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    10046 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/health_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    81888 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/nodes_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    53254 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/notifications_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    19071 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/ping_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    21780 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/requests_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    42278 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/services_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    62218 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/users_api.py
+-rw-r--r--   0 jose       (501) staff       (20)    26521 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api_client.py
+-rw-r--r--   0 jose       (501) staff       (20)      652 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/api_response.py
+-rw-r--r--   0 jose       (501) staff       (20)    14468 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/configuration.py
+-rw-r--r--   0 jose       (501) staff       (20)     5972 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/exceptions.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:33:53.231828 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/
+-rw-r--r--   0 jose       (501) staff       (20)     3715 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/__init__.py
+-rw-r--r--   0 jose       (501) staff       (20)      806 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/account_type.py
+-rw-r--r--   0 jose       (501) staff       (20)      757 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/architecture_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     3064 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/auth0_device_code_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     5870 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/cluster.py
+-rw-r--r--   0 jose       (501) staff       (20)     5710 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/cluster_create.py
+-rw-r--r--   0 jose       (501) staff       (20)     3477 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/create_service_acct_request.py
+-rw-r--r--   0 jose       (501) staff       (20)      765 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/creation_method.py
+-rw-r--r--   0 jose       (501) staff       (20)     2995 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/http_validation_error.py
+-rw-r--r--   0 jose       (501) staff       (20)      989 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/interface_type_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     2786 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/list_results_response.py
+-rw-r--r--   0 jose       (501) staff       (20)      936 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/models_cluster_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      853 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/models_node_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     4605 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/network_interface.py
+-rw-r--r--   0 jose       (501) staff       (20)     6732 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node.py
+-rw-r--r--   0 jose       (501) staff       (20)      769 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node_architecture_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     6997 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node_create.py
+-rw-r--r--   0 jose       (501) staff       (20)      751 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node_role_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     5059 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification.py
+-rw-r--r--   0 jose       (501) staff       (20)     3245 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification_list.py
+-rw-r--r--   0 jose       (501) staff       (20)     3037 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification_request.py
+-rw-r--r--   0 jose       (501) staff       (20)      803 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification_severity_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     5309 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/organization_create.py
+-rw-r--r--   0 jose       (501) staff       (20)      812 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/owner_type_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     3514 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/post_clusters_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     3510 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/post_service_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     5514 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/request.py
+-rw-r--r--   0 jose       (501) staff       (20)      826 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/request_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1125 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/resource_type_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      731 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/role_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     5757 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service.py
+-rw-r--r--   0 jose       (501) staff       (20)     6005 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_create.py
+-rw-r--r--   0 jose       (501) staff       (20)     3205 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_list.py
+-rw-r--r--   0 jose       (501) staff       (20)      788 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_state.py
+-rw-r--r--   0 jose       (501) staff       (20)      836 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      838 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/status_enum_input.py
+-rw-r--r--   0 jose       (501) staff       (20)      834 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/subscription_model_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     3113 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/token_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     6441 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/user.py
+-rw-r--r--   0 jose       (501) staff       (20)     2573 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/user_preferences.py
+-rw-r--r--   0 jose       (501) staff       (20)      815 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/user_role_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     3096 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/validation_error.py
+-rw-r--r--   0 jose       (501) staff       (20)     4885 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/validation_error_loc_inner.py
+-rw-r--r--   0 jose       (501) staff       (20)        0 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/py.typed
+-rw-r--r--   0 jose       (501) staff       (20)     6854 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client/rest.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:33:53.240641 ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/
+-rw-r--r--   0 jose       (501) staff       (20)      582 2024-05-09 02:33:53.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 jose       (501) staff       (20)     4806 2024-05-09 02:33:53.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jose       (501) staff       (20)        1 2024-05-09 02:33:53.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jose       (501) staff       (20)      112 2024-05-09 02:33:53.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/requires.txt
+-rw-r--r--   0 jose       (501) staff       (20)       27 2024-05-09 02:33:53.000000 ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/top_level.txt
+-rw-r--r--   0 jose       (501) staff       (20)     2018 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/pyproject.toml
+-rw-r--r--   0 jose       (501) staff       (20)       69 2024-05-09 02:33:53.241300 ambient_backend_api_client-0.1.1/setup.cfg
+-rw-r--r--   0 jose       (501) staff       (20)     1406 2024-05-09 02:32:44.000000 ambient_backend_api_client-0.1.1/setup.py
+drwxr-xr-x   0 jose       (501) staff       (20)        0 2024-05-09 02:33:53.240469 ambient_backend_api_client-0.1.1/test/
+-rw-r--r--   0 jose       (501) staff       (20)      702 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_account_type.py
+-rw-r--r--   0 jose       (501) staff       (20)      737 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_architecture_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1908 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_auth0_device_code_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     2285 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_cluster.py
+-rw-r--r--   0 jose       (501) staff       (20)     2288 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_cluster_create.py
+-rw-r--r--   0 jose       (501) staff       (20)     1937 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_clusters_api.py
+-rw-r--r--   0 jose       (501) staff       (20)     1681 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_create_service_acct_request.py
+-rw-r--r--   0 jose       (501) staff       (20)      723 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_creation_method.py
+-rw-r--r--   0 jose       (501) staff       (20)      764 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_health_api.py
+-rw-r--r--   0 jose       (501) staff       (20)     1732 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_http_validation_error.py
+-rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_interface_type_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1689 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_list_results_response.py
+-rw-r--r--   0 jose       (501) staff       (20)      788 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_models_cluster_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      767 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_models_node_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1708 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_network_interface.py
+-rw-r--r--   0 jose       (501) staff       (20)     2793 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_node.py
+-rw-r--r--   0 jose       (501) staff       (20)      766 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_node_architecture_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     2797 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_node_create.py
+-rw-r--r--   0 jose       (501) staff       (20)      710 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_node_role_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1982 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_nodes_api.py
+-rw-r--r--   0 jose       (501) staff       (20)     2137 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_notification.py
+-rw-r--r--   0 jose       (501) staff       (20)     3238 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_notification_list.py
+-rw-r--r--   0 jose       (501) staff       (20)     1736 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_notification_request.py
+-rw-r--r--   0 jose       (501) staff       (20)      794 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_notification_severity_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1678 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_notifications_api.py
+-rw-r--r--   0 jose       (501) staff       (20)     2020 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_organization_create.py
+-rw-r--r--   0 jose       (501) staff       (20)      717 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_owner_type_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      890 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_ping_api.py
+-rw-r--r--   0 jose       (501) staff       (20)     3788 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_post_clusters_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     3726 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_post_service_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     2132 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_request.py
+-rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_request_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      997 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_requests_api.py
+-rw-r--r--   0 jose       (501) staff       (20)      738 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_resource_type_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)      681 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_role_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     2226 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_service.py
+-rw-r--r--   0 jose       (501) staff       (20)     2264 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_service_create.py
+-rw-r--r--   0 jose       (501) staff       (20)     3830 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_service_list.py
+-rw-r--r--   0 jose       (501) staff       (20)      709 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_service_state.py
+-rw-r--r--   0 jose       (501) staff       (20)      745 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_service_status_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1311 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_services_api.py
+-rw-r--r--   0 jose       (501) staff       (20)      731 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_status_enum_input.py
+-rw-r--r--   0 jose       (501) staff       (20)      773 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_subscription_model_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1657 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_token_response.py
+-rw-r--r--   0 jose       (501) staff       (20)     2339 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_user.py
+-rw-r--r--   0 jose       (501) staff       (20)     1410 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_user_preferences.py
+-rw-r--r--   0 jose       (501) staff       (20)      710 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_user_role_enum.py
+-rw-r--r--   0 jose       (501) staff       (20)     1623 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_users_api.py
+-rw-r--r--   0 jose       (501) staff       (20)     1626 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_validation_error.py
+-rw-r--r--   0 jose       (501) staff       (20)     1475 2024-05-09 02:31:03.000000 ambient_backend_api_client-0.1.1/test/test_validation_error_loc_inner.py
```

### Comparing `ambient_backend_api_client-0.1.0/PKG-INFO` & `ambient_backend_api_client-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient_backend_api_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: jose@ambientlabscomputing.com
 Keywords: OpenAPI,OpenAPI-Generator,FastAPI
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `ambient_backend_api_client-0.1.0/README.md` & `ambient_backend_api_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/__init__.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/__init__.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/clusters_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/health_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/nodes_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/notifications_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/ping_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/requests_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/services_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api/users_api.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api_client.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/api_response.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/api_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/configuration.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/exceptions.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/__init__.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/account_type.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/architecture_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/auth0_device_code_response.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/cluster.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class Cluster(BaseModel):
     """
     Cluster
     """ # noqa: E501
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = '3e880c1c-5fa7-414c-92b4-d58119c93ee7'
+    identifier: Optional[StrictStr] = '1126bb6b-9e41-49b3-9fa0-75cd01cb93f2'
     owner_id: Optional[StrictStr] = None
     owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     role: RoleEnum
     architecture: ArchitectureEnum
@@ -124,15 +124,15 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '3e880c1c-5fa7-414c-92b4-d58119c93ee7',
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '1126bb6b-9e41-49b3-9fa0-75cd01cb93f2',
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/cluster_create.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/cluster_create.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 class ClusterCreate(BaseModel):
     """
     ClusterCreate
     """ # noqa: E501
     name: StrictStr
     resource_type: Optional[ResourceTypeEnum] = None
-    identifier: Optional[StrictStr] = '3e880c1c-5fa7-414c-92b4-d58119c93ee7'
+    identifier: Optional[StrictStr] = '1126bb6b-9e41-49b3-9fa0-75cd01cb93f2'
     owner_id: Optional[StrictStr] = None
     owner_type: Optional[OwnerTypeEnum] = None
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     role: RoleEnum
     architecture: ArchitectureEnum
@@ -122,15 +122,15 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "resource_type": obj.get("resource_type"),
-            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '3e880c1c-5fa7-414c-92b4-d58119c93ee7',
+            "identifier": obj.get("identifier") if obj.get("identifier") is not None else '1126bb6b-9e41-49b3-9fa0-75cd01cb93f2',
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "role": obj.get("role"),
             "architecture": obj.get("architecture"),
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/create_service_acct_request.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/creation_method.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/http_validation_error.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/interface_type_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/list_results_response.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/list_results_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing_extensions import Self
 
 class ListResultsResponse(BaseModel):
     """
     ListResultsResponse
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Wed May  8 19:55:26 2024'
+    timestamp: Optional[StrictStr] = 'Wed May  8 20:30:12 2024'
     results: List[Any]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -79,13 +79,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 19:55:26 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 20:30:12 2024',
             "results": obj.get("results")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/models_node_status_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/network_interface.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node_architecture_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node_create.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/node_role_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification_list.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class NotificationList(BaseModel):
     """
     NotificationList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Wed May  8 19:55:26 2024'
+    timestamp: Optional[StrictStr] = 'Wed May  8 20:30:12 2024'
     results: List[Notification]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 19:55:26 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 20:30:12 2024',
             "results": [Notification.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification_request.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/notification_severity_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/organization_create.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/owner_type_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/post_clusters_response.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/post_clusters_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class PostClustersResponse(BaseModel):
     """
     PostClustersResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = 'Wed May  8 19:55:26 2024'
+    requested_ts: Optional[StrictStr] = 'Wed May  8 20:30:12 2024'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
     cluster: Cluster
     __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "cluster"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -85,15 +85,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Wed May  8 19:55:26 2024',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Wed May  8 20:30:12 2024',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "cluster": Cluster.from_dict(obj["cluster"]) if obj.get("cluster") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/post_service_response.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/post_service_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class PostServiceResponse(BaseModel):
     """
     PostServiceResponse
     """ # noqa: E501
     request_id: StrictStr
-    requested_ts: Optional[StrictStr] = 'Wed May  8 19:55:26 2024'
+    requested_ts: Optional[StrictStr] = 'Wed May  8 20:30:12 2024'
     location_root: Optional[StrictStr] = 'http://localhost:8001/requests/'
     refresh_interval: Optional[StrictInt] = 10
     service: Service
     __properties: ClassVar[List[str]] = ["request_id", "requested_ts", "location_root", "refresh_interval", "service"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -85,15 +85,15 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "request_id": obj.get("request_id"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Wed May  8 19:55:26 2024',
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 'Wed May  8 20:30:12 2024',
             "location_root": obj.get("location_root") if obj.get("location_root") is not None else 'http://localhost:8001/requests/',
             "refresh_interval": obj.get("refresh_interval") if obj.get("refresh_interval") is not None else 10,
             "service": Service.from_dict(obj["service"]) if obj.get("service") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/request.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     owner_id: StrictStr
     owner_type: OwnerTypeEnum
     description: Optional[StrictStr] = None
     requests: Optional[List[StrictStr]] = None
     notifications: Optional[List[StrictStr]] = None
     status: Optional[RequestStatusEnum] = None
     error: Optional[StrictStr] = None
-    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.715219726437265E9
+    requested_ts: Optional[Union[StrictFloat, StrictInt]] = 1.715221812342966E9
     started_ts: Optional[Union[StrictFloat, StrictInt]] = None
     failed_ts: Optional[Union[StrictFloat, StrictInt]] = None
     completed_ts: Optional[Union[StrictFloat, StrictInt]] = None
     notes: Optional[List[StrictStr]] = None
     data: Optional[Dict[str, Any]] = None
     __properties: ClassVar[List[str]] = ["name", "resource_type", "identifier", "owner_id", "owner_type", "description", "requests", "notifications", "status", "error", "requested_ts", "started_ts", "failed_ts", "completed_ts", "notes", "data"]
 
@@ -129,15 +129,15 @@
             "owner_id": obj.get("owner_id"),
             "owner_type": obj.get("owner_type"),
             "description": obj.get("description"),
             "requests": obj.get("requests"),
             "notifications": obj.get("notifications"),
             "status": obj.get("status"),
             "error": obj.get("error"),
-            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.715219726437265E9,
+            "requested_ts": obj.get("requested_ts") if obj.get("requested_ts") is not None else 1.715221812342966E9,
             "started_ts": obj.get("started_ts"),
             "failed_ts": obj.get("failed_ts"),
             "completed_ts": obj.get("completed_ts"),
             "notes": obj.get("notes"),
             "data": obj.get("data")
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/request_status_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/resource_type_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/role_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_create.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_list.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from typing_extensions import Self
 
 class ServiceList(BaseModel):
     """
     ServiceList
     """ # noqa: E501
     count: StrictInt
-    timestamp: Optional[StrictStr] = 'Wed May  8 19:55:26 2024'
+    timestamp: Optional[StrictStr] = 'Wed May  8 20:30:12 2024'
     results: List[Service]
     __properties: ClassVar[List[str]] = ["count", "timestamp", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -87,13 +87,13 @@
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
-            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 19:55:26 2024',
+            "timestamp": obj.get("timestamp") if obj.get("timestamp") is not None else 'Wed May  8 20:30:12 2024',
             "results": [Service.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_state.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/service_status_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/status_enum_input.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/subscription_model_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/token_response.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/user.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/user_preferences.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/user_role_enum.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/validation_error.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/models/validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client/rest.py` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/PKG-INFO` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient_backend_api_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: FastAPI
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: jose@ambientlabscomputing.com
 Keywords: OpenAPI,OpenAPI-Generator,FastAPI
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `ambient_backend_api_client-0.1.0/ambient_backend_api_client.egg-info/SOURCES.txt` & `ambient_backend_api_client-0.1.1/ambient_backend_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/pyproject.toml` & `ambient_backend_api_client-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/setup.py` & `ambient_backend_api_client-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "ambient_backend_api_client"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "aiohttp >= 3.0.0",
     "aiohttp-retry >= 2.8.3",
     "pydantic >= 2",
```

### Comparing `ambient_backend_api_client-0.1.0/test/test_account_type.py` & `ambient_backend_api_client-0.1.1/test/test_account_type.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_architecture_enum.py` & `ambient_backend_api_client-0.1.1/test/test_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_auth0_device_code_response.py` & `ambient_backend_api_client-0.1.1/test/test_auth0_device_code_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_cluster.py` & `ambient_backend_api_client-0.1.1/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_cluster_create.py` & `ambient_backend_api_client-0.1.1/test/test_cluster_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_clusters_api.py` & `ambient_backend_api_client-0.1.1/test/test_clusters_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_create_service_acct_request.py` & `ambient_backend_api_client-0.1.1/test/test_create_service_acct_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_creation_method.py` & `ambient_backend_api_client-0.1.1/test/test_creation_method.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_health_api.py` & `ambient_backend_api_client-0.1.1/test/test_health_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_http_validation_error.py` & `ambient_backend_api_client-0.1.1/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_interface_type_enum.py` & `ambient_backend_api_client-0.1.1/test/test_interface_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_list_results_response.py` & `ambient_backend_api_client-0.1.1/test/test_list_results_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_models_cluster_status_enum.py` & `ambient_backend_api_client-0.1.1/test/test_models_cluster_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_models_node_status_enum.py` & `ambient_backend_api_client-0.1.1/test/test_models_node_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_network_interface.py` & `ambient_backend_api_client-0.1.1/test/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_node.py` & `ambient_backend_api_client-0.1.1/test/test_node.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_node_architecture_enum.py` & `ambient_backend_api_client-0.1.1/test/test_node_architecture_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_node_create.py` & `ambient_backend_api_client-0.1.1/test/test_node_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_node_role_enum.py` & `ambient_backend_api_client-0.1.1/test/test_node_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_nodes_api.py` & `ambient_backend_api_client-0.1.1/test/test_nodes_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_notification.py` & `ambient_backend_api_client-0.1.1/test/test_notification.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_notification_list.py` & `ambient_backend_api_client-0.1.1/test/test_notification_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_notification_request.py` & `ambient_backend_api_client-0.1.1/test/test_notification_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_notification_severity_enum.py` & `ambient_backend_api_client-0.1.1/test/test_notification_severity_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_notifications_api.py` & `ambient_backend_api_client-0.1.1/test/test_notifications_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_organization_create.py` & `ambient_backend_api_client-0.1.1/test/test_organization_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_owner_type_enum.py` & `ambient_backend_api_client-0.1.1/test/test_owner_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_ping_api.py` & `ambient_backend_api_client-0.1.1/test/test_ping_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_post_clusters_response.py` & `ambient_backend_api_client-0.1.1/test/test_post_clusters_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_post_service_response.py` & `ambient_backend_api_client-0.1.1/test/test_post_service_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_request.py` & `ambient_backend_api_client-0.1.1/test/test_request.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_request_status_enum.py` & `ambient_backend_api_client-0.1.1/test/test_request_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_requests_api.py` & `ambient_backend_api_client-0.1.1/test/test_requests_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_resource_type_enum.py` & `ambient_backend_api_client-0.1.1/test/test_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_role_enum.py` & `ambient_backend_api_client-0.1.1/test/test_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_service.py` & `ambient_backend_api_client-0.1.1/test/test_service.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_service_create.py` & `ambient_backend_api_client-0.1.1/test/test_service_create.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_service_list.py` & `ambient_backend_api_client-0.1.1/test/test_service_list.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_service_state.py` & `ambient_backend_api_client-0.1.1/test/test_service_state.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_service_status_enum.py` & `ambient_backend_api_client-0.1.1/test/test_service_status_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_services_api.py` & `ambient_backend_api_client-0.1.1/test/test_services_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_status_enum_input.py` & `ambient_backend_api_client-0.1.1/test/test_status_enum_input.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_subscription_model_enum.py` & `ambient_backend_api_client-0.1.1/test/test_subscription_model_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_token_response.py` & `ambient_backend_api_client-0.1.1/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_user.py` & `ambient_backend_api_client-0.1.1/test/test_user.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_user_preferences.py` & `ambient_backend_api_client-0.1.1/test/test_user_preferences.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_user_role_enum.py` & `ambient_backend_api_client-0.1.1/test/test_user_role_enum.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_users_api.py` & `ambient_backend_api_client-0.1.1/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_validation_error.py` & `ambient_backend_api_client-0.1.1/test/test_validation_error.py`

 * *Files identical despite different names*

### Comparing `ambient_backend_api_client-0.1.0/test/test_validation_error_loc_inner.py` & `ambient_backend_api_client-0.1.1/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*


# Comparing `tmp/pubnub-7.4.4.tar.gz` & `tmp/pubnub-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubnub-7.4.4.tar", last modified: Wed Apr 10 16:47:46 2024, max compression
+gzip compressed data, was "pubnub-8.0.0.tar", last modified: Thu May  9 15:36:04 2024, max compression
```

## Comparing `pubnub-7.4.4.tar` & `pubnub-8.0.0.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-10 16:47:34.000000 pubnub-7.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-10 16:47:46.838263 pubnub-7.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-10 16:47:34.000000 pubnub-7.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.818263 pubnub-7.4.4/pubnub/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/crypto_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/dtos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.818263 pubnub-7.4.4/pubnub/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/grant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/grant_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/access/revoke_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/channel_groups/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/membership/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/add_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/fetch_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/remove_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/membership/update_memberships.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/space/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/create_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/remove_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/space/update_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.822263 pubnub-7.4.4/pubnub/endpoints/entities/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/create_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/remove_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/entities/user/update_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/fetch_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/file_operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/delete_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/download_file_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/fetch_upload_details.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/file_based_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/list_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/publish_file_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/send_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/file_operations/send_file_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/history_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/message_actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/add_message_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/get_message_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_actions/remove_message_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/message_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_all_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/remove_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/set_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/get_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/manage_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/remove_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/members/set_channel_members.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/get_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/manage_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/remove_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/set_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/objects_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.826263 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/remove_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/set_uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/endpoints/presence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/here_now.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/leave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/set_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/presence/where_now.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/endpoints/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/fire.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/pubsub/subscribe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/endpoints/push/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/add_channels_to_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/list_push_provisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/remove_channels_from_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/push/remove_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/endpoints/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/event_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    20582 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/effects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/event_engine/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/invocations.py
--rw-r--r--   0 runner    (1001) docker     (127)    41947 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/models/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/event_engine/statemachine.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19670 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.830263 pubnub-7.4.4/pubnub/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/access_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/channel_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/entities/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/message_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/message_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/objects_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/objects_v2/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/pn_error_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/push.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.834263 pubnub-7.4.4/pubnub/models/consumer/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/access_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/pn_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/space.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/consumer/v3/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/pubnub/models/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/server/subscribe.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/models/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pnconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pubnub.py
--rw-r--r--   0 runner    (1001) docker     (127)    30155 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pubnub_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20728 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/pubnub_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/pubnub/request_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/request_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/request_handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/request_handlers/requests_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9095 2024-04-10 16:47:34.000000 pubnub-7.4.4/pubnub/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:47:46.838263 pubnub-7.4.4/pubnub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 16:47:46.000000 pubnub-7.4.4/pubnub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 16:47:46.838263 pubnub-7.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-10 16:47:34.000000 pubnub-7.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.997887 pubnub-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 15:35:51.000000 pubnub-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-09 15:36:03.997887 pubnub-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-09 15:35:51.000000 pubnub-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.977887 pubnub-8.0.0/pubnub/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/crypto_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/dtos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.981887 pubnub-8.0.0/pubnub/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.981887 pubnub-8.0.0/pubnub/endpoints/access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/access/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/access/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/access/grant_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/access/revoke_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.981887 pubnub-8.0.0/pubnub/endpoints/channel_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/channel_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/channel_groups/remove_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.981887 pubnub-8.0.0/pubnub/endpoints/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.981887 pubnub-8.0.0/pubnub/endpoints/entities/membership/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/membership/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/membership/add_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/membership/fetch_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/membership/remove_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/membership/update_memberships.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.981887 pubnub-8.0.0/pubnub/endpoints/entities/space/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/space/create_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/space/fetch_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/space/fetch_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/space/remove_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/space/update_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.985887 pubnub-8.0.0/pubnub/endpoints/entities/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/user/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/user/fetch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/user/fetch_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/user/remove_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/entities/user/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/fetch_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.985887 pubnub-8.0.0/pubnub/endpoints/file_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/download_file_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/fetch_upload_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/file_based_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/publish_file_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/send_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/file_operations/send_file_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/history_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.985887 pubnub-8.0.0/pubnub/endpoints/message_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/message_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/message_actions/add_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/message_actions/get_message_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/message_actions/remove_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/message_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.985887 pubnub-8.0.0/pubnub/endpoints/objects_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.985887 pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/get_all_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/get_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/remove_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/set_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.985887 pubnub-8.0.0/pubnub/endpoints/objects_v2/members/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/members/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/members/get_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/members/manage_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/members/remove_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/members/set_channel_members.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.989887 pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/get_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/manage_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/remove_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/set_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/objects_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.989887 pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/get_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/remove_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/set_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.989887 pubnub-8.0.0/pubnub/endpoints/presence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/here_now.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/leave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/set_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/presence/where_now.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.989887 pubnub-8.0.0/pubnub/endpoints/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/pubsub/fire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/pubsub/subscribe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.989887 pubnub-8.0.0/pubnub/endpoints/push/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/push/add_channels_to_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/push/list_push_provisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/push/remove_channels_from_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/push/remove_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/endpoints/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.989887 pubnub-8.0.0/pubnub/event_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20881 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/effects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.993887 pubnub-8.0.0/pubnub/event_engine/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/models/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/models/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42059 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/models/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/event_engine/statemachine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19670 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.993887 pubnub-8.0.0/pubnub/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.993887 pubnub-8.0.0/pubnub/models/consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/access_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.993887 pubnub-8.0.0/pubnub/models/consumer/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/entities/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/entities/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/entities/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/entities/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/message_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/message_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.997887 pubnub-8.0.0/pubnub/models/consumer/objects_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/objects_v2/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/pn_error_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.997887 pubnub-8.0.0/pubnub/models/consumer/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/access_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/pn_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/consumer/v3/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.997887 pubnub-8.0.0/pubnub/models/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/server/subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/models/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/pnconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/pubnub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29971 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/pubnub_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21556 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/pubnub_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.997887 pubnub-8.0.0/pubnub/request_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/request_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/request_handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/request_handlers/requests_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-09 15:35:51.000000 pubnub-8.0.0/pubnub/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:36:03.997887 pubnub-8.0.0/pubnub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-09 15:36:03.000000 pubnub-8.0.0/pubnub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-09 15:36:03.000000 pubnub-8.0.0/pubnub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:36:03.000000 pubnub-8.0.0/pubnub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:36:03.000000 pubnub-8.0.0/pubnub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 15:36:03.000000 pubnub-8.0.0/pubnub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 15:36:03.000000 pubnub-8.0.0/pubnub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 15:36:03.997887 pubnub-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-09 15:35:51.000000 pubnub-8.0.0/setup.py
```

### Comparing `pubnub-7.4.4/LICENSE` & `pubnub-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/PKG-INFO` & `pubnub-8.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubnub
-Version: 7.4.4
+Version: 8.0.0
 Summary: PubNub Real-time push service in the cloud
 Home-page: http://pubnub.com
 Author: PubNub
 Author-email: support@pubnub.com
 License: PubNub Software Development Kit License
 Project-URL: Source, https://github.com/pubnub/python
 Project-URL: Documentation, https://www.pubnub.com/docs/sdks/python
```

### Comparing `pubnub-7.4.4/README.md` & `pubnub-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/__init__.py` & `pubnub-8.0.0/pubnub/__init__.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/builders.py` & `pubnub-8.0.0/pubnub/builders.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABCMeta, abstractmethod
-from .dtos import SubscribeOperation, UnsubscribeOperation
+
+from pubnub.models.subscription import PubNubChannel, PubNubChannelGroup
 from . import utils
 
 
 class PubSubBuilder(object):
     __metaclass__ = ABCMeta
 
-    def __init__(self, subscription_manager):
-        self._subscription_manager = subscription_manager
+    def __init__(self, pubnub_instance):
+        self._pubnub = pubnub_instance
         self._channel_subscriptions = []
         self._channel_group_subscriptions = []
 
     # TODO: make the 'channel' alias
     def channels(self, channels_list):
         utils.extend_list(self._channel_subscriptions, channels_list)
 
@@ -24,45 +25,38 @@
 
     @abstractmethod
     def execute(self):
         pass
 
 
 class SubscribeBuilder(PubSubBuilder):
-    def __init__(self, subscription_manager):
-        super(SubscribeBuilder, self).__init__(subscription_manager)
+    def __init__(self, pubnub_instance):
+        super(SubscribeBuilder, self).__init__(pubnub_instance)
         self._presence_enabled = False
         self._timetoken = 0
 
     def with_presence(self):
         self._presence_enabled = True
         return self
 
     def with_timetoken(self, timetoken):
         self._timetoken = timetoken
         return self
 
     def channel_subscriptions(self):
-        return self._channel_subscriptions
+        return [PubNubChannel(self._pubnub, channel).subscription(self._presence_enabled)
+                for channel in self._channel_subscriptions]
 
     def channel_group_subscriptions(self):
-        return self._channel_group_subscriptions
+        return [PubNubChannelGroup(self._pubnub, group).subscription(self._presence_enabled)
+                for group in self._channel_group_subscriptions]
 
     def execute(self):
-        subscribe_operation = SubscribeOperation(
-            channels=self._channel_subscriptions,
-            channel_groups=self._channel_group_subscriptions,
-            timetoken=self._timetoken,
-            presence_enabled=self._presence_enabled
-        )
+        subscription = self._pubnub.subscription_set(self.channel_subscriptions() + self.channel_group_subscriptions())
 
-        self._subscription_manager.adapt_subscribe_builder(subscribe_operation)
+        subscription.subscribe(timetoken=self._timetoken)
 
 
 class UnsubscribeBuilder(PubSubBuilder):
     def execute(self):
-        unsubscribe_operation = UnsubscribeOperation(
-            channels=self._channel_subscriptions,
-            channel_groups=self._channel_group_subscriptions
-        )
-
-        self._subscription_manager.adapt_unsubscribe_builder(unsubscribe_operation)
+        self._pubnub._subscription_registry.unsubscribe(channels=self._channel_subscriptions,
+                                                        groups=self._channel_group_subscriptions)
```

### Comparing `pubnub-7.4.4/pubnub/callbacks.py` & `pubnub-8.0.0/pubnub/callbacks.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/crypto.py` & `pubnub-8.0.0/pubnub/crypto.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/crypto_core.py` & `pubnub-8.0.0/pubnub/crypto_core.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/dtos.py` & `pubnub-8.0.0/pubnub/dtos.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,34 +18,44 @@
 
     @property
     def groups_with_pressence(self):
         if not self.presence_enabled:
             return self.channel_groups
         return self.channel_groups + [ch + '-pnpres' for ch in self.channel_groups]
 
+    @property
+    def channels_without_presence(self):
+        return list(filter(lambda ch: not ch.endswith('-pnpres'), self.channels))
+
+    @property
+    def channel_groups_without_presence(self):
+        return list(filter(lambda gr: not gr.endswith('-pnpres'), self.channel_groups))
+
 
 class UnsubscribeOperation(object):
     def __init__(self, channels=None, channel_groups=None):
         assert isinstance(channels, (list, tuple))
         assert isinstance(channel_groups, (list, tuple))
 
         self.channels = channels
         self.channel_groups = channel_groups
 
-    def get_subscribed_channels(self, channels, with_presence=False) -> list:
-        result = [ch for ch in channels if ch not in self.channels and not ch.endswith('-pnpres')]
-        if not with_presence:
-            return result
-        return result + [ch + '-pnpres' for ch in result]
-
-    def get_subscribed_channel_groups(self, channel_groups, with_presence=False) -> list:
-        result = [grp for grp in channel_groups if grp not in self.channel_groups and not grp.endswith('-pnpres')]
-        if not with_presence:
-            return result
-        return result + [grp + '-pnpres' for grp in result]
+    def get_subscribed_channels(self, channels) -> list:
+        return [ch for ch in channels if ch not in self.channels]
+
+    def get_subscribed_channel_groups(self, channel_groups) -> list:
+        return [grp for grp in channel_groups if grp not in self.channel_groups]
+
+    @property
+    def channels_without_presence(self):
+        return list(filter(lambda ch: not ch.endswith('-pnpres'), self.channels))
+
+    @property
+    def channel_groups_without_presence(self):
+        return list(filter(lambda gr: not gr.endswith('-pnpres'), self.channel_groups))
 
 
 class StateOperation(object):
     def __init__(self, channels=None, channel_groups=None, state=None):
         self.channels = channels
         self.channel_groups = channel_groups
         self.state = state
```

### Comparing `pubnub-7.4.4/pubnub/endpoints/access/audit.py` & `pubnub-8.0.0/pubnub/endpoints/access/audit.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/access/grant.py` & `pubnub-8.0.0/pubnub/endpoints/access/grant.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/access/grant_token.py` & `pubnub-8.0.0/pubnub/endpoints/access/grant_token.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/access/revoke_token.py` & `pubnub-8.0.0/pubnub/endpoints/access/revoke_token.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py` & `pubnub-8.0.0/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py` & `pubnub-8.0.0/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py` & `pubnub-8.0.0/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/channel_groups/remove_channel_group.py` & `pubnub-8.0.0/pubnub/endpoints/channel_groups/remove_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/endpoint.py` & `pubnub-8.0.0/pubnub/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/endpoint.py` & `pubnub-8.0.0/pubnub/endpoints/entities/endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/membership/add_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/entities/membership/add_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/membership/fetch_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/entities/membership/fetch_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/membership/remove_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/entities/membership/remove_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/membership/update_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/entities/membership/update_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/space/create_space.py` & `pubnub-8.0.0/pubnub/endpoints/entities/space/create_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_space.py` & `pubnub-8.0.0/pubnub/endpoints/entities/space/fetch_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/space/fetch_spaces.py` & `pubnub-8.0.0/pubnub/endpoints/entities/space/fetch_spaces.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/space/remove_space.py` & `pubnub-8.0.0/pubnub/endpoints/entities/space/remove_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/space/update_space.py` & `pubnub-8.0.0/pubnub/endpoints/entities/space/update_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/user/create_user.py` & `pubnub-8.0.0/pubnub/endpoints/entities/user/create_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_user.py` & `pubnub-8.0.0/pubnub/endpoints/entities/user/fetch_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/user/fetch_users.py` & `pubnub-8.0.0/pubnub/endpoints/entities/user/fetch_users.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/user/remove_user.py` & `pubnub-8.0.0/pubnub/endpoints/entities/user/remove_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/entities/user/update_user.py` & `pubnub-8.0.0/pubnub/endpoints/entities/user/update_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/fetch_messages.py` & `pubnub-8.0.0/pubnub/endpoints/fetch_messages.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/delete_file.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/delete_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/download_file.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/download_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/download_file_asyncio.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/download_file_asyncio.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/fetch_upload_details.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/fetch_upload_details.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/get_file_url.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/get_file_url.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/list_files.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/list_files.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/publish_file_message.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/publish_file_message.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/send_file.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/send_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/file_operations/send_file_asyncio.py` & `pubnub-8.0.0/pubnub/endpoints/file_operations/send_file_asyncio.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/history.py` & `pubnub-8.0.0/pubnub/endpoints/history.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/history_delete.py` & `pubnub-8.0.0/pubnub/endpoints/history_delete.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/message_actions/add_message_action.py` & `pubnub-8.0.0/pubnub/endpoints/message_actions/add_message_action.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/message_actions/get_message_actions.py` & `pubnub-8.0.0/pubnub/endpoints/message_actions/get_message_actions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/message_actions/remove_message_action.py` & `pubnub-8.0.0/pubnub/endpoints/message_actions/remove_message_action.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/message_count.py` & `pubnub-8.0.0/pubnub/endpoints/message_count.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/mixins.py` & `pubnub-8.0.0/pubnub/endpoints/mixins.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_all_channels.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/get_all_channels.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/get_channel.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/get_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/remove_channel.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/remove_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/channel/set_channel.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/channel/set_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     def build_path(self):
         return SetChannel.SET_CHANNEL_PATH % (self.pubnub.config.subscribe_key, self._channel)
 
     def build_data(self):
         payload = {
             "name": self._name,
             "description": self._description,
+            "status": self._status,
+            "type": self._type,
             "custom": self._custom
         }
         payload = StatusTypeAwareEndpoint.build_data(self, payload)
         return utils.write_value_as_string(payload)
 
     def create_response(self, envelope):
         return PNSetChannelMetadataResult(envelope)
```

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/get_channel_members.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/members/get_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/manage_channel_members.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/members/manage_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/remove_channel_members.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/members/remove_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/members/set_channel_members.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/members/set_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/get_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/get_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/manage_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/manage_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/remove_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/remove_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/memberships/set_memberships.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/memberships/set_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/objects_endpoint.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/objects_endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/get_uuid.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/get_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/remove_uuid.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/remove_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/objects_v2/uuid/set_uuid.py` & `pubnub-8.0.0/pubnub/endpoints/objects_v2/uuid/set_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/presence/get_state.py` & `pubnub-8.0.0/pubnub/endpoints/presence/get_state.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/presence/heartbeat.py` & `pubnub-8.0.0/pubnub/endpoints/presence/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/presence/here_now.py` & `pubnub-8.0.0/pubnub/endpoints/presence/here_now.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/presence/leave.py` & `pubnub-8.0.0/pubnub/endpoints/presence/leave.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/presence/set_state.py` & `pubnub-8.0.0/pubnub/endpoints/presence/set_state.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/presence/where_now.py` & `pubnub-8.0.0/pubnub/endpoints/presence/where_now.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/pubsub/fire.py` & `pubnub-8.0.0/pubnub/endpoints/pubsub/fire.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/pubsub/publish.py` & `pubnub-8.0.0/pubnub/endpoints/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/pubsub/subscribe.py` & `pubnub-8.0.0/pubnub/endpoints/pubsub/subscribe.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/push/add_channels_to_push.py` & `pubnub-8.0.0/pubnub/endpoints/push/add_channels_to_push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/push/list_push_provisions.py` & `pubnub-8.0.0/pubnub/endpoints/push/list_push_provisions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/push/remove_channels_from_push.py` & `pubnub-8.0.0/pubnub/endpoints/push/remove_channels_from_push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/push/remove_device.py` & `pubnub-8.0.0/pubnub/endpoints/push/remove_device.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/signal.py` & `pubnub-8.0.0/pubnub/endpoints/signal.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/endpoints/time.py` & `pubnub-8.0.0/pubnub/endpoints/time.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/enums.py` & `pubnub-8.0.0/pubnub/enums.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/errors.py` & `pubnub-8.0.0/pubnub/errors.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/event_engine/containers.py` & `pubnub-8.0.0/pubnub/event_engine/containers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/event_engine/dispatcher.py` & `pubnub-8.0.0/pubnub/event_engine/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/event_engine/effects.py` & `pubnub-8.0.0/pubnub/event_engine/effects.py`

 * *Files 5% similar despite different names*

```diff
@@ -269,16 +269,17 @@
 
     def get_timetoken(self):
         return int(self.invocation.timetoken)
 
 
 class HeartbeatEffect(Effect):
     def run(self):
-        channels = self.invocation.channels
-        groups = self.invocation.groups
+        channels = list(filter(lambda ch: not ch.endswith('-pnpres'), self.invocation.channels))
+        groups = list(filter(lambda gr: not gr.endswith('-pnpres'), self.invocation.groups))
+
         if hasattr(self.pubnub, 'event_loop'):
             self.stop_event = self.get_new_stop_event()
             self.run_async(self.heartbeat(channels=channels, groups=groups, stop_event=self.stop_event))
 
     async def heartbeat(self, channels, groups, stop_event):
         request = Heartbeat(self.pubnub).channels(channels).channel_groups(groups).cancellation_event(stop_event)
 
@@ -358,14 +359,18 @@
 
     async def heartbeat(self, channels, groups, attempt, stop_event):
         if self.reconnection_policy is PNReconnectionPolicy.NONE or self.invocation.attempts > self.max_retry_attempts:
             self.event_engine.trigger(events.HeartbeatGiveUpEvent(channels=self.invocation.channels,
                                                                   groups=self.invocation.groups,
                                                                   reason=self.invocation.reason,
                                                                   attempt=self.invocation.attempts))
+
+        channels = list(filter(lambda ch: not ch.endswith('-pnpres'), self.invocation.channels))
+        groups = list(filter(lambda gr: not gr.endswith('-pnpres'), self.invocation.groups))
+
         request = Heartbeat(self.pubnub).channels(channels).channel_groups(groups).cancellation_event(stop_event)
         delay = self.calculate_reconnection_delay(attempt)
         self.logger.warning(f'Will retry to Heartbeat in {delay}s')
         await asyncio.sleep(delay)
 
         response = await request.future()
         if isinstance(response, PubNubException):
```

### Comparing `pubnub-7.4.4/pubnub/event_engine/models/events.py` & `pubnub-8.0.0/pubnub/event_engine/models/events.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/event_engine/models/invocations.py` & `pubnub-8.0.0/pubnub/event_engine/models/invocations.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/event_engine/models/states.py` & `pubnub-8.0.0/pubnub/event_engine/models/states.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,18 +978,20 @@
             state=HeartbeatingState,
             context=self._context
         )
 
     def left(self, event: events.HeartbeatLeftEvent, context: PNContext) -> PNTransition:
         self._context.update(context)
         for channel in event.channels:
-            self._context.channels.remove(channel)
+            if channel in self._context.channels:
+                self._context.channels.remove(channel)
 
         for group in event.groups:
-            self._context.groups.remove(group)
+            if group in self._context.groups:
+                self._context.groups.remove(group) or None
 
         invocation = None
         if not event.suppress_leave:
             invocation = invocations.HeartbeatLeaveInvocation(channels=event.channels,
                                                               groups=event.groups)
 
         return PNTransition(
```

### Comparing `pubnub-7.4.4/pubnub/event_engine/statemachine.py` & `pubnub-8.0.0/pubnub/event_engine/statemachine.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/exceptions.py` & `pubnub-8.0.0/pubnub/exceptions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/features.py` & `pubnub-8.0.0/pubnub/features.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/managers.py` & `pubnub-8.0.0/pubnub/managers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/access_manager.py` & `pubnub-8.0.0/pubnub/models/consumer/access_manager.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/channel_group.py` & `pubnub-8.0.0/pubnub/models/consumer/channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/common.py` & `pubnub-8.0.0/pubnub/models/consumer/common.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/entities/membership.py` & `pubnub-8.0.0/pubnub/models/consumer/entities/membership.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/entities/page.py` & `pubnub-8.0.0/pubnub/models/consumer/entities/page.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/entities/space.py` & `pubnub-8.0.0/pubnub/models/consumer/entities/space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/entities/user.py` & `pubnub-8.0.0/pubnub/models/consumer/entities/user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/file.py` & `pubnub-8.0.0/pubnub/models/consumer/file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/history.py` & `pubnub-8.0.0/pubnub/models/consumer/history.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/message_actions.py` & `pubnub-8.0.0/pubnub/models/consumer/message_actions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel.py` & `pubnub-8.0.0/pubnub/models/consumer/objects_v2/channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/objects_v2/channel_members.py` & `pubnub-8.0.0/pubnub/models/consumer/objects_v2/channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/objects_v2/memberships.py` & `pubnub-8.0.0/pubnub/models/consumer/objects_v2/memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/objects_v2/page.py` & `pubnub-8.0.0/pubnub/models/consumer/objects_v2/page.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/objects_v2/sort.py` & `pubnub-8.0.0/pubnub/models/consumer/objects_v2/sort.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/objects_v2/uuid.py` & `pubnub-8.0.0/pubnub/models/consumer/objects_v2/uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/presence.py` & `pubnub-8.0.0/pubnub/models/consumer/presence.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/pubsub.py` & `pubnub-8.0.0/pubnub/models/consumer/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,18 @@
         self.channel = channel
 
         self.timetoken = timetoken
         self.user_metadata = user_metadata
 
 
 class PNMessageActionResult(PNMessageAction):
-
-    def __init__(self, result):
+    def __init__(self, result, *, subscription=None, channel=None):
         super(PNMessageActionResult, self).__init__(result)
+        self.subscription = subscription
+        self.channel = channel
 
 
 class PNPublishResult(object):
     def __init__(self, envelope, timetoken):
         """
         Representation of publish server response
```

### Comparing `pubnub-7.4.4/pubnub/models/consumer/push.py` & `pubnub-8.0.0/pubnub/models/consumer/push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/time.py` & `pubnub-8.0.0/pubnub/models/consumer/time.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/access_manager.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/access_manager.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/channel.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/group.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/pn_resource.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/pn_resource.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/space.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/user.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/consumer/v3/uuid.py` & `pubnub-8.0.0/pubnub/models/consumer/v3/uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/models/server/subscribe.py` & `pubnub-8.0.0/pubnub/models/server/subscribe.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/pnconfiguration.py` & `pubnub-8.0.0/pubnub/pnconfiguration.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/pubnub.py` & `pubnub-8.0.0/pubnub/pubnub.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
             # TODO: handle the exception
             pass
         finally:
             self._schedule_next()
 
     def _schedule_next(self):
         self._timeout = threading.Timer(self._callback_time, self._run)
-        self._timer.daemon = True
+        self._timeout.daemon = True
         self._timeout.start()
 
 
 class NativeSubscribeMessageWorker(SubscribeMessageWorker):
     def _take_message(self):
         while not self._event.is_set():
             try:
```

### Comparing `pubnub-7.4.4/pubnub/pubnub_asyncio.py` & `pubnub-8.0.0/pubnub/pubnub_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from pubnub.models.consumer.common import PNStatus
 from pubnub.dtos import SubscribeOperation, UnsubscribeOperation
 from pubnub.event_engine.statemachine import StateMachine
 from pubnub.endpoints.presence.heartbeat import Heartbeat
 from pubnub.endpoints.presence.leave import Leave
 from pubnub.endpoints.pubsub.subscribe import Subscribe
-from pubnub.features import feature_enabled
 from pubnub.pubnub_core import PubNubCore
 from pubnub.workers import SubscribeMessageWorker
 from pubnub.managers import SubscriptionManager, PublishSequenceManager, ReconnectionManager, TelemetryManager
 from pubnub import utils
 from pubnub.structures import ResponseInfo, RequestOptions
 from pubnub.enums import PNStatusCategory, PNHeartbeatNotificationOptions, PNOperationType, PNReconnectionPolicy
 from pubnub.callbacks import SubscribeCallback, ReconnectionCallback
@@ -45,17 +44,15 @@
 
         self._connector = None
         self._session = None
 
         self._connector = aiohttp.TCPConnector(verify_ssl=True, loop=self.event_loop)
 
         if not subscription_manager:
-            subscription_manager = (
-                EventEngineSubscriptionManager if feature_enabled('PN_ENABLE_EVENT_ENGINE')
-                else AsyncioSubscriptionManager)
+            subscription_manager = EventEngineSubscriptionManager
 
         if self.config.enable_subscribe:
             self._subscription_manager = subscription_manager(self)
 
         self._publish_sequence_manager = AsyncioPublishSequenceManager(self.event_loop, PubNubCore.MAX_SEQUENCE)
 
         self._telemetry_manager = AsyncioTelemetryManager()
@@ -175,15 +172,14 @@
 
         if options.use_base_path:
             url = utils.build_url(self.config.scheme(), self.base_origin, options.path, options.query_string)
         else:
             url = utils.build_url(scheme="", origin="", path=options.path, params=options.query_string)
 
         url = URL(url, encoded=True)
-
         logger.debug("%s %s %s" % (options.method_string, url, options.data))
 
         if options.request_headers:
             request_headers = {**self.headers, **options.request_headers}
         else:
             request_headers = self.headers
 
@@ -562,14 +558,15 @@
         self.event_engine = StateMachine(states.UnsubscribedState,
                                          name="subscribe")
         self.presence_engine = StateMachine(states.HeartbeatInactiveState,
                                             name="presence")
         self.event_engine.get_dispatcher().set_pn(pubnub_instance)
         self.presence_engine.get_dispatcher().set_pn(pubnub_instance)
         self.loop = asyncio.new_event_loop()
+        self._heartbeat_periodic_callback = None
         pubnub_instance.state_container = self.state_container
         super().__init__(pubnub_instance)
 
     def stop(self):
         self.event_engine.stop()
         self.presence_engine.stop()
 
@@ -589,39 +586,35 @@
                 channels=subscribe_operation.channels_with_pressence,
                 groups=subscribe_operation.groups_with_pressence,
                 with_presence=subscribe_operation.presence_enabled
             )
         self.event_engine.trigger(subscription_event)
         if self._pubnub.config.enable_presence_heartbeat and self._pubnub.config._heartbeat_interval > 0:
             self.presence_engine.trigger(events.HeartbeatJoinedEvent(
-                channels=subscribe_operation.channels,
-                groups=subscribe_operation.channel_groups
+                channels=subscribe_operation.channels_without_presence,
+                groups=subscribe_operation.channel_groups_without_presence
             ))
 
     def adapt_unsubscribe_builder(self, unsubscribe_operation):
         if not isinstance(unsubscribe_operation, UnsubscribeOperation):
             raise PubNubException('Invalid Unsubscribe Operation')
 
-        channels = unsubscribe_operation.get_subscribed_channels(
-            self.event_engine.get_context().channels,
-            self.event_engine.get_context().with_presence)
-
-        groups = unsubscribe_operation.get_subscribed_channel_groups(
-            self.event_engine.get_context().groups,
-            self.event_engine.get_context().with_presence)
+        channels = unsubscribe_operation.get_subscribed_channels(self.event_engine.get_context().channels)
+
+        groups = unsubscribe_operation.get_subscribed_channel_groups(self.event_engine.get_context().groups)
 
         if channels or groups:
             self.event_engine.trigger(events.SubscriptionChangedEvent(channels=channels, groups=groups))
         else:
             self.event_engine.trigger(events.UnsubscribeAllEvent())
 
         if self._pubnub.config.enable_presence_heartbeat and self._pubnub.config._heartbeat_interval > 0:
             self.presence_engine.trigger(event=events.HeartbeatLeftEvent(
-                channels=unsubscribe_operation.channels,
-                groups=unsubscribe_operation.channel_groups,
+                channels=unsubscribe_operation.channels_without_presence,
+                groups=unsubscribe_operation.channel_groups_without_presence,
                 suppress_leave=self._pubnub.config.suppress_leave_events
             ))
 
     def adapt_state_builder(self, state_operation):
         self.state_container.register_state(state_operation.state,
                                             state_operation.channels)
         return super().adapt_state_builder(state_operation)
```

### Comparing `pubnub-7.4.4/pubnub/pubnub_core.py` & `pubnub-8.0.0/pubnub/pubnub_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from pubnub.endpoints.entities.user.update_user import UpdateUser
 from pubnub.endpoints.entities.user.fetch_user import FetchUser
 from pubnub.endpoints.entities.user.fetch_users import FetchUsers
 from pubnub.errors import PNERR_MISUSE_OF_USER_AND_SPACE, PNERR_USER_SPACE_PAIRS_MISSING
 from pubnub.exceptions import PubNubException
 from pubnub.features import feature_flag
 from pubnub.crypto import PubNubCryptoModule
+from pubnub.models.subscription import PubNubChannel, PubNubChannelGroup, PubNubChannelMetadata, PubNubUserMetadata, \
+    PNSubscriptionRegistry, PubNubSubscriptionSet
 
 from abc import ABCMeta, abstractmethod
 
 from .endpoints.objects_v2.uuid.set_uuid import SetUuid
 from .endpoints.objects_v2.channel.get_all_channels import GetAllChannels
 from .endpoints.objects_v2.channel.get_channel import GetChannel
 from .endpoints.objects_v2.channel.remove_channel import RemoveChannel
@@ -81,35 +83,38 @@
 from .managers import TelemetryManager
 
 logger = logging.getLogger("pubnub")
 
 
 class PubNubCore:
     """A base class for PubNub Python API implementations"""
-    SDK_VERSION = "7.4.4"
+    SDK_VERSION = "8.0.0"
     SDK_NAME = "PubNub-Python"
 
     TIMESTAMP_DIVIDER = 1000
     MAX_SEQUENCE = 65535
 
     __metaclass__ = ABCMeta
     __crypto = None
 
+    _subscription_registry: PNSubscriptionRegistry
+
     def __init__(self, config):
         self.config = config
         self.config.validate()
         self.headers = {
             'User-Agent': self.sdk_name
         }
 
         self._subscription_manager = None
         self._publish_sequence_manager = None
         self._telemetry_manager = TelemetryManager()
         self._base_path_manager = BasePathManager(config)
         self._token_manager = TokenManager()
+        self._subscription_registry = PNSubscriptionRegistry(self)
 
     @property
     def base_origin(self):
         return self._base_path_manager.get_base_path()
 
     @property
     def sdk_name(self):
@@ -160,24 +165,24 @@
     def list_channels_in_channel_group(self):
         return ListChannelsInChannelGroup(self)
 
     def remove_channel_group(self):
         return RemoveChannelGroup(self)
 
     def subscribe(self):
-        return SubscribeBuilder(self._subscription_manager)
+        return SubscribeBuilder(self)
 
     def unsubscribe(self):
-        return UnsubscribeBuilder(self._subscription_manager)
+        return UnsubscribeBuilder(self)
 
     def unsubscribe_all(self):
-        return self._subscription_manager.unsubscribe_all()
+        return self._subscription_registry.unsubscribe_all()
 
     def reconnect(self):
-        return self._subscription_manager.reconnect()
+        return self._subscription_registry.reconnect()
 
     def heartbeat(self):
         return Heartbeat(self)
 
     def set_state(self):
         return SetState(self, self._subscription_manager)
 
@@ -636,7 +641,22 @@
 
         if include_custom:
             memberships.include_custom(include_custom)
 
         if sync:
             return memberships.sync()
         return memberships
+
+    def channel(self, channel) -> PubNubChannel:
+        return PubNubChannel(self, channel)
+
+    def channel_group(self, channel_group) -> PubNubChannelGroup:
+        return PubNubChannelGroup(self, channel_group)
+
+    def channel_metadata(self, channel) -> PubNubChannelMetadata:
+        return PubNubChannelMetadata(self, channel)
+
+    def user_metadata(self, user_id) -> PubNubUserMetadata:
+        return PubNubUserMetadata(self, user_id)
+
+    def subscription_set(self, subscriptions: list) -> PubNubSubscriptionSet:
+        return PubNubSubscriptionSet(self, subscriptions)
```

### Comparing `pubnub-7.4.4/pubnub/request_handlers/requests_handler.py` & `pubnub-8.0.0/pubnub/request_handlers/requests_handler.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,27 +51,27 @@
         def callback_to_invoke_in_separate_thread():
             try:
                 envelope = self._build_envelope(platform_options, endpoint_call_options)
                 if cancellation_event is not None and cancellation_event.is_set():
                     # Since there are no way to affect on ongoing request it's response will
                     # be just ignored on cancel call
                     return
-
                 callback(envelope)
             except PubNubException as e:
                 logger.error("Async request PubNubException. %s" % str(e))
                 callback(Envelope(
                     result=None,
                     status=endpoint_call_options.create_status(
                         category=PNStatusCategory.PNBadRequestCategory,
                         response=None,
                         response_info=None,
                         exception=e)))
             except Exception as e:
                 logger.error("Async request Exception. %s" % str(e))
+
                 callback(Envelope(
                     result=None,
                     status=endpoint_call_options.create_status(
                         category=PNStatusCategory.PNInternalExceptionCategory,
                         response=None,
                         response_info=None,
                         exception=e)))
```

### Comparing `pubnub-7.4.4/pubnub/structures.py` & `pubnub-8.0.0/pubnub/structures.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/utils.py` & `pubnub-8.0.0/pubnub/utils.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.4.4/pubnub/workers.py` & `pubnub-8.0.0/pubnub/workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,16 +187,16 @@
                 self.announce(pn_signal_result)
                 return pn_signal_result
 
             elif message.type == SubscribeMessageWorker.TYPE_MESSAGE_ACTION:
                 message_action = extracted_message['data']
                 if 'uuid' not in message_action:
                     message_action['uuid'] = publisher
-
-                message_action_result = PNMessageActionResult(message_action)
+                message_action_result = PNMessageActionResult(message_action, subscription=subscription_match,
+                                                              channel=channel)
                 self._listener_manager.announce_message_action(message_action_result)
 
             else:
                 pn_message_result = PNMessageResult(
                     message=extracted_message,
                     channel=channel,
                     subscription=subscription_match,
```

### Comparing `pubnub-7.4.4/pubnub.egg-info/PKG-INFO` & `pubnub-8.0.0/pubnub.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubnub
-Version: 7.4.4
+Version: 8.0.0
 Summary: PubNub Real-time push service in the cloud
 Home-page: http://pubnub.com
 Author: PubNub
 Author-email: support@pubnub.com
 License: PubNub Software Development Kit License
 Project-URL: Source, https://github.com/pubnub/python
 Project-URL: Documentation, https://www.pubnub.com/docs/sdks/python
```

### Comparing `pubnub-7.4.4/pubnub.egg-info/SOURCES.txt` & `pubnub-8.0.0/pubnub.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,15 @@
 pubnub/event_engine/effects.py
 pubnub/event_engine/statemachine.py
 pubnub/event_engine/models/__init__.py
 pubnub/event_engine/models/events.py
 pubnub/event_engine/models/invocations.py
 pubnub/event_engine/models/states.py
 pubnub/models/__init__.py
+pubnub/models/subscription.py
 pubnub/models/subscription_item.py
 pubnub/models/consumer/__init__.py
 pubnub/models/consumer/access_manager.py
 pubnub/models/consumer/channel_group.py
 pubnub/models/consumer/common.py
 pubnub/models/consumer/file.py
 pubnub/models/consumer/history.py
```

### Comparing `pubnub-7.4.4/setup.py` & `pubnub-8.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pubnub',
-    version='7.4.4',
+    version='8.0.0',
     description='PubNub Real-time push service in the cloud',
     author='PubNub',
     author_email='support@pubnub.com',
     url='http://pubnub.com',
     project_urls={
         'Source': 'https://github.com/pubnub/python',
         'Documentation': 'https://www.pubnub.com/docs/sdks/python',
```


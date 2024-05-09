# Comparing `tmp/airbyte_source_zendesk_support-2.6.3.dev202405091551.tar.gz` & `tmp/airbyte_source_zendesk_support-2.6.3.dev202405091700.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zendesk_support-2.6.3.dev202405091551.tar", max compression
+gzip compressed data, was "airbyte_source_zendesk_support-2.6.3.dev202405091700.tar", max compression
```

## Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551.tar` & `airbyte_source_zendesk_support-2.6.3.dev202405091700.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     4673 2024-05-09 15:48:21.770190 airbyte_source_zendesk_support-2.6.3.dev202405091551/README.md
--rw-r--r--   0        0        0      852 2024-05-09 15:52:10.967524 airbyte_source_zendesk_support-2.6.3.dev202405091551/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/__init__.py
--rw-r--r--   0        0        0     3294 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/components.py
--rw-r--r--   0        0        0    19960 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/manifest.yaml
--rw-r--r--   0        0        0      255 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/run.py
--rw-r--r--   0        0        0      798 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/account_attributes.json
--rw-r--r--   0        0        0     2103 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/article_comments.json
--rw-r--r--   0        0        0     3577 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/articles.json
--rw-r--r--   0        0        0     3046 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/attribute_definitions.json
--rw-r--r--   0        0        0     1741 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/audit_logs.json
--rw-r--r--   0        0        0     2061 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/brands.json
--rw-r--r--   0        0        0     9569 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/custom_roles.json
--rw-r--r--   0        0        0     1211 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/deleted_tickets.json
--rw-r--r--   0        0        0     1098 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/group_memberships.json
--rw-r--r--   0        0        0     1211 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/groups.json
--rw-r--r--   0        0        0     2642 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/macros.json
--rw-r--r--   0        0        0     2659 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/organization_fields.json
--rw-r--r--   0        0        0     1453 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/organization_memberships.json
--rw-r--r--   0        0        0     2262 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/organizations.json
--rw-r--r--   0        0        0     1978 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/post_comments.json
--rw-r--r--   0        0        0     3315 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/posts.json
--rw-r--r--   0        0        0     1843 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/satisfaction_ratings.json
--rw-r--r--   0        0        0     1239 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/schedules.json
--rw-r--r--   0        0        0     1958 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/attachments.json
--rw-r--r--   0        0        0     1835 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/metadata.json
--rw-r--r--   0        0        0     4521 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/tickets.json
--rw-r--r--   0        0        0     1617 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/via.json
--rw-r--r--   0        0        0     2707 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/via_channel.json
--rw-r--r--   0        0        0     3655 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/sla_policies.json
--rw-r--r--   0        0        0      320 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/tags.json
--rw-r--r--   0        0        0     2114 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_activities.json
--rw-r--r--   0        0        0    29608 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_audits.json
--rw-r--r--   0        0        0     2495 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_comments.json
--rw-r--r--   0        0        0     4685 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_fields.json
--rw-r--r--   0        0        0     2644 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_forms.json
--rw-r--r--   0        0        0      855 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_metric_events.json
--rw-r--r--   0        0        0     7095 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_metrics.json
--rw-r--r--   0        0        0     1013 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_skips.json
--rw-r--r--   0        0        0       27 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/tickets.json
--rw-r--r--   0        0        0     1735 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/topics.json
--rw-r--r--   0        0        0     2182 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/user_fields.json
--rw-r--r--   0        0        0     8484 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/users.json
--rw-r--r--   0        0        0     1170 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/votes.json
--rw-r--r--   0        0        0     7876 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/source.py
--rw-r--r--   0        0        0     5975 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/spec.json
--rw-r--r--   0        0        0    39231 2024-05-09 15:48:21.774190 airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/streams.py
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.3.dev202405091551/PKG-INFO
+-rw-r--r--   0        0        0     4673 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/README.md
+-rw-r--r--   0        0        0      852 2024-05-09 17:00:35.007211 airbyte_source_zendesk_support-2.6.3.dev202405091700/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/__init__.py
+-rw-r--r--   0        0        0     3294 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/components.py
+-rw-r--r--   0        0        0    19960 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/manifest.yaml
+-rw-r--r--   0        0        0      255 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/run.py
+-rw-r--r--   0        0        0      798 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/account_attributes.json
+-rw-r--r--   0        0        0     2103 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/article_comments.json
+-rw-r--r--   0        0        0     3577 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/articles.json
+-rw-r--r--   0        0        0     3046 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/attribute_definitions.json
+-rw-r--r--   0        0        0     1741 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/audit_logs.json
+-rw-r--r--   0        0        0     2061 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/brands.json
+-rw-r--r--   0        0        0     9569 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/custom_roles.json
+-rw-r--r--   0        0        0     1211 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/deleted_tickets.json
+-rw-r--r--   0        0        0     1098 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/group_memberships.json
+-rw-r--r--   0        0        0     1211 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/groups.json
+-rw-r--r--   0        0        0     2642 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/macros.json
+-rw-r--r--   0        0        0     2659 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/organization_fields.json
+-rw-r--r--   0        0        0     1453 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/organization_memberships.json
+-rw-r--r--   0        0        0     2262 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/organizations.json
+-rw-r--r--   0        0        0     1978 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/post_comments.json
+-rw-r--r--   0        0        0     3315 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/posts.json
+-rw-r--r--   0        0        0     1843 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/satisfaction_ratings.json
+-rw-r--r--   0        0        0     1239 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/schedules.json
+-rw-r--r--   0        0        0     1958 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/attachments.json
+-rw-r--r--   0        0        0     1835 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/metadata.json
+-rw-r--r--   0        0        0     4521 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/tickets.json
+-rw-r--r--   0        0        0     1617 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/via.json
+-rw-r--r--   0        0        0     2707 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/via_channel.json
+-rw-r--r--   0        0        0     3655 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/sla_policies.json
+-rw-r--r--   0        0        0      320 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/tags.json
+-rw-r--r--   0        0        0     2114 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_activities.json
+-rw-r--r--   0        0        0    29608 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_audits.json
+-rw-r--r--   0        0        0     2495 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_comments.json
+-rw-r--r--   0        0        0     4685 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_fields.json
+-rw-r--r--   0        0        0     2644 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_forms.json
+-rw-r--r--   0        0        0      855 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_metric_events.json
+-rw-r--r--   0        0        0     7095 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_metrics.json
+-rw-r--r--   0        0        0     1013 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_skips.json
+-rw-r--r--   0        0        0       27 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/tickets.json
+-rw-r--r--   0        0        0     1735 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/topics.json
+-rw-r--r--   0        0        0     2182 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/user_fields.json
+-rw-r--r--   0        0        0     8484 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/users.json
+-rw-r--r--   0        0        0     1170 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/votes.json
+-rw-r--r--   0        0        0     7876 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/source.py
+-rw-r--r--   0        0        0     5975 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/spec.json
+-rw-r--r--   0        0        0    39231 2024-05-09 15:48:21.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/streams.py
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 airbyte_source_zendesk_support-2.6.3.dev202405091700/PKG-INFO
```

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/README.md` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/pyproject.toml` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.6.3.dev202405091551"
+version = "2.6.3.dev202405091700"
 name = "airbyte-source-zendesk-support"
 description = "Source implementation for Zendesk Support."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/__init__.py` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/components.py` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/manifest.yaml` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/account_attributes.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/account_attributes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/article_comments.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/article_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/articles.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/attribute_definitions.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/attribute_definitions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/audit_logs.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/audit_logs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/brands.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/brands.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/custom_roles.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/custom_roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/deleted_tickets.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/deleted_tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/group_memberships.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/groups.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/macros.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/organization_fields.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/organization_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/organization_memberships.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/organization_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/organizations.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/post_comments.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/post_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/posts.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/posts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/satisfaction_ratings.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/schedules.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/schedules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/attachments.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/metadata.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/tickets.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/via.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/shared/via_channel.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/shared/via_channel.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/sla_policies.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_activities.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_activities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_audits.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_comments.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_fields.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_forms.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_metric_events.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_metric_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_metrics.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/ticket_skips.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/ticket_skips.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/topics.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/topics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/user_fields.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/user_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/users.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/schemas/votes.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/schemas/votes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/source.py` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/spec.json` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/source_zendesk_support/streams.py` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/source_zendesk_support/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zendesk_support-2.6.3.dev202405091551/PKG-INFO` & `airbyte_source_zendesk_support-2.6.3.dev202405091700/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zendesk-support
-Version: 2.6.3.dev202405091551
+Version: 2.6.3.dev202405091700
 Summary: Source implementation for Zendesk Support.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```


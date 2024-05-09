# Comparing `tmp/onnxscript-0.1.0.dev20240507.tar.gz` & `tmp/onnxscript-0.1.0.dev20240508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240507.tar", last modified: Tue May  7 00:01:17 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240508.tar", last modified: Wed May  8 00:01:06 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240507.tar` & `onnxscript-0.1.0.dev20240508.tar`

### file list

```diff
@@ -1,218 +1,220 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.815414 onnxscript-0.1.0.dev20240507/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.775413 onnxscript-0.1.0.dev20240507/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.775413 onnxscript-0.1.0.dev20240507/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.775413 onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.779414 onnxscript-0.1.0.dev20240507/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.779414 onnxscript-0.1.0.dev20240507/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.767413 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.779414 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.771413 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.767413 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.791414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.795414 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.799414 onnxscript-0.1.0.dev20240507/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2619 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    87244 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20616 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/_type_casting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    52805 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.799414 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.807414 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.807414 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6405 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29763 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34531 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-07 00:01:17.811414 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8193 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-07 00:01:17.000000 onnxscript-0.1.0.dev20240507/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-07 00:01:17.815414 onnxscript-0.1.0.dev20240507/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-07 00:00:56.000000 onnxscript-0.1.0.dev20240507/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.847479 onnxscript-0.1.0.dev20240508/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.819479 onnxscript-0.1.0.dev20240508/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.823479 onnxscript-0.1.0.dev20240508/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.823479 onnxscript-0.1.0.dev20240508/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.823479 onnxscript-0.1.0.dev20240508/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.823479 onnxscript-0.1.0.dev20240508/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.819479 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.823479 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.831479 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.819479 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.819479 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.831479 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.831479 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.831479 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.835479 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.835479 onnxscript-0.1.0.dev20240508/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2619 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    90076 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20685 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/_type_casting.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    55672 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.835479 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.839479 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6718 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      755 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29763 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2140 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/bfloat16_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34531 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 00:01:06.843479 onnxscript-0.1.0.dev20240508/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10854 2024-05-08 00:01:06.000000 onnxscript-0.1.0.dev20240508/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-05-08 00:01:06.000000 onnxscript-0.1.0.dev20240508/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 00:01:06.000000 onnxscript-0.1.0.dev20240508/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-08 00:01:06.000000 onnxscript-0.1.0.dev20240508/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-08 00:01:06.000000 onnxscript-0.1.0.dev20240508/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-08 00:01:06.847479 onnxscript-0.1.0.dev20240508/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-08 00:00:44.000000 onnxscript-0.1.0.dev20240508/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240507/LICENSE` & `onnxscript-0.1.0.dev20240508/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/PKG-INFO` & `onnxscript-0.1.0.dev20240508/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240507
+Version: 0.1.0.dev20240508
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240507/README.md` & `onnxscript-0.1.0.dev20240508/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240508/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240508/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240508/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240508/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240508/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240508/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_convenience.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     Sequence[int],
     Sequence[float],
     Sequence[str],
     _protocols.TensorProtocol,  # This includes all in-memory tensor types
     onnx.TensorProto,
     _core.Attr,
     _core.RefAttr,
+    _protocols.GraphProtocol,
+    Sequence[_protocols.GraphProtocol],
+    _protocols.TypeProtocol,
+    Sequence[_protocols.TypeProtocol],
     None,
 ]
 
 
 def _infer_attribute_type(attr: SupportedAttrTypes) -> _enums.AttributeType:
     """Infer the attribute type based on the type of the Python object."""
     if isinstance(attr, int):
@@ -52,14 +56,38 @@
     if isinstance(attr, Sequence) and all(isinstance(x, float) for x in attr):
         return _enums.AttributeType.FLOATS
     if isinstance(attr, Sequence) and all(isinstance(x, str) for x in attr):
         return _enums.AttributeType.STRINGS
     if isinstance(attr, (_core.TensorBase, onnx.TensorProto, _protocols.TensorProtocol)):
         # Be sure to check TensorProtocol last because isinstance checking on Protocols can be slower
         return _enums.AttributeType.TENSOR
+    if isinstance(attr, (_core.Graph, _protocols.GraphProtocol)):
+        return _enums.AttributeType.GRAPH
+    if isinstance(attr, Sequence) and all(
+        isinstance(x, (_core.Graph, _protocols.GraphProtocol)) for x in attr
+    ):
+        return _enums.AttributeType.GRAPHS
+    if isinstance(
+        attr,
+        (_core.TensorType, _core.SequenceType, _core.OptionalType, _protocols.TypeProtocol),
+    ):
+        return _enums.AttributeType.TYPE_PROTO
+    if isinstance(attr, Sequence) and all(
+        isinstance(
+            x,
+            (
+                _core.TensorType,
+                _core.SequenceType,
+                _core.OptionalType,
+                _protocols.TypeProtocol,
+            ),
+        )
+        for x in attr
+    ):
+        return _enums.AttributeType.TYPE_PROTOS
     raise TypeError(f"Unsupported attribute type: '{type(attr)}'")
 
 
 def convert_attribute(
     name: str,
     attr: SupportedAttrTypes,
     attr_type: _enums.AttributeType | None = None,
@@ -114,14 +142,22 @@
     if attr_type == _enums.AttributeType.STRINGS:
         return _core.AttrStrings(name, attr)  # type: ignore
     if attr_type == _enums.AttributeType.TENSOR:
         if isinstance(attr, (_core.TensorBase, _protocols.TensorProtocol)):
             return _core.AttrTensor(name, attr)
         if isinstance(attr, onnx.TensorProto):
             return _core.AttrTensor(name, serde.TensorProtoTensor(attr))
+    if attr_type == _enums.AttributeType.GRAPH:
+        return _core.AttrGraph(name, attr)  # type: ignore[arg-type]
+    if attr_type == _enums.AttributeType.GRAPHS:
+        return _core.AttrGraphs(name, attr)  # type: ignore[arg-type]
+    if attr_type == _enums.AttributeType.TYPE_PROTO:
+        return _core.AttrTypeProto(name, attr)  # type: ignore[arg-type]
+    if attr_type == _enums.AttributeType.TYPE_PROTOS:
+        return _core.AttrTypeProtos(name, attr)  # type: ignore[arg-type]
     raise TypeError(f"Unsupported attribute type: '{type(attr)}'")
 
 
 def convert_attributes(
     attrs: Mapping[str, SupportedAttrTypes],
 ) -> list[_core.Attr | _core.RefAttr]:
     """Convert a dictionary of attributes to a list of _core.Attr objects.
@@ -144,17 +180,48 @@
         ...     "tensor_proto":
         ...         onnx.TensorProto(
         ...             dims=[3],
         ...             data_type=onnx.TensorProto.FLOAT,
         ...             float_data=[1.0, 2.0, 3.0],
         ...             name="proto",
         ...         ),
+        ...     "graph": ir.Graph([], [], nodes=[], name="graph0"),
+        ...     "graphs": [ir.Graph([], [], nodes=[], name="graph1"), ir.Graph([], [], nodes=[], name="graph2")],
+        ...     "type_proto": ir.TensorType(ir.DataType.FLOAT),
+        ...     "type_protos": [ir.TensorType(ir.DataType.FLOAT), ir.TensorType(ir.DataType.FLOAT)],
         ... }
         >>> convert_attributes(attrs)
-        [AttrInt64('int', 1), AttrFloat32('float', 1.0), AttrString('str', 'hello'), AttrInt64s('ints', [1, 2, 3]), AttrFloat32s('floats', [1.0, 2.0, 3.0]), AttrStrings('strings', ['hello', 'world']), AttrTensor('tensor', Tensor<DOUBLE,[3]>(array([1., 2., 3.]), name='')), AttrTensor('tensor_proto', TensorProtoTensor<FLOAT,[3]>(name='proto'))]
+        [AttrInt64('int', 1), AttrFloat32('float', 1.0), AttrString('str', 'hello'), AttrInt64s('ints', [1, 2, 3]), AttrFloat32s('floats', [1.0, 2.0, 3.0]), AttrStrings('strings', ['hello', 'world']), AttrTensor('tensor', Tensor<DOUBLE,[3]>(array([1., 2., 3.]), name='')), AttrTensor('tensor_proto', TensorProtoTensor<FLOAT,[3]>(name='proto')), AttrInt64s('graph', Graph(
+            name='graph0',
+            inputs=(
+        <BLANKLINE>
+            ),
+            outputs=(
+        <BLANKLINE>
+            ),
+            len()=0
+        )), AttrGraphs('graphs', [Graph(
+            name='graph1',
+            inputs=(
+        <BLANKLINE>
+            ),
+            outputs=(
+        <BLANKLINE>
+            ),
+            len()=0
+        ), Graph(
+            name='graph2',
+            inputs=(
+        <BLANKLINE>
+            ),
+            outputs=(
+        <BLANKLINE>
+            ),
+            len()=0
+        )]), AttrTypeProto('type_proto', Tensor(FLOAT)), AttrTypeProtos('type_protos', [Tensor(FLOAT), Tensor(FLOAT)])]
 
     Args:
         attrs: A dictionary of {<attribute name>: <python objects>} to convert.
 
     Returns:
         A list of _core.Attr objects.
     """
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,48 +897,54 @@
         self,
         domain: str,
         op_type: str,
         inputs: Iterable[Value | None],
         attributes: Iterable[Attr | RefAttr] = (),
         *,
         overload: str = "",
-        num_outputs: int = 1,
+        num_outputs: int | None = None,
+        outputs: Sequence[Value] | None = None,
         version: int | None = None,
         graph: Graph | None = None,
         name: str | None = None,
         doc_string: str | None = None,
         metadata_props: dict[str, str] | None = None,
     ):
         """Initialize a node and add it as a user of the input values.
 
         Args:
             domain: The domain of the operator. For onnx operators, this is an empty string.
             op_type: The name of the operator.
             inputs: The input values. When an input is None, it is an empty input.
             attributes: The attributes. RefAttr can be used only when the node is defined in a Function.
             overload: The overload name when the node is invoking a function.
-            num_outputs: The number of outputs of the node.
+            num_outputs: The number of outputs of the node. If not specified, the number is 1.
+            outputs: The output values. If None, the outputs are created during initialization.
             version: The version of the operator. If None, the version is unspecified and will follow that of the graph.
             graph: The graph that the node belongs to. If None, the node is not added to any graph.
                 A `Node` must belong to zero or one graph.
             name: The name of the node. If None, the node is anonymous.
             doc_string: The documentation string.
             metadata_props: The metadata properties.
+
+        Raises:
+            TypeError: If the attributes are not Attr or RefAttr.
+            ValueError: If `num_outputs`, when not None, is not the same as the length of the outputs.
+            ValueError: If an output value is None, when outputs is specified.
+            ValueError: If an output value has a producer set already, when outputs is specified.
         """
         self._name = name
         self._domain: str = domain
         self._op_type: str = op_type
         # NOTE: Make inputs immutable with the assumption that they are not mutated
         # very often. This way all mutations can be tracked.
         # If necessary, we can cache the inputs and outputs as tuples.
         self._inputs: tuple[Value | None, ...] = tuple(inputs)
         # Values belong to their defining nodes. The values list is immutable
-        self._outputs: tuple[Value, ...] = tuple(
-            Value(self, index=i) for i in range(num_outputs)
-        )
+        self._outputs: tuple[Value, ...] = self._create_outputs(num_outputs, outputs)
         attributes = tuple(attributes)
         if attributes and not isinstance(attributes[0], (Attr, RefAttr)):
             raise TypeError(
                 f"Expected the attributes to be Attr or RefAttr, got {type(attributes[0])}. "
                 "If you are copying the attributes from another node, make sure you call "
                 "node.attributes.values() because it is a dictionary."
             )
@@ -958,14 +964,62 @@
             if input_value is not None:
                 input_value._add_usage(self, i)  # pylint: disable=protected-access
 
         # Add the node to the graph if graph is specified
         if self._graph is not None:
             self._graph.append(self)
 
+    def _create_outputs(
+        self, num_outputs: int | None, outputs: Sequence[Value] | None
+    ) -> tuple[Value, ...]:
+        """Check the parameters and create outputs for the node.
+
+        Args:
+            num_outputs: The number of outputs of the node.
+            outputs: The output values of the node.
+
+        Returns:
+            The output values of the node.
+
+        Raises:
+            ValueError: If `num_outputs`, when not None, is not the same as the length of the outputs.
+            ValueError: If an output value is None.
+            ValueError: If an output value has a producer set already.
+        """
+        # Check num_outputs and outputs are consistent
+        if num_outputs is not None and outputs is not None and num_outputs != len(outputs):
+            raise ValueError(
+                "num_outputs must be the same as len(outputs) when num_outputs is specified."
+                "num_outputs: {num_outputs}, outputs: {outputs}"
+            )
+        # 1. If outputs is specified (can be empty []), use the outputs
+        if outputs is not None:
+            # Check all output values are valid first
+            for output in outputs:
+                if output is None:
+                    raise ValueError(f"Output value cannot be None. All outputs: {outputs}")
+                if output.producer() is not None:
+                    raise ValueError(
+                        f"Supplied output value cannot have a producer when used for initializing a Node. "
+                        f"Output: {output}. All outputs: {outputs}"
+                    )
+            result = []
+            for i, output in enumerate(outputs):
+                output._producer = self  # pylint: disable=protected-access
+                output._index = i  # pylint: disable=protected-access
+                result.append(output)
+            return tuple(result)
+
+        # 2. If num_outputs is specified, create num_outputs outputs
+        if num_outputs is None:
+            # Default to 1 output
+            num_outputs = 1
+        assert num_outputs is not None
+        return tuple(Value(self, index=i) for i in range(num_outputs))
+
     def __str__(self) -> str:
         node_type_text = f"{self._domain}::{self._op_type}" + f":{self._overload}" * (
             self._overload != ""
         )
         inputs_text = (
             "("
             + ", ".join(
@@ -1259,33 +1313,35 @@
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
         metadata_props: Metadata.
     """
 
     __slots__ = (
-        "_producer",
+        "_const_value",
         "_index",
-        "_metadata",
         "_metadata_props",
+        "_metadata",
         "_name",
+        "_producer",
         "_shape",
         "_type",
-        "_const_value",
         "_uses",
+        "doc_string",
     )
 
     def __init__(
         self,
         producer: Node | None,
         *,
         index: int | None,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
+        doc_string: str | None = None,
         const_value: _protocols.TensorProtocol
         | Sequence[_protocols.TensorProtocol]
         | None = None,
     ) -> None:
         # producer is None when the value is an input or an initializer
         self._producer: Node | None = producer
         self._index: int | None = index
@@ -1298,27 +1354,28 @@
         # TODO(justinchuby): Handle initialization when a const value is provided
         # We can get shape and type information from the const value
         self._const_value = const_value
         # Use a collection of (Node, int) to store uses. This is needed
         # because a single use can use the same value multiple times.
         # Use a dictionary to preserve insertion order so that the visiting order is deterministic
         self._uses: dict[tuple[Node, int], None] = {}
+        self.doc_string = doc_string
 
     def __repr__(self) -> str:
         value_name = self.name if self.name else "anonymous:" + str(id(self))
         producer = self.producer()
         producer_text = (
-            producer.name or "anonymous_node:" + str(id(producer))
+            producer.name is not None or "anonymous_node:" + str(id(producer))
             if producer is not None
             else None
         )
         return f"{self.__class__.__name__}({value_name!r}, type={self.type!r}, shape={self.shape}, producer={producer_text}, index={self.index()})"
 
     def __str__(self) -> str:
-        value_name = self.name if self.name else "anonymous:" + str(id(self))
+        value_name = self.name if self.name is not None else "anonymous:" + str(id(self))
         shape_text = str(self.shape) if self.shape is not None else "?"
         type_text = str(self.type) if self.type is not None else "?"
 
         # Quote the name because in reality the names can have invalid characters
         # that make them hard to read
         return f"%{_quoted(value_name)}<{type_text},{shape_text}>"
 
@@ -1461,19 +1518,19 @@
     __slots__ = ()
 
     def __init__(
         self,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
+        doc_string: str | None = None,
     ) -> None:
-        super().__init__(None, index=None)
-        self._name = name
-        self._shape = shape
-        self._type = type
+        super().__init__(
+            None, index=None, name=name, shape=shape, type=type, doc_string=doc_string
+        )
 
 
 def _check_node_safe_to_remove(
     node: Node, to_remove: AbstractSet[Node], graph_outputs: AbstractSet[Value]
 ) -> None:
     """Check if a node is safe to remove.
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,21 +163,23 @@
 
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
         metadata_props: Metadata that will be serialized to the ONNX file.
         meta: Metadata store for graph transform passes.
+        doc_string: Documentation string.
     """
 
     name: str
     shape: ShapeProtocol | None
     type: TypeProtocol | None
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
+    doc_string: str | None
 
     def producer(self) -> NodeProtocol | None:
         """The node that produces this value."""
         ...
 
     def index(self) -> int | None:
         """The index of the output of the node that produces this value."""
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/_type_casting.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/_type_casting.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240508/onnxscript/ir/serde.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,15 +452,14 @@
             )
             values[initializer.name] = initializer_value
 
     # Add ValueInfos for this graph scope
     value_info = {info.name: info for info in proto.value_info}
 
     # Deserialize nodes with all known values
-    # TODO(justinchuby): Handle unsorted nodes
     nodes = [_deserialize_node(node, scoped_values, value_info) for node in proto.node]
 
     # Fill in values for graph outputs
     outputs = [deserialize_value_info_proto(info, values[info.name]) for info in proto.output]
     scoped_values.pop()
     return _core.Graph(
         inputs,
@@ -510,21 +509,21 @@
     )
 
 
 def deserialize_value_info_proto(
     proto: onnx.ValueInfoProto, value: _core.Value | None
 ) -> _core.Value:
     if value is None:
-        value = _core.Value(None, index=None)
-        value.name = proto.name
+        value = _core.Value(None, index=None, name=proto.name)
     value.shape = deserialize_type_proto_for_shape(proto.type)
     value.type = deserialize_type_proto_for_type(proto.type)
     metadata_props = deserialize_metadata_props(proto.metadata_props)
     if metadata_props is not None:
         value.metadata_props.update(metadata_props)
+    value.doc_string = _get_field(proto, "doc_string")
     return value
 
 
 def deserialize_type_proto_for_shape(proto: onnx.TypeProto) -> _core.Shape | None:
     if proto.HasField("tensor_type"):
         if (shape_proto := _get_field(proto.tensor_type, "shape")) is None:
             return None
@@ -731,58 +730,108 @@
 
 def _deserialize_node(
     proto: onnx.NodeProto,
     scoped_values: list[dict[str, _core.Value]],
     value_info: dict[str, onnx.ValueInfoProto],
 ) -> _core.Node:
     node_inputs: list[_core.Value | None] = []
-    for name in proto.input:
-        if name == "":
+    for input_name in proto.input:
+        if input_name == "":
             # Empty input
             node_inputs.append(None)
             continue
+
+        # Find the input in all value scopes
         found = False
         for values in reversed(scoped_values):
-            if name not in values:
+            if input_name not in values:
                 continue
-            node_inputs.append(values[name])
+            node_inputs.append(values[input_name])
             found = True
+            del values  # Remove the reference so it is not used by mistake
             break
         if not found:
-            raise ValueError(
-                f"Input '{name}' of node '{proto.name}({proto.domain}::{proto.op_type}:{getattr(proto, 'overload', '')})' not found in any scope"
-                f" (current depth: {len(scoped_values)})"
+            # If the input is not found, we know the graph may be unsorted and
+            # the input may be a supposed-to-be initializer or an output of a node that comes later.
+            # Here we create the value with the name and add it to the current scope.
+            # Nodes need to check the value pool for potentially initialized outputs
+            logger.warning(
+                "Input '%s' of node '%s(%s::%s:%s)' not found in any scope. "
+                "The graph may be unsorted. Creating a new input (current depth: %s) .",
+                input_name,
+                proto.name,
+                proto.domain,
+                proto.op_type,
+                getattr(proto, "overload", ""),
+                len(scoped_values),
             )
-    node = _core.Node(
+            if len(scoped_values) > 1:
+                logger.warning(
+                    "Caveat: The value is created in the subgraph. If "
+                    "the node is referencing a value that is not in the current graph, "
+                    "it is impossible to create it in the correct scope.",
+                )
+            value = _core.Value(None, index=None, name=input_name)
+            # Fill in shape/type information if they exist
+            if input_name in value_info:
+                deserialize_value_info_proto(value_info[input_name], value)
+            node_inputs.append(value)
+            # We can only create the value in the current scope. If the subgraph is
+            # referencing a value that is not in the current scope, it is impossible
+            # to create it in the correct scope.
+            scoped_values[-1][input_name] = value
+
+    # Build the output values for the node.
+    node_outputs: list[_core.Value] = []
+    for output_name in proto.output:
+        if output_name == "":
+            # Empty output
+            node_outputs.append(_core.Value(None, index=None, name=""))
+            continue
+
+        # 1. When the graph is unsorted, we may be able to find the output already created
+        # as an input to some other nodes in the current scope.
+        # Note that a value is always owned by the producing node. Even though a value
+        # can be created when parsing inputs of other nodes, the new node created here
+        # that produces the value will assume ownership. It is then impossible to transfer
+        # the ownership to any other node.
+
+        # The output can only be found in the current scope. It is impossible for
+        # a node to produce an output that is not in its own scope.
+        current_scope = scoped_values[-1]
+        if output_name in current_scope:
+            value = current_scope[output_name]
+        else:
+            # 2. Common scenario: the graph is sorted and this is the first time we see the output.
+            # Create the value and add it to the current scope.
+            value = _core.Value(None, index=None, name=output_name)
+            current_scope[output_name] = value
+        # Fill in shape/type information if they exist
+        if output_name in value_info:
+            deserialize_value_info_proto(value_info[output_name], value)
+        else:
+            logger.debug(
+                "ValueInfoProto not found for output '%s' in node '%s' of type '%s'",
+                output_name,
+                proto.name,
+                proto.op_type,
+            )
+        node_outputs.append(value)
+    return _core.Node(
         proto.domain,
         proto.op_type,
         node_inputs,
         [_deserialize_attribute(a, scoped_values) for a in proto.attribute],
         overload=getattr(proto, "overload", ""),
-        num_outputs=len(proto.output),
+        outputs=node_outputs,
         name=proto.name,
         doc_string=_get_field(proto, "doc_string"),
         metadata_props=deserialize_metadata_props(proto.metadata_props),
     )
 
-    for output, value in zip(proto.output, node.outputs):
-        value.name = output
-        if output in value_info:
-            deserialize_value_info_proto(value_info[output], value)
-        else:
-            logger.debug(
-                "ValueInfoProto not found for output '%s' in node '%s' of type '%s'",
-                output,
-                proto.name,
-                proto.op_type,
-            )
-        scoped_values[-1][output] = value
-
-    return node
-
 
 # Serialization
 
 
 def serialize_model(model: _protocols.ModelProtocol) -> onnx.ModelProto:
     return serialize_model_into(onnx.ModelProto(), from_=model)
 
@@ -1244,14 +1293,16 @@
     if from_.metadata_props:
         _serialize_metadata_props_into(value_info_proto.metadata_props, from_.metadata_props)
     if from_.type is not None:
         serialize_type_into(value_info_proto.type, from_.type)
     # Need to create the type _before_ writing the shape so that the shape can be written to the leaf type proto
     if from_.shape is not None:
         serialize_shape_into(value_info_proto.type, from_.shape)
+    if from_.doc_string:
+        value_info_proto.doc_string = from_.doc_string
 
 
 def serialize_type_into(type_proto: onnx.TypeProto, from_: _protocols.TypeProtocol) -> None:
     if from_.denotation:
         type_proto.denotation = from_.denotation
     if isinstance(from_, _core.TensorType):
         tensor_type_proto = type_proto.tensor_type
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240508/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/main.py` & `onnxscript-0.1.0.dev20240508/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240508/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240508/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from onnxscript.rewriter import _ir_utils, pattern
 
 op = pattern.onnxop
 logger = logging.getLogger(__name__)
 
 
 # condition to check if we need to replace the pattern
-def check_if_need_reshape(input_a, input_b, shape_c, **_) -> bool:
+def check_if_not_need_reshape(input_a, input_b, shape_c, **_) -> bool:
     """If matmul broadcasting is enough, then we don't need the reshapes.
 
     To validate this, we need to check the following:
     1. Input shapes check: input_a and input_b should be broadcastable
     2. Output shape check: shape_c should be the same as the output shape from the matmul(input_a, input_b)
 
     If the above are true, then we don't need the reshapes.
@@ -104,17 +104,20 @@
         shorter_shape = input_b_shape
     else:
         longer_shape = input_b_shape
         shorter_shape = input_a_shape
     broadcast_matmul_output_shape = (
         longer_shape[: -len(shorter_shape)] + broadcast_matmul_output_shape
     )
-    if mimic_matmul_broadcast_behavior and dim_b == 2:
+    if mimic_matmul_broadcast_behavior and dim_b == 2 and input_b_shape[-1] == 1:
+        # If input_b is expanded to 2-D, then we need to remove the last dimension
         broadcast_matmul_output_shape = broadcast_matmul_output_shape[:-1]
-    if mimic_matmul_broadcast_behavior and dim_a == 2:
+    if mimic_matmul_broadcast_behavior and dim_a == 2 and input_a_shape[0] == 1:
+        # If input_a is expanded to 2-D, then we need to remove the first dimension
+        # of input_a, which would be the -2nd dimension of the output shape.
         broadcast_matmul_output_shape.pop(-2)
     if shape_c != broadcast_matmul_output_shape:
         logger.info(
             "Final output shape is not the same. Expected %s vs actual %s",
             shape_c,
             broadcast_matmul_output_shape,
         )
@@ -145,21 +148,21 @@
     return op.Reshape(matmul, shape_c)
 
 
 # Register the rewrite rules
 two_reshapes_matmul_reshape_rule = pattern.RewriteRule(
     two_reshapes_matmul_reshape_pattern,
     matmul,
-    check_if_need_reshape,
+    check_if_not_need_reshape,
 )
 one_reshape_matmul_reshape_rule = pattern.RewriteRule(
     one_reshape_matmul_reshape_pattern,
     matmul,
-    # We can use the same check_if_need_reshape function for both the rules,
+    # We can use the same check_if_not_need_reshape function for both the rules,
     # as one_reshape_matmul_reshape_pattern is a subset of two_reshapes_matmul_reshape_pattern.
-    check_if_need_reshape,
+    check_if_not_need_reshape,
 )
 
 # NOTE: The order of the rules is important. Larger pattern should be checked first.
 rules = pattern.RewriteRuleSet(
     [two_reshapes_matmul_reshape_rule, one_reshape_matmul_reshape_rule]
 )
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from onnxscript.rewriter import pattern
-from onnxscript.rewriter.broadcast_to_matmul import check_if_need_reshape
+from onnxscript.rewriter.broadcast_to_matmul import check_if_not_need_reshape
 
 op = pattern.onnxop
 
 
 # Pattern to match against
 def reshape_gemm_reshape_pattern(input_a, input_b, input_c, shape_a, shape_c):
     reshape_a = op.Reshape(input_a, shape_a)
@@ -14,8 +14,8 @@
 
 
 def matmul_add(op, input_a, input_b, input_c, **_):
     matmul = op.MatMul(input_a, input_b)
     return op.Add(matmul, input_c)
 
 
-rule = pattern.RewriteRule(reshape_gemm_reshape_pattern, matmul_add, check_if_need_reshape)
+rule = pattern.RewriteRule(reshape_gemm_reshape_pattern, matmul_add, check_if_not_need_reshape)
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,11 +47,12 @@
     if function_rules:
         for rule_cls in function_rules:
             count, model = rule_cls().apply_to_model(model)
             print(f"Applied {count} of onnxruntime specific function rewrite rules.")
     if pattern_rules:
         count = pattern.RewriteRuleSet(pattern_rules).apply_to_model(model)
         print(f"Applied {count} of onnxruntime specific pattern rewrite rules.")
+
     model_proto = ir.serde.serialize_model(model)
     remove_unused.remove_unused_nodes(model_proto)
     remove_unused_function.remove_unused_functions(model_proto)
     return model_proto
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240508/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240508/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240508/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240508/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240508/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240508/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript/values.py` & `onnxscript-0.1.0.dev20240508/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240508/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240507
+Version: 0.1.0.dev20240508
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240507/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240508/onnxscript.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 onnxscript/rewriter/generic_pattern.py
 onnxscript/rewriter/no_op.py
 onnxscript/rewriter/pattern.py
 onnxscript/rewriter/onnxruntime/__init__.py
 onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
 onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
 onnxscript/rewriter/onnxruntime/softmax.py
+onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
 onnxscript/rewriter/onnxruntime/transformers/__init__.py
 onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
 onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
 onnxscript/rewriter/onnxruntime/transformers/layernorm.py
 onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
 onnxscript/testing/__init__.py
 onnxscript/utils/__init__.py
```

### Comparing `onnxscript-0.1.0.dev20240507/pyproject.toml` & `onnxscript-0.1.0.dev20240508/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240507/setup.py` & `onnxscript-0.1.0.dev20240508/setup.py`

 * *Files identical despite different names*


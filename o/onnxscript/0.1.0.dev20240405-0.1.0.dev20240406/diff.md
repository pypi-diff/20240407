# Comparing `tmp/onnxscript-0.1.0.dev20240405.tar.gz` & `tmp/onnxscript-0.1.0.dev20240406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240405.tar", last modified: Fri Apr  5 00:00:48 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240406.tar", last modified: Sat Apr  6 00:01:35 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240405.tar` & `onnxscript-0.1.0.dev20240406.tar`

### file list

```diff
@@ -1,213 +1,212 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2151 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10580 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.671727 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.679726 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.679726 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.679726 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43786 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.683727 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.683727 onnxscript-0.1.0.dev20240405/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50865 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1528 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2449 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2278 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15508 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43700 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.683727 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/onnx_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tensor.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11925 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/testing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/
--rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12891 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/common/testutils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.667727 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.691727 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/error_reproduction.py
--rw-r--r--   0 vsts      (1001) docker     (127)    79029 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23392 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   102066 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      993 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/functions/ort_custom_ops.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/attrref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2349 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1380 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/dropout.py
--rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1140 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/eg1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4713 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/getitem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2025 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1569 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/identity.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/m1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/multi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2907 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4969 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2564 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2549 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/renaming.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/sequences.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13534 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1432 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2202 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/tests/models/type_double.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/type_annotation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7933 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-05 00:00:48.000000 onnxscript-0.1.0.dev20240405/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     5060 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-05 00:00:48.695726 onnxscript-0.1.0.dev20240405/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-05 00:00:32.000000 onnxscript-0.1.0.dev20240405/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.490856 onnxscript-0.1.0.dev20240406/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-06 00:01:35.490856 onnxscript-0.1.0.dev20240406/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.466856 onnxscript-0.1.0.dev20240406/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2151 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.466856 onnxscript-0.1.0.dev20240406/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.470856 onnxscript-0.1.0.dev20240406/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11068 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_legacy_ir/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5929 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_legacy_ir/protobuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.470856 onnxscript-0.1.0.dev20240406/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10580 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.470856 onnxscript-0.1.0.dev20240406/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.462856 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.470856 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.478856 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.462856 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.462856 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.478856 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.478856 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.478856 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.482856 onnxscript-0.1.0.dev20240406/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50865 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1528 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2449 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2278 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15508 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43841 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.482856 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.486856 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.486856 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15445 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.486856 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1130 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43596 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.486856 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.486856 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.490856 onnxscript-0.1.0.dev20240406/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.490856 onnxscript-0.1.0.dev20240406/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 00:01:35.490856 onnxscript-0.1.0.dev20240406/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-06 00:01:35.000000 onnxscript-0.1.0.dev20240406/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7932 2024-04-06 00:01:35.000000 onnxscript-0.1.0.dev20240406/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 00:01:35.000000 onnxscript-0.1.0.dev20240406/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-06 00:01:35.000000 onnxscript-0.1.0.dev20240406/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-06 00:01:35.000000 onnxscript-0.1.0.dev20240406/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6507 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-06 00:01:35.490856 onnxscript-0.1.0.dev20240406/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-06 00:00:42.000000 onnxscript-0.1.0.dev20240406/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240405/LICENSE` & `onnxscript-0.1.0.dev20240406/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/PKG-INFO` & `onnxscript-0.1.0.dev20240406/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240405
+Version: 0.1.0.dev20240406
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240405/README.md` & `onnxscript-0.1.0.dev20240406/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240406/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240406/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240406/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240406/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240406/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240406/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240406/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -826,15 +826,15 @@
         # Insert value info for nodes in top level graph.
         new_value_info.update(self.generate_maingraph_value_info_proto())
         # Do not store input, output or initializer into value_info
         for input in onnx_model.graph.input:
             new_value_info.pop(input.name, None)
         for output in onnx_model.graph.output:
             new_value_info.pop(output.name, None)
-        for tensor in onnx_model.graph.initializer:
+        for tensor in onnx_model.graph.initializer:  # type: ignore[assignment]
             new_value_info.pop(tensor.name, None)
         existing_value_info.update(new_value_info)
         onnx_model.graph.value_info.extend(existing_value_info.values())
 
         return onnx_model
 
     @runtime_typing.checked
```

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240406/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240406/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "serialize_value",
 ]
 
 import collections
 import logging
 import os
 import typing
-from typing import Any, Mapping, Sequence
+from typing import Any, List, Mapping, Sequence
 
 import numpy as np
 import onnx
 import onnx.external_data_helper
 import onnx.numpy_helper
 
 from onnxscript.ir import (
@@ -414,41 +414,43 @@
         name=_get_field(proto, "name"),
     )
 
 
 def deserialize_function(proto: onnx.FunctionProto) -> _core.Function:
     inputs = [_core.Input(name) for name in proto.input]
     values: dict[str, _core.Value] = {v.name: v for v in inputs}  # type: ignore[misc]
-    value_info = {info.name: info for info in proto.value_info}
+    value_info = {info.name: info for info in getattr(proto, "value_info", [])}
 
     # TODO(justinchuby): Handle unsorted nodes
     nodes = [_deserialize_node(node, [values], value_info=value_info) for node in proto.node]
     outputs = [values[name] for name in proto.output]
     graph = _core.Graph(
         inputs,
         outputs,
         nodes=nodes,
         initializers=(),
         doc_string=_get_field(proto, "doc_string"),
         opset_imports=deserialize_opset_import(proto.opset_import),
         name=(
-            f"{proto.name}_{proto.domain}" + f"__{proto.overload}" if proto.overload else ""
+            f"{proto.name}_{proto.domain}" + f"__{proto.overload}"
+            if hasattr(proto, "overload") and proto.overload
+            else ""
         ),
     )
     attributes = [_deserialize_attribute(attr, []) for attr in proto.attribute_proto]
     # Attributes without defaults
     attributes += [
         _core.Attr(name, _enums.AttributeType.UNDEFINED, None) for name in proto.attribute
     ]
     return _core.Function(
         domain=proto.domain,
         name=proto.name,
-        overload=proto.overload,
+        overload=getattr(proto, "overload", ""),
         graph=graph,
-        attributes=typing.cast(list[_core.Attr], attributes),
+        attributes=typing.cast(List[_core.Attr], attributes),
     )
 
 
 def deserialize_value_info_proto(
     proto: onnx.ValueInfoProto, value: _core.Value | None
 ) -> _core.Value:
     if value is None:
@@ -635,23 +637,23 @@
             if name not in values:
                 continue
             node_inputs.append(values[name])
             found = True
             break
         if not found:
             raise ValueError(
-                f"Input '{name}' of node '{proto.name}({proto.domain}::{proto.op_type}:{proto.overload})' not found in any scope"
+                f"Input '{name}' of node '{proto.name}({proto.domain}::{proto.op_type}:{getattr(proto, 'overload', '')})' not found in any scope"
                 f" (current depth: {len(scoped_values)})"
             )
     node = _core.Node(
         proto.domain,
         proto.op_type,
         node_inputs,
         [_deserialize_attribute(a, scoped_values) for a in proto.attribute],
-        overload=proto.overload,
+        overload=getattr(proto, "overload", ""),
         num_outputs=len(proto.output),
         name=_get_field(proto, "name"),
     )
 
     for output, value in zip(proto.output, node.outputs):
         value.name = output
         if output in value_info:
@@ -660,15 +662,15 @@
             logger.debug(
                 "ValueInfoProto not found for output '%s' in node '%s' of type '%s'",
                 output,
                 proto.name,
                 proto.op_type,
             )
         scoped_values[-1][output] = value
-    for prop in proto.metadata_props:
+    for prop in getattr(proto, "metadata_props", []):
         node.metadata_props[prop.key] = prop.value
     return node
 
 
 # Serialization
```

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240406/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/main.py` & `onnxscript-0.1.0.dev20240406/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240406/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240406/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240406/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240406/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript/values.py` & `onnxscript-0.1.0.dev20240406/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240406/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240405
+Version: 0.1.0.dev20240406
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240405/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240406/onnxscript.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 onnxscript/evaluator.py
 onnxscript/irbuilder.py
 onnxscript/main.py
 onnxscript/onnx_types.py
 onnxscript/py.typed
 onnxscript/sourceinfo.py
 onnxscript/tensor.py
-onnxscript/testing.py
 onnxscript/type_annotation.py
 onnxscript/values.py
 onnxscript.egg-info/PKG-INFO
 onnxscript.egg-info/SOURCES.txt
 onnxscript.egg-info/dependency_links.txt
 onnxscript.egg-info/requires.txt
 onnxscript.egg-info/top_level.txt
@@ -26,14 +25,18 @@
 onnxscript/_internal/ast_utils.py
 onnxscript/_internal/autocast.py
 onnxscript/_internal/deprecation.py
 onnxscript/_internal/param_manipulation.py
 onnxscript/_internal/runtime_typing.py
 onnxscript/_internal/utils.py
 onnxscript/_internal/version_utils.py
+onnxscript/_legacy_ir/__init__.py
+onnxscript/_legacy_ir/irbuilder.py
+onnxscript/_legacy_ir/protobuilder.py
+onnxscript/_legacy_ir/visitor.py
 onnxscript/_thirdparty/asciichartpy.py
 onnxscript/backend/__init__.py
 onnxscript/backend/onnx_backend.py
 onnxscript/backend/onnx_export.py
 onnxscript/diagnostics/infra/__init__.py
 onnxscript/diagnostics/infra/_infra.py
 onnxscript/diagnostics/infra/context.py
@@ -147,42 +150,37 @@
 onnxscript/onnx_opset/_impl/opset8.py
 onnxscript/onnx_opset/_impl/opset9.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
 onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
-onnxscript/tests/__init__.py
-onnxscript/tests/common/__init__.py
-onnxscript/tests/common/onnx_script_test_case.py
-onnxscript/tests/common/testutils.py
-onnxscript/tests/function_libs/torch_lib/error_reproduction.py
-onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
-onnxscript/tests/function_libs/torch_lib/ops_test_common.py
-onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-onnxscript/tests/functions/gemmgelu.py
-onnxscript/tests/functions/ort_custom_ops.py
-onnxscript/tests/models/__init__.py
-onnxscript/tests/models/attrref.py
-onnxscript/tests/models/cast_like.py
-onnxscript/tests/models/different_opset.py
-onnxscript/tests/models/dropout.py
-onnxscript/tests/models/eager_op.py
-onnxscript/tests/models/eg1.py
-onnxscript/tests/models/getitem.py
-onnxscript/tests/models/graph_attr.py
-onnxscript/tests/models/identity.py
-onnxscript/tests/models/if_statement.py
-onnxscript/tests/models/loops_break.py
-onnxscript/tests/models/loops_while.py
-onnxscript/tests/models/m1.py
-onnxscript/tests/models/multi.py
-onnxscript/tests/models/onnxfns1.py
-onnxscript/tests/models/onnxfns1A.py
-onnxscript/tests/models/onnxfns2.py
-onnxscript/tests/models/opt_input.py
-onnxscript/tests/models/opt_output.py
-onnxscript/tests/models/renaming.py
-onnxscript/tests/models/sequences.py
-onnxscript/tests/models/signal_dft.py
-onnxscript/tests/models/subfunction.py
-onnxscript/tests/models/type_double.py
+onnxscript/optimizer/__init__.py
+onnxscript/optimizer/constant_folding.py
+onnxscript/optimizer/copy_propagation.py
+onnxscript/optimizer/evaluator.py
+onnxscript/optimizer/fold_constants_v0.py
+onnxscript/optimizer/remove_unused.py
+onnxscript/optimizer/remove_unused_function.py
+onnxscript/optimizer/simple_function_folding.py
+onnxscript/rewriter/__init__.py
+onnxscript/rewriter/broadcast_to_matmul.py
+onnxscript/rewriter/cast_constant_of_shape.py
+onnxscript/rewriter/erfgelu.py
+onnxscript/rewriter/function_rule.py
+onnxscript/rewriter/gemm_to_matmul_add.py
+onnxscript/rewriter/generic_pattern.py
+onnxscript/rewriter/no_op.py
+onnxscript/rewriter/pattern.py
+onnxscript/rewriter/onnxruntime/__init__.py
+onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+onnxscript/rewriter/onnxruntime/softmax.py
+onnxscript/rewriter/onnxruntime/transformers/__init__.py
+onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+onnxscript/testing/__init__.py
+onnxscript/utils/__init__.py
+onnxscript/utils/evaluation_utils.py
+onnxscript/utils/timing_utils.py
+onnxscript/utils/utils.py
```

### Comparing `onnxscript-0.1.0.dev20240405/pyproject.toml` & `onnxscript-0.1.0.dev20240406/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -63,29 +63,63 @@
 module = "tools.*"
 disallow_untyped_defs = true
 
 # Ignore errors in test
 [[tool.mypy.overrides]]
 module = [
   "setup",
-  "onnxscript.tests.models.*",
-  "onnxscript.tests.onnx_backend_test_code.*",
+  "tests.models.*",
+  "tests.onnx_backend_test_code.*",
 ]
 ignore_errors = true
 
+[[tool.mypy.overrides]]
+module = [
+  "onnxrewriter.rewriter.generic_pattern_test.*",
+]
+check_untyped_defs = false
+disable_error_code = 'override,import-untyped,no-untyped-def,assignment'
+disallow_incomplete_defs = true
+disallow_untyped_defs = true
+disallow_untyped_decorators = true
+show_column_numbers = true
+strict_optional = true
+warn_incomplete_stub = true
+warn_no_return = true
+warn_redundant_casts = true
+warn_unused_configs = true
+warn_unused_ignores = false
+
+[[tool.mypy.overrides]]
+module = [
+  "onnxrewriter.rewriter.generic_pattern.*",
+]
+check_untyped_defs = false
+disable_error_code = 'override,import-untyped,no-untyped-def,assignment,union-attr,func-returns-value,annotation-unchecked,arg-type,index,name-defined,attr-defined'
+disallow_incomplete_defs = true
+disallow_untyped_defs = true
+disallow_untyped_decorators = true
+show_column_numbers = true
+strict_optional = true
+warn_incomplete_stub = true
+warn_no_return = true
+warn_redundant_casts = true
+warn_unused_configs = true
+warn_unused_ignores = false
+
 [tool.black]
 target-version = ["py38", "py39", "py310", "py311"]
 # Black's extend-exclude needs to be a regex string
-extend-exclude = "/onnxscript/tests/models|/onnxscript/tests/onnx_backend_test_code"
+extend-exclude = "/tests/models|/tests/onnx_backend_test_code"
 line-length = 95
 
 [tool.isort]
 profile = "black"
 extend_skip_glob = [
-  "onnxscript/tests/onnx_backend_test_code/*.py",
+  "tests/onnx_backend_test_code/*.py",
 ]
 
 [tool.pylint.messages_control]
 # NOTE: This list is for vscode. Add new disables in pyproject_pylint.toml for lintrunner
 # Exclude patterns should be modified in .lintrunner.toml
 disable = [
   "consider-using-from-import",
@@ -153,16 +187,24 @@
     "TRY003", # Messages can be constructed in the exception
     "UP006", # keep-runtime-typing
     "UP007", # keep-runtime-typing
 ]
 line-length = 95
 ignore-init-module-imports = true
 
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
+"pathlib".msg = "Using pathlib can impact performance. Use os.path instead"
+
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["TID252"] # Allow relative imports in init files
+"setup.py" = ["TID251"] # pathlib is allowed in supporting code
+"**/{examples,tests,docs,tools,utils,opgen}/*" = ["TID251"] # pathlib is allowed in supporting code
+"**/*_test.py" = ["TID251"] # pathlib is allowed in tests
+"**/generic_pattern.py" = ["FBT003", "UP037"]  # inline ignoring fails
+"**/generic_pattern_test.py" = ["ARG001", "ARG002", "PLR2004"]
 
 [tool.ruff.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "all"
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `onnxscript-0.1.0.dev20240405/setup.py` & `onnxscript-0.1.0.dev20240406/setup.py`

 * *Files identical despite different names*


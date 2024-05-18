# Comparing `tmp/onnxscript-0.1.0.dev20240516.tar.gz` & `tmp/onnxscript-0.1.0.dev20240517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240516.tar", last modified: Thu May 16 00:01:02 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240517.tar", last modified: Fri May 17 00:02:00 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240516.tar` & `onnxscript-0.1.0.dev20240517.tar`

### file list

```diff
@@ -1,220 +1,222 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.854841 onnxscript-0.1.0.dev20240516/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-16 00:01:02.854841 onnxscript-0.1.0.dev20240516/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.806840 onnxscript-0.1.0.dev20240516/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.806840 onnxscript-0.1.0.dev20240516/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36693 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.802840 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.810840 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.822841 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.802840 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.802840 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.822841 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.822841 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.826840 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.830841 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   291013 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.830841 onnxscript-0.1.0.dev20240516/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2702 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10934 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    93832 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2962 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20889 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/_type_casting.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58555 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.834841 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.842841 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.842841 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.846841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6735 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26344 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2140 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/bfloat16_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5171 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40099 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 00:01:02.850841 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-16 00:01:02.000000 onnxscript-0.1.0.dev20240516/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-16 00:01:02.854841 onnxscript-0.1.0.dev20240516/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-16 00:00:44.000000 onnxscript-0.1.0.dev20240516/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.168126 onnxscript-0.1.0.dev20240517/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-17 00:02:00.168126 onnxscript-0.1.0.dev20240517/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8671 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.092126 onnxscript-0.1.0.dev20240517/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2364 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.104126 onnxscript-0.1.0.dev20240517/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.104126 onnxscript-0.1.0.dev20240517/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36693 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.104126 onnxscript-0.1.0.dev20240517/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.104126 onnxscript-0.1.0.dev20240517/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.080126 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.104126 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.128126 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.088126 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.088126 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.128126 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.132126 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.132126 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27429 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.136126 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   291013 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.140126 onnxscript-0.1.0.dev20240517/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2750 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10936 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94051 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4285 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2962 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20997 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2863 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/_type_casting.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.144126 onnxscript-0.1.0.dev20240517/onnxscript/ir/passes/
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/passes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8468 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/passes/_pass_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    59696 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.144126 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.152126 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.156126 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4393 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10925 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2114 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.160126 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1516 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6735 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      664 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      759 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26344 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      848 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.160126 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2154 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.160126 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/bfloat16_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3284 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1274 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5171 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1841 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.164126 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40099 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.164126 onnxscript-0.1.0.dev20240517/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17964 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.168126 onnxscript-0.1.0.dev20240517/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-17 00:02:00.168126 onnxscript-0.1.0.dev20240517/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11072 2024-05-17 00:02:00.000000 onnxscript-0.1.0.dev20240517/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8302 2024-05-17 00:02:00.000000 onnxscript-0.1.0.dev20240517/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-17 00:02:00.000000 onnxscript-0.1.0.dev20240517/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-17 00:02:00.000000 onnxscript-0.1.0.dev20240517/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-17 00:02:00.000000 onnxscript-0.1.0.dev20240517/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6461 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-17 00:02:00.168126 onnxscript-0.1.0.dev20240517/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-17 00:00:46.000000 onnxscript-0.1.0.dev20240517/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240516/LICENSE` & `onnxscript-0.1.0.dev20240517/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/PKG-INFO` & `onnxscript-0.1.0.dev20240517/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240516
+Version: 0.1.0.dev20240517
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/b77f39393b9bba2fbb69a8e972fc8a36d2e811fb
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/d71b74fb0b194e718a1fa78eddef7d89b57cf4a1
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `onnxscript-0.1.0.dev20240516/README.md` & `onnxscript-0.1.0.dev20240517/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240517/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240517/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240517/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240517/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240517/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Graph building functions using the ONNX IR, compatible with the original TorchScriptGraph usage."""
 
 from __future__ import annotations
 
 import ctypes
+import typing
 from typing import Any, Dict, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import onnx
 import onnx.checker
 import onnx.defs
 import onnx.helper
@@ -173,50 +174,14 @@
     def onnx_dtype(self) -> int:
         raise NotImplementedError("onnx_dtype is not supported for TorchScriptTensor.")
 
     def value_info(self) -> Optional[onnx.ValueInfoProto]:
         raise NotImplementedError("value_info is not supported for TorchScriptTensor.")
 
 
-class _Node(ir.Node):
-    """A node that will produce TorchScriptTensor as outputs for compatibility."""
-
-    def __init__(
-        self,
-        domain: str,
-        op_type: str,
-        inputs: Sequence[ir.Value | None],
-        attributes: Sequence[ir.Attr | ir.RefAttr] = (),
-        *,
-        overload: str = "",
-        num_outputs: int = 1,
-        version: int | None = None,
-        name: str | None = None,
-        doc_string: str | None = None,
-    ):
-        super().__init__(
-            domain=domain,
-            op_type=op_type,
-            inputs=inputs,
-            attributes=attributes,
-            overload=overload,
-            num_outputs=num_outputs,
-            version=version,
-            name=name,
-            doc_string=doc_string,
-        )
-        self._outputs: tuple[TorchScriptTensor, ...] = tuple(
-            TorchScriptTensor(producer=self, index=i) for i in range(num_outputs)
-        )
-
-    @property  # type: ignore[misc]
-    def outputs(self) -> Sequence[TorchScriptTensor]:
-        return self._outputs
-
-
 class TorchScriptTracingEvaluator(evaluator.Evaluator):
     """An onnxscript Evaluator that captures the graph."""
 
     def __init__(self, graph: TorchScriptGraph):
         self._graph: TorchScriptGraph = graph
 
     @property
@@ -364,24 +329,24 @@
     Returns:
         The outputs of the created node.
     """
     # Filter out None attributes, this can be convenient client side because
     # now they can pass through None attributes, and have them not show up
     attributes = {k: v for k, v in attributes.items() if v is not None}
 
-    node = _Node(
+    node = ir.Node(
         domain,
         op_type,
         inputs=inputs,
         attributes=[_build_attribute(key, value) for key, value in attributes.items()],
-        num_outputs=num_outputs,
+        outputs=[TorchScriptTensor() for _ in range(num_outputs)],
     )
     graph.append(node)
 
-    return node.outputs
+    return typing.cast(Sequence[TorchScriptTensor], node.outputs)
 
 
 def _shared_functions() -> list[ir.Function]:
     """Hack to always include the share ops."""
 
     # TODO: Remove after https://github.com/microsoft/onnxscript/issues/834 is fixed
     return [
@@ -493,14 +458,15 @@
             # Only the root graph can have initializers. Add as initializer
             # to root graph, and add as input to current graph.
             self._initializers_inputs_from_parent[name] = (
                 self._parent_torch_script_graph.add_initializer(name, value)
             )
         else:
             input = TorchScriptTensor(name=name)
+            input.const_value = _TorchTensor(value)
             self._initializers_inputs[name] = input
             self._initializers[name] = value
         return input
 
     def register_outputs(
         self, outputs: Union[TorchScriptTensor, Tuple[TorchScriptTensor, ...]]
     ):
@@ -728,18 +694,18 @@
         unique_custom_domains: Dict[str, int] = {"": opset_version}
 
         for function in function_dict.values():
             # TODO(BowenBao): All local function domain versions are hardcoded as 1.
             unique_custom_domains[function.domain] = 1
 
         if include_initializers:
-            self._graph.initializers.update(
-                {name: _TorchTensor(value) for name, value in self._initializers.items()}
-            )
+            self._graph.initializers.update(self._initializers_inputs)
         else:
+            # TODO(justinchuby): Potentially set to const_value to None instead so we
+            # don't lose handle on the values.
             self._graph.initializers.clear()
 
         onnx_model = ir.Model(
             self._graph,
             ir_version=8,
             producer_name=f"pytorch {torch.__version__}",
             functions=[*function_dict.values(), *_shared_functions()],
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240517/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,17 +64,19 @@
     # Types
     "OperatorIdentifier",
     # Protobuf compatible types
     "TensorProtoTensor",
     # Conversion functions
     "from_proto",
     "to_proto",
+    # Pass infrastructure
+    "passes",
 ]
 
-from onnxscript.ir import serde
+from onnxscript.ir import passes, serde
 from onnxscript.ir._core import (
     Attr,
     AttrFloat32,
     AttrFloat32s,
     AttrGraph,
     AttrGraphs,
     AttrInt64,
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_convenience.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         ...         ),
         ...     "graph": ir.Graph([], [], nodes=[], name="graph0"),
         ...     "graphs": [ir.Graph([], [], nodes=[], name="graph1"), ir.Graph([], [], nodes=[], name="graph2")],
         ...     "type_proto": ir.TensorType(ir.DataType.FLOAT),
         ...     "type_protos": [ir.TensorType(ir.DataType.FLOAT), ir.TensorType(ir.DataType.FLOAT)],
         ... }
         >>> convert_attributes(attrs)
-        [AttrInt64('int', 1), AttrFloat32('float', 1.0), AttrString('str', 'hello'), AttrInt64s('ints', [1, 2, 3]), AttrFloat32s('floats', [1.0, 2.0, 3.0]), AttrStrings('strings', ['hello', 'world']), AttrTensor('tensor', Tensor<DOUBLE,[3]>(array([1., 2., 3.]), name='')), AttrTensor('tensor_proto', TensorProtoTensor<FLOAT,[3]>(name='proto')), AttrInt64s('graph', Graph(
+        [AttrInt64('int', 1), AttrFloat32('float', 1.0), AttrString('str', 'hello'), AttrInt64s('ints', [1, 2, 3]), AttrFloat32s('floats', [1.0, 2.0, 3.0]), AttrStrings('strings', ['hello', 'world']), AttrTensor('tensor', Tensor<DOUBLE,[3]>(array([1., 2., 3.]), name=None)), AttrTensor('tensor_proto', TensorProtoTensor<FLOAT,[3]>(name='proto')), AttrInt64s('graph', Graph(
             name='graph0',
             inputs=(
         <BLANKLINE>
             ),
             outputs=(
         <BLANKLINE>
             ),
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     OrderedDict,
     Sequence,
     Union,
 )
 
 import numpy as np
 
+import onnxscript
 from onnxscript.ir import (
     _display,
     _enums,
     _linked_list,
     _metadata,
     _name_authority,
     _protocols,
@@ -270,15 +271,15 @@
 
     def __init__(
         self,
         value: TArrayCompatible,
         dtype: _enums.DataType | None = None,
         *,
         shape: Shape | None = None,
-        name: str = "",
+        name: str | None = None,
         doc_string: str | None = None,
         metadata_props: dict[str, str] | None = None,
     ) -> None:
         """Initialize a tensor.
 
         Args:
             value: The backing data of the tensor. It can be a numpy array compatible object or a DLPack compatible object.
@@ -614,15 +615,15 @@
     )
 
     def __init__(
         self,
         value: Sequence[bytes] | npt.NDArray[np.bytes_],
         *,
         shape: Shape | None = None,
-        name: str = "",
+        name: str | None = None,
         doc_string: str | None = None,
         metadata_props: dict[str, str] | None = None,
     ) -> None:
         """Initialize a tensor.
 
         Args:
             value: The backing data of the tensor. It can be a numpy array or a Sequence of bytes.
@@ -1360,29 +1361,27 @@
         producer: Node | None = None,
         *,
         index: int | None = None,
         name: str | None = None,
         shape: Shape | None = None,
         type: _protocols.TypeProtocol | None = None,
         doc_string: str | None = None,
-        const_value: _protocols.TensorProtocol
-        | Sequence[_protocols.TensorProtocol]
-        | None = None,
+        const_value: _protocols.TensorProtocol | None = None,
     ) -> None:
         """Initialize a value.
 
         Args:
             producer: The node that produces the value.
                 It can be ``None`` when the value is initialized first than its producer.
             index: The index of the output of the defining node.
             name: The name of the value.
             shape: The shape of the value.
             type: The type of the value.
             doc_string: The documentation string.
-            const_value: The constant tensor is the value constant.
+            const_value: The constant tensor if the value is constant.
         """
         self._producer: Node | None = producer
         self._index: int | None = index
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = None
 
         self._name: str | None = name
@@ -1452,14 +1451,16 @@
 
     @property
     def name(self) -> str | None:
         return self._name
 
     @name.setter
     def name(self, value: str | None) -> None:
+        if self._const_value is not None:
+            self._const_value.name = value
         self._name = value
 
     @property
     def type(self) -> _protocols.TypeProtocol | None:
         """The type of the tensor.
 
         Example types can be ``TensorType``, ``SparseTensorType``, ``SequenceType``, ``OptionalType``.
@@ -1505,27 +1506,32 @@
             self._shape = value
             return
         raise TypeError(f"Expected value to be a Shape or None, got '{type(value)}'")
 
     @property
     def const_value(
         self,
-    ) -> _protocols.TensorProtocol | Sequence[_protocols.TensorProtocol] | None:
+    ) -> _protocols.TensorProtocol | None:
         """A concrete value.
 
         The value can be backed by different raw data types, such as numpy arrays.
         The only guarantee is that it conforms TensorProtocol.
         """
         return self._const_value
 
     @const_value.setter
     def const_value(
         self,
-        value: _protocols.TensorProtocol | Sequence[_protocols.TensorProtocol] | None,
+        value: _protocols.TensorProtocol | None,
     ) -> None:
+        if onnxscript.DEBUG:
+            if value is not None and not isinstance(value, _protocols.TensorProtocol):
+                raise TypeError(
+                    f"Expected value to be a TensorProtocol or None, got '{type(value)}'"
+                )
         self._const_value = value
 
     @property
     def meta(self) -> _metadata.MetadataStore:
         """The metadata store for intermediate analysis.
 
         Write to the :attr:`metadata_props` if you would like the metadata to be serialized
@@ -1646,35 +1652,36 @@
 
     def __init__(
         self,
         inputs: Sequence[Input],
         outputs: Sequence[Value],
         *,
         nodes: Iterable[Node],
-        initializers: Sequence[_protocols.TensorProtocol] = (),
+        initializers: Sequence[Value] = (),
         doc_string: str | None = None,
         opset_imports: dict[str, int] | None = None,
         name: str | None = None,
         metadata_props: dict[str, str] | None = None,
     ):
         self.name = name
 
         # Private fields that are not to be accessed by any other classes
         self._inputs = list(inputs)
         self._outputs = list(outputs)
+        self._initializers = {}
         for initializer in initializers:
             if isinstance(initializer, str):
                 raise TypeError(
-                    "Initializer must be a TensorProtocol, not a string. "
+                    "Initializer must be a Value, not a string. "
                     "If you are copying the initializers from another graph, "
                     "make sure you call graph.initializers.values() because it is a dictionary."
                 )
             if initializer.name is None:
                 raise ValueError(f"Initializer must have a name: {initializer}")
-        self._initializers = {tensor.name: tensor for tensor in initializers}
+            self._initializers[initializer.name] = initializer
         self._doc_string = doc_string
         self._opset_imports = opset_imports or {}
         self._metadata: _metadata.MetadataStore | None = None
         self._metadata_props: dict[str, str] | None = metadata_props
         self._nodes: _linked_list.DoublyLinkedSet[Node] = _linked_list.DoublyLinkedSet()
         # Be sure the initialize the name authority before extending the nodes
         # because it is used to name the nodes and their outputs
@@ -1687,15 +1694,15 @@
         return self._inputs
 
     @property
     def outputs(self) -> list[Value]:
         return self._outputs
 
     @property
-    def initializers(self) -> dict[str, _protocols.TensorProtocol]:
+    def initializers(self) -> dict[str, Value]:
         return self._initializers
 
     @property
     def doc_string(self) -> str | None:
         return self._doc_string
 
     @doc_string.setter
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_protocols.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         raw: The raw data behind this tensor. It can be anything.
         size: The number of elements in the tensor.
         nbytes: The number of bytes in the tensor.
         metadata_props: Metadata that will be serialized to the ONNX file.
         meta: Metadata store for graph transform passes.
     """
 
-    name: str
+    name: str | None
     shape: ShapeProtocol
     dtype: _enums.DataType
     doc_string: str | None
     raw: Any
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
@@ -172,22 +172,24 @@
     Attributes:
         name: The name of the value. A value is always named when it is part of a graph.
         shape: The shape of the value.
         type: The type of the value.
         metadata_props: Metadata that will be serialized to the ONNX file.
         meta: Metadata store for graph transform passes.
         doc_string: Documentation string.
+        const_value: The constant tensor is the value constant.
     """
 
     name: str
     shape: ShapeProtocol | None
     type: TypeProtocol | None
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
     doc_string: str | None
+    const_value: TensorProtocol | None
 
     def producer(self) -> NodeProtocol | None:
         """The node that produces this value."""
         ...
 
     def index(self) -> int | None:
         """The index of the output of the node that produces this value."""
@@ -288,15 +290,15 @@
         meta: Metadata store for graph transform passes.
     """
 
     # TODO(justinchuby): Support quantization_annotation
     name: str | None
     inputs: MutableSequence[ValueProtocol]
     outputs: MutableSequence[ValueProtocol]
-    initializers: MutableMapping[str, TensorProtocol]
+    initializers: MutableMapping[str, ValueProtocol]
     doc_string: str
     opset_imports: MutableMapping[str, int]
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
@@ -348,15 +350,15 @@
         metadata_props: Metadata that will be serialized to the ONNX file.
         meta: Metadata store for graph transform passes.
     """
 
     name: str | None
     inputs: Sequence[ValueProtocol]
     outputs: Sequence[ValueProtocol]
-    initializers: Mapping[str, TensorProtocol]
+    initializers: Mapping[str, ValueProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
     metadata_props: MutableMapping[str, str]
     meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/_type_casting.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/_type_casting.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240517/onnxscript/ir/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,21 @@
         )
         self._metadata: _metadata.MetadataStore | None = None
 
     @property
     def name(self) -> str:
         return self._proto.name
 
+    @name.setter
+    def name(self, value: str | None) -> None:
+        if value is None:
+            self._proto.ClearField("name")
+        else:
+            self._proto.name = value
+
     @property
     def shape(self) -> _core.Shape:
         return _core.Shape(self._proto.dims, frozen=True)
 
     @property
     def dtype(self) -> _enums.DataType:
         return _enums.DataType(self._proto.data_type)
@@ -484,70 +491,83 @@
                         function_value_value_info_mapping[function_id][output.name],
                         output,
                     )
             # The function outputs are handled as well because they are also node outputs
 
 
 def deserialize_graph(proto: onnx.GraphProto) -> _core.Graph:
+    """Deserialize a graph proto, recursively if needed.
+
+    Args:
+        proto: The graph proto to deserialize.
+
+    Returns:
+        IR Graph.
+    """
     return _deserialize_graph(proto, [])
 
 
 def _deserialize_graph(
     proto: onnx.GraphProto, scoped_values: list[dict[str, _core.Value]]
 ) -> _core.Graph:
     """Deserialize a graph proto, recursively if needed.
 
     Args:
         proto: The graph proto to deserialize.
         scoped_values: A list of dictionaries mapping value names to their corresponding Value objects.
             Every time we enter a new graph, a new scope is created and appended to this list to include
             all values defined in the scope.
         scoped_value_info: A list of dictionaries mapping value names to their corresponding ValueInfoProto.
+
+    Returns:
+        IR Graph.
     """
     # Create values for initializers and inputs
-    initializers = [deserialize_tensor(tensor) for tensor in proto.initializer]
+    initializer_tensors = [deserialize_tensor(tensor) for tensor in proto.initializer]
     inputs = [_core.Input(info.name) for info in proto.input]
     for info, value in zip(proto.input, inputs):
         deserialize_value_info_proto(info, value)
 
     # Initialize the values dictionary for this graph scope with the inputs and initializers
     values: dict[str, _core.Value] = {v.name: v for v in inputs}  # type: ignore[misc]
     scoped_values.append(values)
-    for initializer in initializers:
-        if initializer.name in values:
+    initializer_values = []
+    for tensor in initializer_tensors:
+        if tensor.name in values:
             # The initializer is for an input
-            values[initializer.name].const_value = initializer
+            initializer_value = values[tensor.name]
+            initializer_value.const_value = tensor
         else:
             # The initializer is for some other value. Create this value first
             initializer_value = _core.Value(
                 None,
                 index=None,
-                name=initializer.name,
+                name=tensor.name,
                 # TODO(justinchuby): Fix type hinting for shape and dtype
-                shape=initializer.shape,  # type: ignore
-                type=_core.TensorType(initializer.dtype),
-                const_value=initializer,
+                shape=tensor.shape,  # type: ignore
+                type=_core.TensorType(tensor.dtype),
+                const_value=tensor,
             )
-            values[initializer.name] = initializer_value
+            values[tensor.name] = initializer_value  # type: ignore[index]
+        initializer_values.append(initializer_value)
 
     # Add ValueInfos for this graph scope
     value_info = {info.name: info for info in proto.value_info}
 
     # Deserialize nodes with all known values
     nodes = [_deserialize_node(node, scoped_values, value_info) for node in proto.node]
 
     # Fill in values for graph outputs
     outputs = [deserialize_value_info_proto(info, values[info.name]) for info in proto.output]
     scoped_values.pop()
     return _core.Graph(
         inputs,
         outputs,
         nodes=nodes,
-        # TODO(justinchuby): Attach the values associated with the initializers
-        initializers=initializers,
+        initializers=initializer_values,
         doc_string=_get_field(proto, "doc_string"),
         name=_get_field(proto, "name"),
         metadata_props=deserialize_metadata_props(proto.metadata_props),
     )
 
 
 def deserialize_function(proto: onnx.FunctionProto) -> _core.Function:
@@ -701,17 +721,17 @@
     if proto.data_location == onnx.TensorProto.EXTERNAL:
         external_info = onnx.external_data_helper.ExternalDataInfo(proto)
         return _core.ExternalTensor(
             path=os.path.join(base_path, external_info.location),
             offset=external_info.offset,
             length=external_info.length,
             dtype=_enums.DataType(proto.data_type),
-            name=proto.name,
+            name=_get_field(proto, "name"),
             shape=_core.Shape(proto.dims),
-            doc_string=proto.doc_string,
+            doc_string=_get_field(proto, "doc_string"),
             metadata_props=deserialize_metadata_props(proto.metadata_props),
         )
     if proto.data_type == _enums.DataType.STRING:
         name = _get_field(proto, "name")
         doc_string = _get_field(proto, "doc_string")
         metadata_props = deserialize_metadata_props(proto.metadata_props)
         return _core.StringTensor(
@@ -1044,14 +1064,24 @@
     for key in sorted(from_):
         string_string_entries.add(key=key, value=from_[key])
 
 
 def serialize_graph(
     graph: _protocols.GraphProtocol | _protocols.GraphViewProtocol,
 ) -> onnx.GraphProto:
+    """Serializes the given graph into an :class:`onnx.GraphProto`.
+
+    When the graph initializers do not have `const_value` set, they will be skipped.
+
+    Args:
+        graph: The graph to be serialized.
+
+    Returns:
+        The serialized ONNX GraphProto object.
+    """
     graph_proto = onnx.GraphProto()
     serialize_graph_into(graph_proto, from_=graph)
     return graph_proto
 
 
 def serialize_graph_into(
     graph_proto: onnx.GraphProto,
@@ -1061,15 +1091,23 @@
         graph_proto.name = from_.name
     if from_.doc_string:
         graph_proto.doc_string = from_.doc_string
     for input_ in from_.inputs:
         serialize_value_into(graph_proto.input.add(), input_)
     # TODO(justinchuby): Support sparse_initializer
     for initializer in from_.initializers.values():
-        serialize_tensor_into(graph_proto.initializer.add(), from_=initializer)
+        if initializer.const_value is None:
+            # Skip initializers without constant values
+            logger.warning(
+                "Initializer '%s' does not have a constant value set.", initializer.name
+            )
+            continue
+        # Make sure the tensor's name is the same as the value's name
+        initializer.const_value.name = initializer.name
+        serialize_tensor_into(graph_proto.initializer.add(), from_=initializer.const_value)
     for node in from_:
         serialize_node_into(graph_proto.node.add(), from_=node)
         for node_output in node.outputs:
             if not _should_create_value_info_for_value(node_output):
                 # No need to serialize value info if it is not set
                 continue
             if node_output.is_graph_output():
@@ -1213,15 +1251,16 @@
     if isinstance(from_, TensorProtoTensor):
         # Directly copy from the tensor proto if it is available
         tensor_proto.CopyFrom(from_.raw)
         if from_.metadata_props:
             _serialize_metadata_props_into(tensor_proto.metadata_props, from_.metadata_props)
         return
 
-    tensor_proto.name = from_.name
+    if from_.name:
+        tensor_proto.name = from_.name
     if from_.doc_string:
         tensor_proto.doc_string = from_.doc_string
     tensor_proto.data_type = from_.dtype.value
     tensor_proto.dims.extend(from_.shape.numpy())
     if isinstance(from_, _core.ExternalTensor):
         # Store external tensors as is
         tensor_proto.data_location = onnx.TensorProto.EXTERNAL
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240517/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/main.py` & `onnxscript-0.1.0.dev20240517/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240517/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         inline_simple_functions(model)
         modified = fold_constants(
             model, external_data_folder, onnx_shape_inference=onnx_shape_inference
         )
 
         remove_unused_nodes(model)
         inline_simple_functions(model)
-        remove_unused_functions(model)
+        model = remove_unused_functions(model)
         inline_functions_with_unused_outputs(model)
         # NOTE: This is general rewrite rules
         model = rewriter.rewrite(
             model,
             pattern_rewrite_rules=[
                 *no_op.rules.rules,  # TODO: merge this rule into constant folding?
                 *broadcast_to_matmul.rules.rules,
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240517/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240517/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240517/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240517/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240517/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,9 +35,9 @@
         if not isinstance(pattern_rewrite_rules, RewriteRuleSet):
             # Create a pattern rule-set using provided rules
             pattern_rewrite_rules = pattern.RewriteRuleSet(pattern_rewrite_rules)
         count = pattern_rewrite_rules.apply_to_model(model_ir)
         print(f"Applied {count} of general pattern rewrite rules.")
     model = ir.serde.serialize_model(model_ir)
     remove_unused.remove_unused_nodes(model)
-    remove_unused_function.remove_unused_functions(model)
+    model = remove_unused_function.remove_unused_functions(model)
     return model
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,9 +50,9 @@
             print(f"Applied {count} of onnxruntime specific function rewrite rules.")
     if pattern_rules:
         count = pattern.RewriteRuleSet(pattern_rules).apply_to_model(model)
         print(f"Applied {count} of onnxruntime specific pattern rewrite rules.")
 
     model_proto = ir.serde.serialize_model(model)
     remove_unused.remove_unused_nodes(model_proto)
-    remove_unused_function.remove_unused_functions(model_proto)
+    model_proto = remove_unused_function.remove_unused_functions(model_proto)
     return model_proto
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/bfloat16_utils/bfloat16_converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240517/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240517/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240517/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240517/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240517/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240517/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript/values.py` & `onnxscript-0.1.0.dev20240517/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240517/onnxscript.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240516
+Version: 0.1.0.dev20240517
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://onnxscript.ai/
 Project-URL: Repository, https://github.com/microsoft/onnxscript
-Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/b77f39393b9bba2fbb69a8e972fc8a36d2e811fb
+Project-URL: Commit, https://github.com/microsoft/onnxscript/tree/d71b74fb0b194e718a1fa78eddef7d89b57cf4a1
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `onnxscript-0.1.0.dev20240516/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240517/onnxscript.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -120,21 +120,22 @@
 onnxscript/function_libs/torch_lib/ops/vision.py
 onnxscript/ir/__init__.py
 onnxscript/ir/_convenience.py
 onnxscript/ir/_core.py
 onnxscript/ir/_display.py
 onnxscript/ir/_enums.py
 onnxscript/ir/_graph_comparison.py
-onnxscript/ir/_invariants.py
 onnxscript/ir/_linked_list.py
 onnxscript/ir/_metadata.py
 onnxscript/ir/_name_authority.py
 onnxscript/ir/_protocols.py
 onnxscript/ir/_type_casting.py
 onnxscript/ir/serde.py
+onnxscript/ir/passes/__init__.py
+onnxscript/ir/passes/_pass_infra.py
 onnxscript/onnx_opset/__init__.py
 onnxscript/onnx_opset/_impl/opset1.py
 onnxscript/onnx_opset/_impl/opset10.py
 onnxscript/onnx_opset/_impl/opset11.py
 onnxscript/onnx_opset/_impl/opset12.py
 onnxscript/onnx_opset/_impl/opset13.py
 onnxscript/onnx_opset/_impl/opset14.py
```

### Comparing `onnxscript-0.1.0.dev20240516/pyproject.toml` & `onnxscript-0.1.0.dev20240517/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240516/setup.py` & `onnxscript-0.1.0.dev20240517/setup.py`

 * *Files identical despite different names*


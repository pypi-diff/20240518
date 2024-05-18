# Comparing `tmp/codefly_cli-0.0.4.tar.gz` & `tmp/codefly_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefly_cli-0.0.4.tar", max compression
+gzip compressed data, was "codefly_cli-0.0.5.tar", max compression
```

## Comparing `codefly_cli-0.0.4.tar` & `codefly_cli-0.0.5.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.4/codefly_cli/actions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/actions/v0/__init__.py
--rw-r--r--   0        0        0     2004 2024-05-13 13:49:13.446542 codefly_cli-0.0.4/codefly_cli/actions/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448403 codefly_cli-0.0.4/codefly_cli/actions/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2009 2024-05-13 13:49:13.448579 codefly_cli-0.0.4/codefly_cli/actions/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.447517 codefly_cli-0.0.4/codefly_cli/actions/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     3743 2024-05-13 13:49:13.447494 codefly_cli-0.0.4/codefly_cli/actions/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446585 codefly_cli-0.0.4/codefly_cli/actions/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2588 2024-05-13 13:49:13.448454 codefly_cli-0.0.4/codefly_cli/actions/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448732 codefly_cli-0.0.4/codefly_cli/actions/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.4/codefly_cli/base/__init__.py
--rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.4/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/base/v0/__init__.py
--rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1676 2024-05-13 13:49:49.184868 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1855 2024-05-13 13:49:49.188891 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3371 2024-05-13 13:49:49.183146 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1615 2024-05-13 13:49:49.202244 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1791 2024-05-13 13:49:49.179812 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1950 2024-05-13 13:49:49.203856 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1704 2024-05-13 13:49:49.190337 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2613 2024-05-13 13:49:49.181480 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1701 2024-05-13 13:49:49.199660 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2168 2024-05-13 13:49:49.122019 codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2399 2024-05-13 13:49:13.447867 codefly_cli-0.0.4/codefly_cli/base/v0/agent_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448589 codefly_cli-0.0.4/codefly_cli/base/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     2500 2024-05-13 13:49:13.448413 codefly_cli-0.0.4/codefly_cli/base/v0/configuration_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.446805 codefly_cli-0.0.4/codefly_cli/base/v0/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5828 2024-05-13 13:49:13.449218 codefly_cli-0.0.4/codefly_cli/base/v0/endpoint_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449713 codefly_cli-0.0.4/codefly_cli/base/v0/endpoint_pb2_grpc.py
--rw-r--r--   0        0        0     2169 2024-05-13 13:49:13.449335 codefly_cli-0.0.4/codefly_cli/base/v0/environment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449018 codefly_cli-0.0.4/codefly_cli/base/v0/environment_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2024-05-13 13:49:13.448914 codefly_cli-0.0.4/codefly_cli/base/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.448654 codefly_cli-0.0.4/codefly_cli/base/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2768 2024-05-13 13:49:13.449677 codefly_cli-0.0.4/codefly_cli/base/v0/network_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451000 codefly_cli-0.0.4/codefly_cli/base/v0/network_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-13 13:49:13.449946 codefly_cli-0.0.4/codefly_cli/base/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.449931 codefly_cli-0.0.4/codefly_cli/base/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-13 13:49:13.450029 codefly_cli-0.0.4/codefly_cli/base/v0/scope_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450124 codefly_cli-0.0.4/codefly_cli/base/v0/scope_pb2_grpc.py
--rw-r--r--   0        0        0     4669 2024-05-13 13:49:13.450065 codefly_cli-0.0.4/codefly_cli/base/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450638 codefly_cli-0.0.4/codefly_cli/base/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2414 2024-05-13 13:49:13.450683 codefly_cli-0.0.4/codefly_cli/base/v0/spec_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450790 codefly_cli-0.0.4/codefly_cli/base/v0/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3318 2024-05-13 13:49:13.450982 codefly_cli-0.0.4/codefly_cli/base/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450985 codefly_cli-0.0.4/codefly_cli/base/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/buf/__init__.py
--rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.4/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.4/codefly_cli/buf/validate/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/buf/validate/__init__.py
--rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.4/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1735 2024-05-13 13:49:49.171523 codefly_cli-0.0.4/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
--rw-r--r--   0        0        0   105220 2024-05-13 13:49:49.169873 codefly_cli-0.0.4/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.4/codefly_cli/buf/validate/expression.proto
--rw-r--r--   0        0        0     2292 2024-05-13 13:49:13.450790 codefly_cli-0.0.4/codefly_cli/buf/validate/expression_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.450818 codefly_cli-0.0.4/codefly_cli/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/__init__.py
--rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1833 2024-05-13 13:49:49.173958 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/private.proto
--rw-r--r--   0        0        0     2332 2024-05-13 13:49:13.450797 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/private_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.451295 codefly_cli-0.0.4/codefly_cli/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.4/codefly_cli/buf/validate/validate.proto
--rw-r--r--   0        0        0   144402 2024-05-13 13:49:13.452802 codefly_cli-0.0.4/codefly_cli/buf/validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452137 codefly_cli-0.0.4/codefly_cli/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/cli/__init__.py
--rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.4/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/cli/v0/__init__.py
--rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.4/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7578 2024-05-13 13:49:49.187411 codefly_cli-0.0.4/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    10048 2024-05-13 13:49:49.118488 codefly_cli-0.0.4/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0    11732 2024-05-13 13:49:13.451372 codefly_cli-0.0.4/codefly_cli/cli/v0/cli_pb2.py
--rw-r--r--   0        0        0    28562 2024-05-13 13:49:13.452428 codefly_cli-0.0.4/codefly_cli/cli/v0/cli_pb2_grpc.py
--rw-r--r--   0        0        0     4280 2024-05-13 15:09:26.582753 codefly_cli-0.0.4/codefly_cli/codefly.py
--rw-r--r--   0        0        0     1517 2024-05-13 13:49:49.218228 codefly_cli-0.0.4/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1912 2024-05-13 13:49:49.220245 codefly_cli-0.0.4/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1792 2024-05-13 13:49:13.453277 codefly_cli-0.0.4/codefly_cli/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453501 codefly_cli-0.0.4/codefly_cli/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2690 2024-05-13 13:49:13.453447 codefly_cli-0.0.4/codefly_cli/google/api/http_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453409 codefly_cli-0.0.4/codefly_cli/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/observability/__init__.py
--rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.4/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/observability/v0/__init__.py
--rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-05-13 13:49:49.211153 codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1550 2024-05-13 13:49:49.209688 codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2265 2024-05-13 13:49:49.213031 codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2214 2024-05-13 13:49:49.214782 codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2474 2024-05-13 13:49:13.452611 codefly_cli-0.0.4/codefly_cli/observability/v0/dependencies_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452686 codefly_cli-0.0.4/codefly_cli/observability/v0/dependencies_pb2_grpc.py
--rw-r--r--   0        0        0     1837 2024-05-13 13:49:13.452443 codefly_cli-0.0.4/codefly_cli/observability/v0/inventory_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.452782 codefly_cli-0.0.4/codefly_cli/observability/v0/inventory_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2024-05-13 13:49:13.452547 codefly_cli-0.0.4/codefly_cli/observability/v0/logs_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453108 codefly_cli-0.0.4/codefly_cli/observability/v0/logs_pb2_grpc.py
--rw-r--r--   0        0        0     2098 2024-05-13 13:49:13.453294 codefly_cli-0.0.4/codefly_cli/observability/v0/metrics_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454033 codefly_cli-0.0.4/codefly_cli/observability/v0/metrics_pb2_grpc.py
--rw-r--r--   0        0        0     2985 2024-05-13 13:49:13.454381 codefly_cli-0.0.4/codefly_cli/observability/v0/sessions_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.453846 codefly_cli-0.0.4/codefly_cli/observability/v0/sessions_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/__init__.py
--rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.4/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/agent/__init__.py
--rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.4/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/agent/v0/__init__.py
--rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.4/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3328 2024-05-13 13:49:49.194622 codefly_cli-0.0.4/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4050 2024-05-13 13:49:49.205929 codefly_cli-0.0.4/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     5107 2024-05-13 13:49:13.453465 codefly_cli-0.0.4/codefly_cli/services/agent/v0/agent_pb2.py
--rw-r--r--   0        0        0     2895 2024-05-13 13:49:13.454028 codefly_cli-0.0.4/codefly_cli/services/agent/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     6560 2024-05-13 13:49:13.454342 codefly_cli-0.0.4/codefly_cli/services/agent/v0/communicate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454415 codefly_cli-0.0.4/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
--rw-r--r--   0        0        0     2426 2024-05-13 13:49:13.454363 codefly_cli-0.0.4/codefly_cli/services/agent/v0/cyclonedx_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.454382 codefly_cli-0.0.4/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/builder/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/builder/v0/__init__.py
--rw-r--r--   0        0        0    11603 2024-05-13 13:49:13.455038 codefly_cli-0.0.4/codefly_cli/services/builder/v0/builder_pb2.py
--rw-r--r--   0        0        0    15720 2024-05-13 13:49:13.455498 codefly_cli-0.0.4/codefly_cli/services/builder/v0/builder_pb2_grpc.py
--rw-r--r--   0        0        0     3239 2024-05-13 13:49:13.455801 codefly_cli-0.0.4/codefly_cli/services/builder/v0/deployment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455001 codefly_cli-0.0.4/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     1959 2024-05-13 13:49:13.455543 codefly_cli-0.0.4/codefly_cli/services/builder/v0/docker_pb2.py
--rw-r--r--   0        0        0      159 2024-05-13 13:49:13.455789 codefly_cli-0.0.4/codefly_cli/services/builder/v0/docker_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/runtime/__init__.py
--rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.4/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.4/codefly_cli/services/runtime/v0/__init__.py
--rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.4/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7530 2024-05-13 13:49:49.198194 codefly_cli-0.0.4/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    11345 2024-05-13 13:49:13.455933 codefly_cli-0.0.4/codefly_cli/services/runtime/v0/runtime_pb2.py
--rw-r--r--   0        0        0    15818 2024-05-13 13:49:13.456279 codefly_cli-0.0.4/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
--rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.4/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
--rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.4/codefly_cli/tests/test_cli.py
--rw-r--r--   0        0        0      481 2024-05-13 15:09:48.842568 codefly_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.5/codefly_cli/actions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/actions/v0/__init__.py
+-rw-r--r--   0        0        0     2004 2024-05-16 14:53:37.499836 codefly_cli-0.0.5/codefly_cli/actions/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499681 codefly_cli-0.0.5/codefly_cli/actions/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2009 2024-05-16 14:53:37.499220 codefly_cli-0.0.5/codefly_cli/actions/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499510 codefly_cli-0.0.5/codefly_cli/actions/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     3743 2024-05-16 14:53:37.499953 codefly_cli-0.0.5/codefly_cli/actions/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499899 codefly_cli-0.0.5/codefly_cli/actions/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2588 2024-05-16 14:53:37.499937 codefly_cli-0.0.5/codefly_cli/actions/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499877 codefly_cli-0.0.5/codefly_cli/actions/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.5/codefly_cli/base/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.5/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/base/v0/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1676 2024-05-13 13:49:49.184868 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1855 2024-05-13 13:49:49.188891 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     3371 2024-05-13 13:49:49.183146 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1615 2024-05-13 13:49:49.202244 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1791 2024-05-13 13:49:49.179812 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2024-05-13 13:49:49.203856 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1704 2024-05-13 13:49:49.190337 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2613 2024-05-13 13:49:49.181480 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1701 2024-05-13 13:49:49.199660 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2168 2024-05-13 13:49:49.122019 codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2399 2024-05-16 14:53:37.499708 codefly_cli-0.0.5/codefly_cli/base/v0/agent_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499646 codefly_cli-0.0.5/codefly_cli/base/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     2500 2024-05-16 14:53:37.499461 codefly_cli-0.0.5/codefly_cli/base/v0/configuration_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499745 codefly_cli-0.0.5/codefly_cli/base/v0/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-05-16 14:53:37.500444 codefly_cli-0.0.5/codefly_cli/base/v0/endpoint_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500443 codefly_cli-0.0.5/codefly_cli/base/v0/endpoint_pb2_grpc.py
+-rw-r--r--   0        0        0     2169 2024-05-16 14:53:37.500330 codefly_cli-0.0.5/codefly_cli/base/v0/environment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500340 codefly_cli-0.0.5/codefly_cli/base/v0/environment_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2024-05-16 14:53:37.500972 codefly_cli-0.0.5/codefly_cli/base/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501854 codefly_cli-0.0.5/codefly_cli/base/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2768 2024-05-16 14:53:37.501436 codefly_cli-0.0.5/codefly_cli/base/v0/network_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501580 codefly_cli-0.0.5/codefly_cli/base/v0/network_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-16 14:53:37.501802 codefly_cli-0.0.5/codefly_cli/base/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501756 codefly_cli-0.0.5/codefly_cli/base/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-16 14:53:37.501624 codefly_cli-0.0.5/codefly_cli/base/v0/scope_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501786 codefly_cli-0.0.5/codefly_cli/base/v0/scope_pb2_grpc.py
+-rw-r--r--   0        0        0     4669 2024-05-16 14:53:37.501891 codefly_cli-0.0.5/codefly_cli/base/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502450 codefly_cli-0.0.5/codefly_cli/base/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2414 2024-05-16 14:53:37.501961 codefly_cli-0.0.5/codefly_cli/base/v0/spec_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502506 codefly_cli-0.0.5/codefly_cli/base/v0/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     3318 2024-05-16 14:53:37.502732 codefly_cli-0.0.5/codefly_cli/base/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503340 codefly_cli-0.0.5/codefly_cli/base/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/buf/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.5/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.5/codefly_cli/buf/validate/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/buf/validate/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.5/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1735 2024-05-13 13:49:49.171523 codefly_cli-0.0.5/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0   105220 2024-05-13 13:49:49.169873 codefly_cli-0.0.5/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.5/codefly_cli/buf/validate/expression.proto
+-rw-r--r--   0        0        0     2292 2024-05-16 14:53:37.503962 codefly_cli-0.0.5/codefly_cli/buf/validate/expression_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503883 codefly_cli-0.0.5/codefly_cli/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1833 2024-05-13 13:49:49.173958 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/private.proto
+-rw-r--r--   0        0        0     2332 2024-05-16 14:53:37.503853 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/private_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504685 codefly_cli-0.0.5/codefly_cli/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.5/codefly_cli/buf/validate/validate.proto
+-rw-r--r--   0        0        0   144402 2024-05-16 14:53:37.506101 codefly_cli-0.0.5/codefly_cli/buf/validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504729 codefly_cli-0.0.5/codefly_cli/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/cli/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.5/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/cli/v0/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.5/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7578 2024-05-13 13:49:49.187411 codefly_cli-0.0.5/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    10048 2024-05-13 13:49:49.118488 codefly_cli-0.0.5/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0    11729 2024-05-16 14:53:37.505430 codefly_cli-0.0.5/codefly_cli/cli/v0/cli_pb2.py
+-rw-r--r--   0        0        0    28562 2024-05-16 14:53:37.504644 codefly_cli-0.0.5/codefly_cli/cli/v0/cli_pb2_grpc.py
+-rw-r--r--   0        0        0     4393 2024-05-18 18:05:46.058203 codefly_cli-0.0.5/codefly_cli/codefly.py
+-rw-r--r--   0        0        0     1517 2024-05-13 13:49:49.218228 codefly_cli-0.0.5/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1912 2024-05-13 13:49:49.220245 codefly_cli-0.0.5/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1792 2024-05-16 14:53:37.504861 codefly_cli-0.0.5/codefly_cli/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504934 codefly_cli-0.0.5/codefly_cli/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2690 2024-05-16 14:53:37.504907 codefly_cli-0.0.5/codefly_cli/google/api/http_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505129 codefly_cli-0.0.5/codefly_cli/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/observability/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.5/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/observability/v0/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-05-13 13:49:49.211153 codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1550 2024-05-13 13:49:49.209688 codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2265 2024-05-13 13:49:49.213031 codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2214 2024-05-13 13:49:49.214782 codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2474 2024-05-16 14:53:37.505558 codefly_cli-0.0.5/codefly_cli/observability/v0/dependencies_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506072 codefly_cli-0.0.5/codefly_cli/observability/v0/dependencies_pb2_grpc.py
+-rw-r--r--   0        0        0     1837 2024-05-16 14:53:37.505766 codefly_cli-0.0.5/codefly_cli/observability/v0/inventory_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505954 codefly_cli-0.0.5/codefly_cli/observability/v0/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2024-05-16 14:53:37.506417 codefly_cli-0.0.5/codefly_cli/observability/v0/logs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506415 codefly_cli-0.0.5/codefly_cli/observability/v0/logs_pb2_grpc.py
+-rw-r--r--   0        0        0     2098 2024-05-16 14:53:37.506262 codefly_cli-0.0.5/codefly_cli/observability/v0/metrics_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506455 codefly_cli-0.0.5/codefly_cli/observability/v0/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0     2985 2024-05-16 14:53:37.506432 codefly_cli-0.0.5/codefly_cli/observability/v0/sessions_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506726 codefly_cli-0.0.5/codefly_cli/observability/v0/sessions_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.5/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/agent/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.5/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/agent/v0/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.5/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3328 2024-05-13 13:49:49.194622 codefly_cli-0.0.5/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4050 2024-05-13 13:49:49.205929 codefly_cli-0.0.5/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     5107 2024-05-16 14:53:37.507542 codefly_cli-0.0.5/codefly_cli/services/agent/v0/agent_pb2.py
+-rw-r--r--   0        0        0     2895 2024-05-16 14:53:37.507520 codefly_cli-0.0.5/codefly_cli/services/agent/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     6560 2024-05-16 14:53:37.507558 codefly_cli-0.0.5/codefly_cli/services/agent/v0/communicate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507148 codefly_cli-0.0.5/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
+-rw-r--r--   0        0        0     2426 2024-05-16 14:53:37.507482 codefly_cli-0.0.5/codefly_cli/services/agent/v0/cyclonedx_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507429 codefly_cli-0.0.5/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/builder/v0/__init__.py
+-rw-r--r--   0        0        0    11603 2024-05-16 14:53:37.507453 codefly_cli-0.0.5/codefly_cli/services/builder/v0/builder_pb2.py
+-rw-r--r--   0        0        0    15720 2024-05-16 14:53:37.508035 codefly_cli-0.0.5/codefly_cli/services/builder/v0/builder_pb2_grpc.py
+-rw-r--r--   0        0        0     3239 2024-05-16 14:53:37.508589 codefly_cli-0.0.5/codefly_cli/services/builder/v0/deployment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508879 codefly_cli-0.0.5/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-05-16 14:53:37.508593 codefly_cli-0.0.5/codefly_cli/services/builder/v0/docker_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508837 codefly_cli-0.0.5/codefly_cli/services/builder/v0/docker_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/runtime/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.5/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.5/codefly_cli/services/runtime/v0/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.5/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7530 2024-05-13 13:49:49.198194 codefly_cli-0.0.5/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    11252 2024-05-16 14:53:37.509254 codefly_cli-0.0.5/codefly_cli/services/runtime/v0/runtime_pb2.py
+-rw-r--r--   0        0        0    15818 2024-05-16 14:53:37.509221 codefly_cli-0.0.5/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
+-rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.5/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.5/codefly_cli/tests/test_cli.py
+-rw-r--r--   0        0        0      481 2024-05-18 17:05:03.083406 codefly_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.5/PKG-INFO
```

### Comparing `codefly_cli-0.0.4/codefly_cli/actions/v0/module_pb2.py` & `codefly_cli-0.0.5/codefly_cli/actions/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/actions/v0/organization_pb2.py` & `codefly_cli-0.0.5/codefly_cli/actions/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/actions/v0/service_pb2.py` & `codefly_cli-0.0.5/codefly_cli/actions/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/actions/v0/workspace_pb2.py` & `codefly_cli-0.0.5/codefly_cli/actions/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/agent_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/configuration_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/endpoint_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/environment_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/module_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/network_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/network_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/organization_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/scope_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/service_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/spec_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/base/v0/workspace_pb2.py` & `codefly_cli-0.0.5/codefly_cli/base/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/BUILD.bazel` & `codefly_cli-0.0.5/codefly_cli/buf/validate/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/expression.proto` & `codefly_cli-0.0.5/codefly_cli/buf/validate/expression.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/expression_pb2.py` & `codefly_cli-0.0.5/codefly_cli/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/priv/BUILD.bazel` & `codefly_cli-0.0.5/codefly_cli/buf/validate/priv/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/priv/private.proto` & `codefly_cli-0.0.5/codefly_cli/buf/validate/priv/private.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/priv/private_pb2.py` & `codefly_cli-0.0.5/codefly_cli/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/validate.proto` & `codefly_cli-0.0.5/codefly_cli/buf/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/buf/validate/validate_pb2.py` & `codefly_cli-0.0.5/codefly_cli/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/cli/v0/cli_pb2.py` & `codefly_cli-0.0.5/codefly_cli/cli/v0/cli_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from observability.v0 import dependencies_pb2 as observability_dot_v0_dot_dependencies__pb2
 from observability.v0 import logs_pb2 as observability_dot_v0_dot_logs__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63li/v0/cli.proto\x12\x10observability.v0\x1a\x16\x62\x61se/v0/endpoint.proto\x1a\x17\x62\x61se/v0/workspace.proto\x1a\x1b\x62\x61se/v0/configuration.proto\x1a\x1dservices/agent/v0/agent.proto\x1a!services/runtime/v0/runtime.proto\x1a observability/v0/inventory.proto\x1a#observability/v0/dependencies.proto\x1a\x1bobservability/v0/logs.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"2\n\x1aGetAgentInformationRequest\x12\x14\n\x05\x61gent\x18\x01 \x01(\tR\x05\x61gent\"M\n\x12MultiGraphResponse\x12\x37\n\x06graphs\x18\x01 \x03(\x0b\x32\x1f.observability.v0.GraphResponseR\x06graphs\"`\n\x0e\x41\x63tiveResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12\x16\n\x06module\x18\x02 \x01(\tR\x06module\x12\x18\n\x07service\x18\x03 \x01(\tR\x07service\"c\n\x12RunningInformation\x12\x16\n\x06module\x18\x01 \x01(\tR\x06module\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1b\n\tagent_pid\x18\x03 \x01(\x05R\x08\x61gentPid\"a\n\x11GetAddressRequest\x12\x16\n\x06module\x18\x01 \x01(\tR\x06module\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1a\n\x08\x65ndpoint\x18\x03 \x01(\tR\x08\x65ndpoint\".\n\x12GetAddressResponse\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\"K\n\x17GetConfigurationRequest\x12\x16\n\x06module\x18\x01 \x01(\tR\x06module\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\"X\n\x18GetConfigurationResponse\x12<\n\rconfiguration\x18\x01 \x01(\x0b\x32\x16.base.v0.ConfigurationR\rconfiguration\"[\n\x19GetConfigurationsResponse\x12>\n\x0e\x63onfigurations\x18\x01 \x03(\x0b\x32\x16.base.v0.ConfigurationR\x0e\x63onfigurations\"\"\n\nFlowStatus\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\"\x11\n\x0fStopFlowRequest\"\x12\n\x10StopFlowResponse\"\x14\n\x12\x44\x65stroyFlowRequest\"\x15\n\x13\x44\x65stroyFlowResponse2\x8e\x0f\n\x03\x43LI\x12\x45\n\x04Ping\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\r\x82\xd3\xe4\x93\x02\x07\x12\x05/ping\x12\x8c\x01\n\x13GetAgentInformation\x12,.observability.v0.GetAgentInformationRequest\x1a#.services.agent.v0.AgentInformation\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/agent/{agent}/information\x12\x61\n\x15GetWorkspaceInventory\x12\x16.google.protobuf.Empty\x1a\x12.base.v0.Workspace\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/workspace/inventory\x12\x8a\x01\n\"GetWorkspaceServiceDependencyGraph\x12\x16.google.protobuf.Empty\x1a\x1f.observability.v0.GraphResponse\"+\x82\xd3\xe4\x93\x02%\x12#/workspace/service-dependency-graph\x12\x91\x01\n(GetWorkspacePublicModulesDependencyGraph\x12\x16.google.protobuf.Empty\x1a$.observability.v0.MultiGraphResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/workspace/public-modules-graph\x12\x65\n\tGetActive\x12\x16.google.protobuf.Empty\x1a .observability.v0.ActiveResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/workspace/information\x12\x9b\x01\n\x0cGetAddresses\x12#.observability.v0.GetAddressRequest\x1a$.observability.v0.GetAddressResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/workspace/network-mapping/{module}/{service}/{endpoint}\x12\x9e\x01\n\x10GetConfiguration\x12).observability.v0.GetConfigurationRequest\x1a*.observability.v0.GetConfigurationResponse\"3\x82\xd3\xe4\x93\x02-\x12+/workspace/configuration/{module}/{service}\x12\xba\x01\n\x1dGetDependenciesConfigurations\x12).observability.v0.GetConfigurationRequest\x1a+.observability.v0.GetConfigurationsResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/workspace/dependencies-configurations/{module}/{service}\x12\xb0\x01\n\x18GetRuntimeConfigurations\x12).observability.v0.GetConfigurationRequest\x1a+.observability.v0.GetConfigurationsResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/workspace/runtime-configurations/{module}/{service}\x12P\n\x04Logs\x12\x16.google.protobuf.Empty\x1a\x15.observability.v0.Log\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/workspace/logs0\x01\x12p\n\x10\x41\x63tiveLogHistory\x12\x1c.observability.v0.LogRequest\x1a\x1d.observability.v0.LogResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/workspace/logs/history\x12\x65\n\rGetFlowStatus\x12\x16.google.protobuf.Empty\x1a\x1c.observability.v0.FlowStatus\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/workspace/flow/status\x12o\n\x08StopFlow\x12!.observability.v0.StopFlowRequest\x1a\".observability.v0.StopFlowResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x14/workspace/flow/stop\x12{\n\x0b\x44\x65stroyFlow\x12$.observability.v0.DestroyFlowRequest\x1a%.observability.v0.DestroyFlowResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/workspace/flow/destroyB\xb2\x01\n\x14\x63om.observability.v0B\x08\x43liProtoP\x01Z/github.com/codefly-dev/core/generated/go/cli/v0\xa2\x02\x03OVX\xaa\x02\x10Observability.V0\xca\x02\x10Observability\\V0\xe2\x02\x1cObservability\\V0\\GPBMetadata\xea\x02\x11Observability::V0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63li/v0/cli.proto\x12\x10observability.v0\x1a\x16\x62\x61se/v0/endpoint.proto\x1a\x17\x62\x61se/v0/workspace.proto\x1a\x1b\x62\x61se/v0/configuration.proto\x1a\x1dservices/agent/v0/agent.proto\x1a!services/runtime/v0/runtime.proto\x1a observability/v0/inventory.proto\x1a#observability/v0/dependencies.proto\x1a\x1bobservability/v0/logs.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"2\n\x1aGetAgentInformationRequest\x12\x14\n\x05\x61gent\x18\x01 \x01(\tR\x05\x61gent\"M\n\x12MultiGraphResponse\x12\x37\n\x06graphs\x18\x01 \x03(\x0b\x32\x1f.observability.v0.GraphResponseR\x06graphs\"`\n\x0e\x41\x63tiveResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12\x16\n\x06module\x18\x02 \x01(\tR\x06module\x12\x18\n\x07service\x18\x03 \x01(\tR\x07service\"c\n\x12RunningInformation\x12\x16\n\x06module\x18\x01 \x01(\tR\x06module\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1b\n\tagent_pid\x18\x03 \x01(\x05R\x08\x61gentPid\"a\n\x11GetAddressRequest\x12\x16\n\x06module\x18\x01 \x01(\tR\x06module\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\x12\x1a\n\x08\x65ndpoint\x18\x03 \x01(\tR\x08\x65ndpoint\".\n\x12GetAddressResponse\x12\x18\n\x07\x61\x64\x64ress\x18\x01 \x01(\tR\x07\x61\x64\x64ress\"K\n\x17GetConfigurationRequest\x12\x16\n\x06module\x18\x01 \x01(\tR\x06module\x12\x18\n\x07service\x18\x02 \x01(\tR\x07service\"X\n\x18GetConfigurationResponse\x12<\n\rconfiguration\x18\x01 \x01(\x0b\x32\x16.base.v0.ConfigurationR\rconfiguration\"[\n\x19GetConfigurationsResponse\x12>\n\x0e\x63onfigurations\x18\x01 \x03(\x0b\x32\x16.base.v0.ConfigurationR\x0e\x63onfigurations\"\"\n\nFlowStatus\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\"\x11\n\x0fStopFlowRequest\"\x12\n\x10StopFlowResponse\"\x14\n\x12\x44\x65stroyFlowRequest\"\x15\n\x13\x44\x65stroyFlowResponse2\x90\x0f\n\x03\x43LI\x12\x45\n\x04Ping\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\r\x82\xd3\xe4\x93\x02\x07\x12\x05/ping\x12\x8c\x01\n\x13GetAgentInformation\x12,.observability.v0.GetAgentInformationRequest\x1a#.services.agent.v0.AgentInformation\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/agent/{agent}/information\x12\x61\n\x15GetWorkspaceInventory\x12\x16.google.protobuf.Empty\x1a\x12.base.v0.Workspace\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/workspace/inventory\x12\x8a\x01\n\"GetWorkspaceServiceDependencyGraph\x12\x16.google.protobuf.Empty\x1a\x1f.observability.v0.GraphResponse\"+\x82\xd3\xe4\x93\x02%\x12#/workspace/service-dependency-graph\x12\x93\x01\n(GetWorkspacePublicModulesDependencyGraph\x12\x16.google.protobuf.Empty\x1a$.observability.v0.MultiGraphResponse\")\x82\xd3\xe4\x93\x02#\x12!/workspace/public-endpoints-graph\x12\x65\n\tGetActive\x12\x16.google.protobuf.Empty\x1a .observability.v0.ActiveResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/workspace/information\x12\x9b\x01\n\x0cGetAddresses\x12#.observability.v0.GetAddressRequest\x1a$.observability.v0.GetAddressResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/workspace/network-mapping/{module}/{service}/{endpoint}\x12\x9e\x01\n\x10GetConfiguration\x12).observability.v0.GetConfigurationRequest\x1a*.observability.v0.GetConfigurationResponse\"3\x82\xd3\xe4\x93\x02-\x12+/workspace/configuration/{module}/{service}\x12\xba\x01\n\x1dGetDependenciesConfigurations\x12).observability.v0.GetConfigurationRequest\x1a+.observability.v0.GetConfigurationsResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/workspace/dependencies-configurations/{module}/{service}\x12\xb0\x01\n\x18GetRuntimeConfigurations\x12).observability.v0.GetConfigurationRequest\x1a+.observability.v0.GetConfigurationsResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/workspace/runtime-configurations/{module}/{service}\x12P\n\x04Logs\x12\x16.google.protobuf.Empty\x1a\x15.observability.v0.Log\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/workspace/logs0\x01\x12p\n\x10\x41\x63tiveLogHistory\x12\x1c.observability.v0.LogRequest\x1a\x1d.observability.v0.LogResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/workspace/logs/history\x12\x65\n\rGetFlowStatus\x12\x16.google.protobuf.Empty\x1a\x1c.observability.v0.FlowStatus\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/workspace/flow/status\x12o\n\x08StopFlow\x12!.observability.v0.StopFlowRequest\x1a\".observability.v0.StopFlowResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x14/workspace/flow/stop\x12{\n\x0b\x44\x65stroyFlow\x12$.observability.v0.DestroyFlowRequest\x1a%.observability.v0.DestroyFlowResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x17/workspace/flow/destroyB\xb2\x01\n\x14\x63om.observability.v0B\x08\x43liProtoP\x01Z/github.com/codefly-dev/core/generated/go/cli/v0\xa2\x02\x03OVX\xaa\x02\x10Observability.V0\xca\x02\x10Observability\\V0\xe2\x02\x1cObservability\\V0\\GPBMetadata\xea\x02\x11Observability::V0b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cli.v0.cli_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\024com.observability.v0B\010CliProtoP\001Z/github.com/codefly-dev/core/generated/go/cli/v0\242\002\003OVX\252\002\020Observability.V0\312\002\020Observability\\V0\342\002\034Observability\\V0\\GPBMetadata\352\002\021Observability::V0'
@@ -38,15 +38,15 @@
   _globals['_CLI'].methods_by_name['GetAgentInformation']._loaded_options = None
   _globals['_CLI'].methods_by_name['GetAgentInformation']._serialized_options = b'\202\323\344\223\002\034\022\032/agent/{agent}/information'
   _globals['_CLI'].methods_by_name['GetWorkspaceInventory']._loaded_options = None
   _globals['_CLI'].methods_by_name['GetWorkspaceInventory']._serialized_options = b'\202\323\344\223\002\026\022\024/workspace/inventory'
   _globals['_CLI'].methods_by_name['GetWorkspaceServiceDependencyGraph']._loaded_options = None
   _globals['_CLI'].methods_by_name['GetWorkspaceServiceDependencyGraph']._serialized_options = b'\202\323\344\223\002%\022#/workspace/service-dependency-graph'
   _globals['_CLI'].methods_by_name['GetWorkspacePublicModulesDependencyGraph']._loaded_options = None
-  _globals['_CLI'].methods_by_name['GetWorkspacePublicModulesDependencyGraph']._serialized_options = b'\202\323\344\223\002!\022\037/workspace/public-modules-graph'
+  _globals['_CLI'].methods_by_name['GetWorkspacePublicModulesDependencyGraph']._serialized_options = b'\202\323\344\223\002#\022!/workspace/public-endpoints-graph'
   _globals['_CLI'].methods_by_name['GetActive']._loaded_options = None
   _globals['_CLI'].methods_by_name['GetActive']._serialized_options = b'\202\323\344\223\002\030\022\026/workspace/information'
   _globals['_CLI'].methods_by_name['GetAddresses']._loaded_options = None
   _globals['_CLI'].methods_by_name['GetAddresses']._serialized_options = b'\202\323\344\223\002:\0228/workspace/network-mapping/{module}/{service}/{endpoint}'
   _globals['_CLI'].methods_by_name['GetConfiguration']._loaded_options = None
   _globals['_CLI'].methods_by_name['GetConfiguration']._serialized_options = b'\202\323\344\223\002-\022+/workspace/configuration/{module}/{service}'
   _globals['_CLI'].methods_by_name['GetDependenciesConfigurations']._loaded_options = None
@@ -88,9 +88,9 @@
   _globals['_STOPFLOWRESPONSE']._serialized_start=1166
   _globals['_STOPFLOWRESPONSE']._serialized_end=1184
   _globals['_DESTROYFLOWREQUEST']._serialized_start=1186
   _globals['_DESTROYFLOWREQUEST']._serialized_end=1206
   _globals['_DESTROYFLOWRESPONSE']._serialized_start=1208
   _globals['_DESTROYFLOWRESPONSE']._serialized_end=1229
   _globals['_CLI']._serialized_start=1232
-  _globals['_CLI']._serialized_end=3166
+  _globals['_CLI']._serialized_end=3168
 # @@protoc_insertion_point(module_scope)
```

### Comparing `codefly_cli-0.0.4/codefly_cli/cli/v0/cli_pb2_grpc.py` & `codefly_cli-0.0.5/codefly_cli/cli/v0/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/codefly.py` & `codefly_cli-0.0.5/codefly_cli/codefly.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,27 +18,35 @@
 
 from google.protobuf.empty_pb2 import Empty
 
 
 def filter_configurations(configurations: List[configuration.Configuration], runtime_context: str) -> List[configuration.Configuration]:
     return [conf for conf in configurations if conf.runtime_context.kind == runtime_context]
 
+@pytest.fixture
+def with_dependencies():
+    launcher = Launcher(show_cli_output=True)
+    launcher.start()
+    codefly.init("..")
+    yield
+    launcher.close()
+
 class Launcher:
     def __init__(self, root: str = "..", scope: str = "", show_cli_output: bool = False, keep_alive: bool = False):
         self.cmd = None
         self.cli = None
         self.show_cli_output = show_cli_output
         self.dir = find_service_dir(os.path.abspath(root))
         print(f"running in {self.dir}")
         self.scope = scope
         self.keep_alive = keep_alive
-        self.module = "python-visitors" #codefly.get_module()
-        self.service = "visits" #codefly.get_service()
-        self.unique = "python-visitors/visits" #codefly.get_unique()
-        self.runtime_context = "native" # TODO: fix
+        self.module = codefly.get_module()
+        self.service = codefly.get_service()
+        self.unique = codefly.get_unique()
+        self.runtime_context = codefly.runtime_context()
 
 
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `codefly_cli-0.0.4/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/google/api/annotations_pb2.py` & `codefly_cli-0.0.5/codefly_cli/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/google/api/http_pb2.py` & `codefly_cli-0.0.5/codefly_cli/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/dependencies_pb2.py` & `codefly_cli-0.0.5/codefly_cli/observability/v0/dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/inventory_pb2.py` & `codefly_cli-0.0.5/codefly_cli/observability/v0/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/logs_pb2.py` & `codefly_cli-0.0.5/codefly_cli/observability/v0/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/metrics_pb2.py` & `codefly_cli-0.0.5/codefly_cli/observability/v0/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/observability/v0/sessions_pb2.py` & `codefly_cli-0.0.5/codefly_cli/observability/v0/sessions_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/agent/v0/agent_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/agent/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/agent/v0/agent_pb2_grpc.py` & `codefly_cli-0.0.5/codefly_cli/services/agent/v0/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/agent/v0/communicate_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/agent/v0/communicate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/agent/v0/cyclonedx_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/agent/v0/cyclonedx_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/builder/v0/builder_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/builder/v0/builder_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/builder/v0/builder_pb2_grpc.py` & `codefly_cli-0.0.5/codefly_cli/services/builder/v0/builder_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/builder/v0/deployment_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/builder/v0/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/builder/v0/docker_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/builder/v0/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc` & `codefly_cli-0.0.5/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/services/runtime/v0/runtime_pb2.py` & `codefly_cli-0.0.5/codefly_cli/services/runtime/v0/runtime_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from base.v0 import endpoint_pb2 as base_dot_v0_dot_endpoint__pb2
 from base.v0 import network_pb2 as base_dot_v0_dot_network__pb2
 from base.v0 import configuration_pb2 as base_dot_v0_dot_configuration__pb2
 from services.agent.v0 import agent_pb2 as services_dot_agent_dot_v0_dot_agent__pb2
 from services.agent.v0 import communicate_pb2 as services_dot_agent_dot_v0_dot_communicate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!services/runtime/v0/runtime.proto\x12\x13services.runtime.v0\x1a\x13\x62\x61se/v0/scope.proto\x1a\x12\x62\x61se/v0/spec.proto\x1a\x19\x62\x61se/v0/environment.proto\x1a\x15\x62\x61se/v0/service.proto\x1a\x16\x62\x61se/v0/endpoint.proto\x1a\x15\x62\x61se/v0/network.proto\x1a\x1b\x62\x61se/v0/configuration.proto\x1a\x1dservices/agent/v0/agent.proto\x1a#services/agent/v0/communicate.proto\"\x91\x01\n\nLoadStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.LoadStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"+\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05READY\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"\xc9\x01\n\x0bLoadRequest\x12\'\n\x0f\x64\x65veloper_debug\x18\x01 \x01(\x08R\x0e\x64\x65veloperDebug\x12#\n\rdisable_catch\x18\x02 \x01(\x08R\x0c\x64isableCatch\x12\x34\n\x08identity\x18\x03 \x01(\x0b\x32\x18.base.v0.ServiceIdentityR\x08identity\x12\x36\n\x0b\x65nvironment\x18\x04 \x01(\x0b\x32\x14.base.v0.EnvironmentR\x0b\x65nvironment\"\xa4\x01\n\x0cLoadResponse\x12*\n\x07version\x18\x01 \x01(\x0b\x32\x10.base.v0.VersionR\x07version\x12\x37\n\x06status\x18\x02 \x01(\x0b\x32\x1f.services.runtime.v0.LoadStatusR\x06status\x12/\n\tendpoints\x18\x03 \x03(\x0b\x32\x11.base.v0.EndpointR\tendpoints\"\x91\x01\n\nInitStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.InitStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"+\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05READY\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"\x85\x03\n\x0bInitRequest\x12@\n\x0fruntime_context\x18\x01 \x01(\x0b\x32\x17.base.v0.RuntimeContextR\x0eruntimeContext\x12<\n\rconfiguration\x18\x02 \x01(\x0b\x32\x16.base.v0.ConfigurationR\rconfiguration\x12S\n\x19proposed_network_mappings\x18\x03 \x03(\x0b\x32\x17.base.v0.NetworkMappingR\x17proposedNetworkMappings\x12H\n\x16\x64\x65pendencies_endpoints\x18\x04 \x03(\x0b\x32\x11.base.v0.EndpointR\x15\x64\x65pendenciesEndpoints\x12W\n\x1b\x64\x65pendencies_configurations\x18\x05 \x03(\x0b\x32\x16.base.v0.ConfigurationR\x1a\x64\x65pendenciesConfigurations\"\x9c\x02\n\x0cInitResponse\x12\x37\n\x06status\x18\x01 \x01(\x0b\x32\x1f.services.runtime.v0.InitStatusR\x06status\x12@\n\x0fruntime_context\x18\x02 \x01(\x0b\x32\x17.base.v0.RuntimeContextR\x0eruntimeContext\x12\x42\n\x10network_mappings\x18\x03 \x03(\x0b\x32\x17.base.v0.NetworkMappingR\x0fnetworkMappings\x12M\n\x16runtime_configurations\x18\x04 \x03(\x0b\x32\x16.base.v0.ConfigurationR\x15runtimeConfigurations\"\x91\x01\n\x0cStartRequest\x12$\n\x05specs\x18\x01 \x01(\x0b\x32\x0e.base.v0.SpecsR\x05specs\x12[\n\x1d\x64\x65pendencies_network_mappings\x18\x02 \x03(\x0b\x32\x17.base.v0.NetworkMappingR\x1b\x64\x65pendenciesNetworkMappings\"\x95\x01\n\x0bStartStatus\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.services.runtime.v0.StartStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07STARTED\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"I\n\rStartResponse\x12\x38\n\x06status\x18\x01 \x01(\x0b\x32 .services.runtime.v0.StartStatusR\x06status\"\x93\x01\n\nTestStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.TestStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"O\n\x0bTestRequest\x12@\n\x0fruntime_context\x18\x01 \x01(\x0b\x32\x17.base.v0.RuntimeContextR\x0eruntimeContext\"G\n\x0cTestResponse\x12\x37\n\x06status\x18\x01 \x01(\x0b\x32\x1f.services.runtime.v0.TestStatusR\x06status\"\r\n\x0bStopRequest\"\x93\x01\n\nStopStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.StopStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"G\n\x0cStopResponse\x12\x37\n\x06status\x18\x01 \x01(\x0b\x32\x1f.services.runtime.v0.StopStatusR\x06status\"\x10\n\x0e\x44\x65stroyRequest\"\x99\x01\n\rDestroyStatus\x12?\n\x05state\x18\x01 \x01(\x0e\x32).services.runtime.v0.DestroyStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"M\n\x0f\x44\x65stroyResponse\x12:\n\x06status\x18\x01 \x01(\x0b\x32\".services.runtime.v0.DestroyStatusR\x06status\"\x14\n\x12InformationRequest\"\x8c\x01\n\x0c\x44\x65siredState\x12=\n\x05stage\x18\x01 \x01(\x0e\x32\'.services.runtime.v0.DesiredState.StageR\x05stage\"=\n\x05Stage\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NOOP\x10\x01\x12\x08\n\x04LOAD\x10\x02\x12\x08\n\x04INIT\x10\x03\x12\t\n\x05START\x10\x04\"\xf5\x03\n\x13InformationResponse\x12\x46\n\rdesired_state\x18\x01 \x01(\x0b\x32!.services.runtime.v0.DesiredStateR\x0c\x64\x65siredState\x12@\n\x0bload_status\x18\x02 \x01(\x0b\x32\x1f.services.runtime.v0.LoadStatusR\nloadStatus\x12@\n\x0binit_status\x18\x03 \x01(\x0b\x32\x1f.services.runtime.v0.InitStatusR\ninitStatus\x12\x43\n\x0cstart_status\x18\x04 \x01(\x0b\x32 .services.runtime.v0.StartStatusR\x0bstartStatus\x12@\n\x0bstop_status\x18\x05 \x01(\x0b\x32\x1f.services.runtime.v0.StopStatusR\nstopStatus\x12I\n\x0e\x44\x65stroy_status\x18\x06 \x01(\x0b\x32\".services.runtime.v0.DestroyStatusR\rDestroyStatus\x12@\n\x0btest_status\x18\x07 \x01(\x0b\x32\x1f.services.runtime.v0.TestStatusR\ntestStatus2\xa6\x05\n\x07Runtime\x12M\n\x04Load\x12 .services.runtime.v0.LoadRequest\x1a!.services.runtime.v0.LoadResponse\"\x00\x12M\n\x04Init\x12 .services.runtime.v0.InitRequest\x1a!.services.runtime.v0.InitResponse\"\x00\x12P\n\x05Start\x12!.services.runtime.v0.StartRequest\x1a\".services.runtime.v0.StartResponse\"\x00\x12M\n\x04Stop\x12 .services.runtime.v0.StopRequest\x1a!.services.runtime.v0.StopResponse\"\x00\x12V\n\x07\x44\x65stroy\x12#.services.runtime.v0.DestroyRequest\x1a$.services.runtime.v0.DestroyResponse\"\x00\x12M\n\x04Test\x12 .services.runtime.v0.TestRequest\x1a!.services.runtime.v0.TestResponse\"\x00\x12\x62\n\x0bInformation\x12\'.services.runtime.v0.InformationRequest\x1a(.services.runtime.v0.InformationResponse\"\x00\x12Q\n\x0b\x43ommunicate\x12\x19.services.agent.v0.Engage\x1a%.services.agent.v0.InformationRequest\"\x00\x42\xd3\x01\n\x17\x63om.services.runtime.v0B\x0cRuntimeProtoP\x01Z<github.com/codefly-dev/core/generated/go/services/runtime/v0\xa2\x02\x03SRV\xaa\x02\x13Services.Runtime.V0\xca\x02\x13Services\\Runtime\\V0\xe2\x02\x1fServices\\Runtime\\V0\\GPBMetadata\xea\x02\x15Services::Runtime::V0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!services/runtime/v0/runtime.proto\x12\x13services.runtime.v0\x1a\x13\x62\x61se/v0/scope.proto\x1a\x12\x62\x61se/v0/spec.proto\x1a\x19\x62\x61se/v0/environment.proto\x1a\x15\x62\x61se/v0/service.proto\x1a\x16\x62\x61se/v0/endpoint.proto\x1a\x15\x62\x61se/v0/network.proto\x1a\x1b\x62\x61se/v0/configuration.proto\x1a\x1dservices/agent/v0/agent.proto\x1a#services/agent/v0/communicate.proto\"\x91\x01\n\nLoadStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.LoadStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"+\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05READY\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"\xc9\x01\n\x0bLoadRequest\x12\'\n\x0f\x64\x65veloper_debug\x18\x01 \x01(\x08R\x0e\x64\x65veloperDebug\x12#\n\rdisable_catch\x18\x02 \x01(\x08R\x0c\x64isableCatch\x12\x34\n\x08identity\x18\x03 \x01(\x0b\x32\x18.base.v0.ServiceIdentityR\x08identity\x12\x36\n\x0b\x65nvironment\x18\x04 \x01(\x0b\x32\x14.base.v0.EnvironmentR\x0b\x65nvironment\"\xa4\x01\n\x0cLoadResponse\x12*\n\x07version\x18\x01 \x01(\x0b\x32\x10.base.v0.VersionR\x07version\x12\x37\n\x06status\x18\x02 \x01(\x0b\x32\x1f.services.runtime.v0.LoadStatusR\x06status\x12/\n\tendpoints\x18\x03 \x03(\x0b\x32\x11.base.v0.EndpointR\tendpoints\"\x91\x01\n\nInitStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.InitStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"+\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05READY\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"\x85\x03\n\x0bInitRequest\x12@\n\x0fruntime_context\x18\x01 \x01(\x0b\x32\x17.base.v0.RuntimeContextR\x0eruntimeContext\x12<\n\rconfiguration\x18\x02 \x01(\x0b\x32\x16.base.v0.ConfigurationR\rconfiguration\x12S\n\x19proposed_network_mappings\x18\x03 \x03(\x0b\x32\x17.base.v0.NetworkMappingR\x17proposedNetworkMappings\x12H\n\x16\x64\x65pendencies_endpoints\x18\x04 \x03(\x0b\x32\x11.base.v0.EndpointR\x15\x64\x65pendenciesEndpoints\x12W\n\x1b\x64\x65pendencies_configurations\x18\x05 \x03(\x0b\x32\x16.base.v0.ConfigurationR\x1a\x64\x65pendenciesConfigurations\"\x9c\x02\n\x0cInitResponse\x12\x37\n\x06status\x18\x01 \x01(\x0b\x32\x1f.services.runtime.v0.InitStatusR\x06status\x12@\n\x0fruntime_context\x18\x02 \x01(\x0b\x32\x17.base.v0.RuntimeContextR\x0eruntimeContext\x12\x42\n\x10network_mappings\x18\x03 \x03(\x0b\x32\x17.base.v0.NetworkMappingR\x0fnetworkMappings\x12M\n\x16runtime_configurations\x18\x04 \x03(\x0b\x32\x16.base.v0.ConfigurationR\x15runtimeConfigurations\"\x91\x01\n\x0cStartRequest\x12$\n\x05specs\x18\x01 \x01(\x0b\x32\x0e.base.v0.SpecsR\x05specs\x12[\n\x1d\x64\x65pendencies_network_mappings\x18\x02 \x03(\x0b\x32\x17.base.v0.NetworkMappingR\x1b\x64\x65pendenciesNetworkMappings\"\x95\x01\n\x0bStartStatus\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.services.runtime.v0.StartStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07STARTED\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"I\n\rStartResponse\x12\x38\n\x06status\x18\x01 \x01(\x0b\x32 .services.runtime.v0.StartStatusR\x06status\"\x93\x01\n\nTestStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.TestStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"\r\n\x0bTestRequest\"G\n\x0cTestResponse\x12\x37\n\x06status\x18\x01 \x01(\x0b\x32\x1f.services.runtime.v0.TestStatusR\x06status\"\r\n\x0bStopRequest\"\x93\x01\n\nStopStatus\x12<\n\x05state\x18\x01 \x01(\x0e\x32&.services.runtime.v0.StopStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"G\n\x0cStopResponse\x12\x37\n\x06status\x18\x01 \x01(\x0b\x32\x1f.services.runtime.v0.StopStatusR\x06status\"\x10\n\x0e\x44\x65stroyRequest\"\x99\x01\n\rDestroyStatus\x12?\n\x05state\x18\x01 \x01(\x0e\x32).services.runtime.v0.DestroyStatus.StatusR\x05state\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\"-\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\t\n\x05\x45RROR\x10\x02\"M\n\x0f\x44\x65stroyResponse\x12:\n\x06status\x18\x01 \x01(\x0b\x32\".services.runtime.v0.DestroyStatusR\x06status\"\x14\n\x12InformationRequest\"\x8c\x01\n\x0c\x44\x65siredState\x12=\n\x05stage\x18\x01 \x01(\x0e\x32\'.services.runtime.v0.DesiredState.StageR\x05stage\"=\n\x05Stage\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NOOP\x10\x01\x12\x08\n\x04LOAD\x10\x02\x12\x08\n\x04INIT\x10\x03\x12\t\n\x05START\x10\x04\"\xf5\x03\n\x13InformationResponse\x12\x46\n\rdesired_state\x18\x01 \x01(\x0b\x32!.services.runtime.v0.DesiredStateR\x0c\x64\x65siredState\x12@\n\x0bload_status\x18\x02 \x01(\x0b\x32\x1f.services.runtime.v0.LoadStatusR\nloadStatus\x12@\n\x0binit_status\x18\x03 \x01(\x0b\x32\x1f.services.runtime.v0.InitStatusR\ninitStatus\x12\x43\n\x0cstart_status\x18\x04 \x01(\x0b\x32 .services.runtime.v0.StartStatusR\x0bstartStatus\x12@\n\x0bstop_status\x18\x05 \x01(\x0b\x32\x1f.services.runtime.v0.StopStatusR\nstopStatus\x12I\n\x0e\x44\x65stroy_status\x18\x06 \x01(\x0b\x32\".services.runtime.v0.DestroyStatusR\rDestroyStatus\x12@\n\x0btest_status\x18\x07 \x01(\x0b\x32\x1f.services.runtime.v0.TestStatusR\ntestStatus2\xa6\x05\n\x07Runtime\x12M\n\x04Load\x12 .services.runtime.v0.LoadRequest\x1a!.services.runtime.v0.LoadResponse\"\x00\x12M\n\x04Init\x12 .services.runtime.v0.InitRequest\x1a!.services.runtime.v0.InitResponse\"\x00\x12P\n\x05Start\x12!.services.runtime.v0.StartRequest\x1a\".services.runtime.v0.StartResponse\"\x00\x12M\n\x04Stop\x12 .services.runtime.v0.StopRequest\x1a!.services.runtime.v0.StopResponse\"\x00\x12V\n\x07\x44\x65stroy\x12#.services.runtime.v0.DestroyRequest\x1a$.services.runtime.v0.DestroyResponse\"\x00\x12M\n\x04Test\x12 .services.runtime.v0.TestRequest\x1a!.services.runtime.v0.TestResponse\"\x00\x12\x62\n\x0bInformation\x12\'.services.runtime.v0.InformationRequest\x1a(.services.runtime.v0.InformationResponse\"\x00\x12Q\n\x0b\x43ommunicate\x12\x19.services.agent.v0.Engage\x1a%.services.agent.v0.InformationRequest\"\x00\x42\xd3\x01\n\x17\x63om.services.runtime.v0B\x0cRuntimeProtoP\x01Z<github.com/codefly-dev/core/generated/go/services/runtime/v0\xa2\x02\x03SRV\xaa\x02\x13Services.Runtime.V0\xca\x02\x13Services\\Runtime\\V0\xe2\x02\x1fServices\\Runtime\\V0\\GPBMetadata\xea\x02\x15Services::Runtime::V0b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'services.runtime.v0.runtime_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\027com.services.runtime.v0B\014RuntimeProtoP\001Z<github.com/codefly-dev/core/generated/go/services/runtime/v0\242\002\003SRV\252\002\023Services.Runtime.V0\312\002\023Services\\Runtime\\V0\342\002\037Services\\Runtime\\V0\\GPBMetadata\352\002\025Services::Runtime::V0'
@@ -56,37 +56,37 @@
   _globals['_STARTRESPONSE']._serialized_start=1939
   _globals['_STARTRESPONSE']._serialized_end=2012
   _globals['_TESTSTATUS']._serialized_start=2015
   _globals['_TESTSTATUS']._serialized_end=2162
   _globals['_TESTSTATUS_STATUS']._serialized_start=2117
   _globals['_TESTSTATUS_STATUS']._serialized_end=2162
   _globals['_TESTREQUEST']._serialized_start=2164
-  _globals['_TESTREQUEST']._serialized_end=2243
-  _globals['_TESTRESPONSE']._serialized_start=2245
-  _globals['_TESTRESPONSE']._serialized_end=2316
-  _globals['_STOPREQUEST']._serialized_start=2318
-  _globals['_STOPREQUEST']._serialized_end=2331
-  _globals['_STOPSTATUS']._serialized_start=2334
-  _globals['_STOPSTATUS']._serialized_end=2481
+  _globals['_TESTREQUEST']._serialized_end=2177
+  _globals['_TESTRESPONSE']._serialized_start=2179
+  _globals['_TESTRESPONSE']._serialized_end=2250
+  _globals['_STOPREQUEST']._serialized_start=2252
+  _globals['_STOPREQUEST']._serialized_end=2265
+  _globals['_STOPSTATUS']._serialized_start=2268
+  _globals['_STOPSTATUS']._serialized_end=2415
   _globals['_STOPSTATUS_STATUS']._serialized_start=2117
   _globals['_STOPSTATUS_STATUS']._serialized_end=2162
-  _globals['_STOPRESPONSE']._serialized_start=2483
-  _globals['_STOPRESPONSE']._serialized_end=2554
-  _globals['_DESTROYREQUEST']._serialized_start=2556
-  _globals['_DESTROYREQUEST']._serialized_end=2572
-  _globals['_DESTROYSTATUS']._serialized_start=2575
-  _globals['_DESTROYSTATUS']._serialized_end=2728
+  _globals['_STOPRESPONSE']._serialized_start=2417
+  _globals['_STOPRESPONSE']._serialized_end=2488
+  _globals['_DESTROYREQUEST']._serialized_start=2490
+  _globals['_DESTROYREQUEST']._serialized_end=2506
+  _globals['_DESTROYSTATUS']._serialized_start=2509
+  _globals['_DESTROYSTATUS']._serialized_end=2662
   _globals['_DESTROYSTATUS_STATUS']._serialized_start=2117
   _globals['_DESTROYSTATUS_STATUS']._serialized_end=2162
-  _globals['_DESTROYRESPONSE']._serialized_start=2730
-  _globals['_DESTROYRESPONSE']._serialized_end=2807
-  _globals['_INFORMATIONREQUEST']._serialized_start=2809
-  _globals['_INFORMATIONREQUEST']._serialized_end=2829
-  _globals['_DESIREDSTATE']._serialized_start=2832
-  _globals['_DESIREDSTATE']._serialized_end=2972
-  _globals['_DESIREDSTATE_STAGE']._serialized_start=2911
-  _globals['_DESIREDSTATE_STAGE']._serialized_end=2972
-  _globals['_INFORMATIONRESPONSE']._serialized_start=2975
-  _globals['_INFORMATIONRESPONSE']._serialized_end=3476
-  _globals['_RUNTIME']._serialized_start=3479
-  _globals['_RUNTIME']._serialized_end=4157
+  _globals['_DESTROYRESPONSE']._serialized_start=2664
+  _globals['_DESTROYRESPONSE']._serialized_end=2741
+  _globals['_INFORMATIONREQUEST']._serialized_start=2743
+  _globals['_INFORMATIONREQUEST']._serialized_end=2763
+  _globals['_DESIREDSTATE']._serialized_start=2766
+  _globals['_DESIREDSTATE']._serialized_end=2906
+  _globals['_DESIREDSTATE_STAGE']._serialized_start=2845
+  _globals['_DESIREDSTATE_STAGE']._serialized_end=2906
+  _globals['_INFORMATIONRESPONSE']._serialized_start=2909
+  _globals['_INFORMATIONRESPONSE']._serialized_end=3410
+  _globals['_RUNTIME']._serialized_start=3413
+  _globals['_RUNTIME']._serialized_end=4091
 # @@protoc_insertion_point(module_scope)
```

### Comparing `codefly_cli-0.0.4/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py` & `codefly_cli-0.0.5/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc` & `codefly_cli-0.0.5/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.4/PKG-INFO` & `codefly_cli-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: codefly-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Antoine Toussaint
 Author-email: antoine.toussaint@codefly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
-Requires-Dist: codefly-sdk (>=0.0.12,<0.0.13)
+Requires-Dist: codefly-sdk (>=0.0.13,<0.0.14)
 Requires-Dist: grpcio (>=1.63.0,<2.0.0)
 Requires-Dist: grpclib (>=0.4.7,<0.5.0)
 Requires-Dist: protobuf (>=5.26.1,<6.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
```


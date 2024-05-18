# Comparing `tmp/codefly_cli-0.0.6.tar.gz` & `tmp/codefly_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefly_cli-0.0.6.tar", max compression
+gzip compressed data, was "codefly_cli-0.0.7.tar", max compression
```

## Comparing `codefly_cli-0.0.6.tar` & `codefly_cli-0.0.7.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.6/codefly_cli/actions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/actions/v0/__init__.py
--rw-r--r--   0        0        0     2004 2024-05-16 14:53:37.499836 codefly_cli-0.0.6/codefly_cli/actions/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499681 codefly_cli-0.0.6/codefly_cli/actions/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2009 2024-05-16 14:53:37.499220 codefly_cli-0.0.6/codefly_cli/actions/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499510 codefly_cli-0.0.6/codefly_cli/actions/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     3743 2024-05-16 14:53:37.499953 codefly_cli-0.0.6/codefly_cli/actions/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499899 codefly_cli-0.0.6/codefly_cli/actions/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2588 2024-05-16 14:53:37.499937 codefly_cli-0.0.6/codefly_cli/actions/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499877 codefly_cli-0.0.6/codefly_cli/actions/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.6/codefly_cli/base/__init__.py
--rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.6/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/base/v0/__init__.py
--rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1676 2024-05-13 13:49:49.184868 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1855 2024-05-13 13:49:49.188891 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3371 2024-05-13 13:49:49.183146 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1615 2024-05-13 13:49:49.202244 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1791 2024-05-13 13:49:49.179812 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1950 2024-05-13 13:49:49.203856 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1704 2024-05-13 13:49:49.190337 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2613 2024-05-13 13:49:49.181480 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1701 2024-05-13 13:49:49.199660 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2168 2024-05-13 13:49:49.122019 codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2399 2024-05-16 14:53:37.499708 codefly_cli-0.0.6/codefly_cli/base/v0/agent_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499646 codefly_cli-0.0.6/codefly_cli/base/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     2500 2024-05-16 14:53:37.499461 codefly_cli-0.0.6/codefly_cli/base/v0/configuration_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499745 codefly_cli-0.0.6/codefly_cli/base/v0/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5828 2024-05-16 14:53:37.500444 codefly_cli-0.0.6/codefly_cli/base/v0/endpoint_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500443 codefly_cli-0.0.6/codefly_cli/base/v0/endpoint_pb2_grpc.py
--rw-r--r--   0        0        0     2169 2024-05-16 14:53:37.500330 codefly_cli-0.0.6/codefly_cli/base/v0/environment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500340 codefly_cli-0.0.6/codefly_cli/base/v0/environment_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2024-05-16 14:53:37.500972 codefly_cli-0.0.6/codefly_cli/base/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501854 codefly_cli-0.0.6/codefly_cli/base/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2768 2024-05-16 14:53:37.501436 codefly_cli-0.0.6/codefly_cli/base/v0/network_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501580 codefly_cli-0.0.6/codefly_cli/base/v0/network_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-16 14:53:37.501802 codefly_cli-0.0.6/codefly_cli/base/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501756 codefly_cli-0.0.6/codefly_cli/base/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-16 14:53:37.501624 codefly_cli-0.0.6/codefly_cli/base/v0/scope_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501786 codefly_cli-0.0.6/codefly_cli/base/v0/scope_pb2_grpc.py
--rw-r--r--   0        0        0     4669 2024-05-16 14:53:37.501891 codefly_cli-0.0.6/codefly_cli/base/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502450 codefly_cli-0.0.6/codefly_cli/base/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2414 2024-05-16 14:53:37.501961 codefly_cli-0.0.6/codefly_cli/base/v0/spec_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502506 codefly_cli-0.0.6/codefly_cli/base/v0/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3318 2024-05-16 14:53:37.502732 codefly_cli-0.0.6/codefly_cli/base/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503340 codefly_cli-0.0.6/codefly_cli/base/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/buf/__init__.py
--rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.6/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.6/codefly_cli/buf/validate/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/buf/validate/__init__.py
--rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.6/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1735 2024-05-13 13:49:49.171523 codefly_cli-0.0.6/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
--rw-r--r--   0        0        0   105220 2024-05-13 13:49:49.169873 codefly_cli-0.0.6/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.6/codefly_cli/buf/validate/expression.proto
--rw-r--r--   0        0        0     2292 2024-05-16 14:53:37.503962 codefly_cli-0.0.6/codefly_cli/buf/validate/expression_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503883 codefly_cli-0.0.6/codefly_cli/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/__init__.py
--rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1833 2024-05-13 13:49:49.173958 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/private.proto
--rw-r--r--   0        0        0     2332 2024-05-16 14:53:37.503853 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/private_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504685 codefly_cli-0.0.6/codefly_cli/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.6/codefly_cli/buf/validate/validate.proto
--rw-r--r--   0        0        0   144402 2024-05-16 14:53:37.506101 codefly_cli-0.0.6/codefly_cli/buf/validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504729 codefly_cli-0.0.6/codefly_cli/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/cli/__init__.py
--rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.6/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/cli/v0/__init__.py
--rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.6/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7578 2024-05-13 13:49:49.187411 codefly_cli-0.0.6/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    10048 2024-05-13 13:49:49.118488 codefly_cli-0.0.6/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0    11729 2024-05-16 14:53:37.505430 codefly_cli-0.0.6/codefly_cli/cli/v0/cli_pb2.py
--rw-r--r--   0        0        0    28562 2024-05-16 14:53:37.504644 codefly_cli-0.0.6/codefly_cli/cli/v0/cli_pb2_grpc.py
--rw-r--r--   0        0        0     4393 2024-05-18 18:05:46.058203 codefly_cli-0.0.6/codefly_cli/codefly.py
--rw-r--r--   0        0        0     1517 2024-05-13 13:49:49.218228 codefly_cli-0.0.6/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1912 2024-05-13 13:49:49.220245 codefly_cli-0.0.6/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1792 2024-05-16 14:53:37.504861 codefly_cli-0.0.6/codefly_cli/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504934 codefly_cli-0.0.6/codefly_cli/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2690 2024-05-16 14:53:37.504907 codefly_cli-0.0.6/codefly_cli/google/api/http_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505129 codefly_cli-0.0.6/codefly_cli/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/observability/__init__.py
--rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.6/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/observability/v0/__init__.py
--rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-05-13 13:49:49.211153 codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1550 2024-05-13 13:49:49.209688 codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2265 2024-05-13 13:49:49.213031 codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2214 2024-05-13 13:49:49.214782 codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2474 2024-05-16 14:53:37.505558 codefly_cli-0.0.6/codefly_cli/observability/v0/dependencies_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506072 codefly_cli-0.0.6/codefly_cli/observability/v0/dependencies_pb2_grpc.py
--rw-r--r--   0        0        0     1837 2024-05-16 14:53:37.505766 codefly_cli-0.0.6/codefly_cli/observability/v0/inventory_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505954 codefly_cli-0.0.6/codefly_cli/observability/v0/inventory_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2024-05-16 14:53:37.506417 codefly_cli-0.0.6/codefly_cli/observability/v0/logs_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506415 codefly_cli-0.0.6/codefly_cli/observability/v0/logs_pb2_grpc.py
--rw-r--r--   0        0        0     2098 2024-05-16 14:53:37.506262 codefly_cli-0.0.6/codefly_cli/observability/v0/metrics_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506455 codefly_cli-0.0.6/codefly_cli/observability/v0/metrics_pb2_grpc.py
--rw-r--r--   0        0        0     2985 2024-05-16 14:53:37.506432 codefly_cli-0.0.6/codefly_cli/observability/v0/sessions_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506726 codefly_cli-0.0.6/codefly_cli/observability/v0/sessions_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/__init__.py
--rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.6/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/agent/__init__.py
--rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.6/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/agent/v0/__init__.py
--rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.6/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3328 2024-05-13 13:49:49.194622 codefly_cli-0.0.6/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4050 2024-05-13 13:49:49.205929 codefly_cli-0.0.6/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     5107 2024-05-16 14:53:37.507542 codefly_cli-0.0.6/codefly_cli/services/agent/v0/agent_pb2.py
--rw-r--r--   0        0        0     2895 2024-05-16 14:53:37.507520 codefly_cli-0.0.6/codefly_cli/services/agent/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     6560 2024-05-16 14:53:37.507558 codefly_cli-0.0.6/codefly_cli/services/agent/v0/communicate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507148 codefly_cli-0.0.6/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
--rw-r--r--   0        0        0     2426 2024-05-16 14:53:37.507482 codefly_cli-0.0.6/codefly_cli/services/agent/v0/cyclonedx_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507429 codefly_cli-0.0.6/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/builder/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/builder/v0/__init__.py
--rw-r--r--   0        0        0    11603 2024-05-16 14:53:37.507453 codefly_cli-0.0.6/codefly_cli/services/builder/v0/builder_pb2.py
--rw-r--r--   0        0        0    15720 2024-05-16 14:53:37.508035 codefly_cli-0.0.6/codefly_cli/services/builder/v0/builder_pb2_grpc.py
--rw-r--r--   0        0        0     3239 2024-05-16 14:53:37.508589 codefly_cli-0.0.6/codefly_cli/services/builder/v0/deployment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508879 codefly_cli-0.0.6/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     1959 2024-05-16 14:53:37.508593 codefly_cli-0.0.6/codefly_cli/services/builder/v0/docker_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508837 codefly_cli-0.0.6/codefly_cli/services/builder/v0/docker_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/runtime/__init__.py
--rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.6/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.6/codefly_cli/services/runtime/v0/__init__.py
--rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.6/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7530 2024-05-13 13:49:49.198194 codefly_cli-0.0.6/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    11252 2024-05-16 14:53:37.509254 codefly_cli-0.0.6/codefly_cli/services/runtime/v0/runtime_pb2.py
--rw-r--r--   0        0        0    15818 2024-05-16 14:53:37.509221 codefly_cli-0.0.6/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
--rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.6/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
--rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.6/codefly_cli/tests/test_cli.py
--rw-r--r--   0        0        0      481 2024-05-18 18:06:11.560639 codefly_cli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.7/codefly_cli/actions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/actions/v0/__init__.py
+-rw-r--r--   0        0        0     2004 2024-05-16 14:53:37.499836 codefly_cli-0.0.7/codefly_cli/actions/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499681 codefly_cli-0.0.7/codefly_cli/actions/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2009 2024-05-16 14:53:37.499220 codefly_cli-0.0.7/codefly_cli/actions/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499510 codefly_cli-0.0.7/codefly_cli/actions/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     3743 2024-05-16 14:53:37.499953 codefly_cli-0.0.7/codefly_cli/actions/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499899 codefly_cli-0.0.7/codefly_cli/actions/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2588 2024-05-16 14:53:37.499937 codefly_cli-0.0.7/codefly_cli/actions/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499877 codefly_cli-0.0.7/codefly_cli/actions/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.7/codefly_cli/base/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.7/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/base/v0/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1676 2024-05-18 18:07:17.078576 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1855 2024-05-18 18:07:17.085209 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     3371 2024-05-18 18:07:17.076349 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1615 2024-05-18 18:07:17.101736 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1791 2024-05-18 18:07:17.072066 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2024-05-18 18:07:17.103610 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1704 2024-05-18 18:07:17.087333 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2613 2024-05-18 18:07:17.074126 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1701 2024-05-18 18:07:17.098860 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2168 2024-05-18 18:07:16.996487 codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2399 2024-05-16 14:53:37.499708 codefly_cli-0.0.7/codefly_cli/base/v0/agent_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499646 codefly_cli-0.0.7/codefly_cli/base/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     2500 2024-05-16 14:53:37.499461 codefly_cli-0.0.7/codefly_cli/base/v0/configuration_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499745 codefly_cli-0.0.7/codefly_cli/base/v0/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-05-16 14:53:37.500444 codefly_cli-0.0.7/codefly_cli/base/v0/endpoint_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500443 codefly_cli-0.0.7/codefly_cli/base/v0/endpoint_pb2_grpc.py
+-rw-r--r--   0        0        0     2169 2024-05-16 14:53:37.500330 codefly_cli-0.0.7/codefly_cli/base/v0/environment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500340 codefly_cli-0.0.7/codefly_cli/base/v0/environment_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2024-05-16 14:53:37.500972 codefly_cli-0.0.7/codefly_cli/base/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501854 codefly_cli-0.0.7/codefly_cli/base/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2768 2024-05-16 14:53:37.501436 codefly_cli-0.0.7/codefly_cli/base/v0/network_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501580 codefly_cli-0.0.7/codefly_cli/base/v0/network_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-16 14:53:37.501802 codefly_cli-0.0.7/codefly_cli/base/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501756 codefly_cli-0.0.7/codefly_cli/base/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-16 14:53:37.501624 codefly_cli-0.0.7/codefly_cli/base/v0/scope_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501786 codefly_cli-0.0.7/codefly_cli/base/v0/scope_pb2_grpc.py
+-rw-r--r--   0        0        0     4669 2024-05-16 14:53:37.501891 codefly_cli-0.0.7/codefly_cli/base/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502450 codefly_cli-0.0.7/codefly_cli/base/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2414 2024-05-16 14:53:37.501961 codefly_cli-0.0.7/codefly_cli/base/v0/spec_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502506 codefly_cli-0.0.7/codefly_cli/base/v0/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     3318 2024-05-16 14:53:37.502732 codefly_cli-0.0.7/codefly_cli/base/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503340 codefly_cli-0.0.7/codefly_cli/base/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/buf/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.7/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.7/codefly_cli/buf/validate/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/buf/validate/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.7/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1735 2024-05-18 18:07:17.059629 codefly_cli-0.0.7/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0   105220 2024-05-18 18:07:17.056893 codefly_cli-0.0.7/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.7/codefly_cli/buf/validate/expression.proto
+-rw-r--r--   0        0        0     2292 2024-05-16 14:53:37.503962 codefly_cli-0.0.7/codefly_cli/buf/validate/expression_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503883 codefly_cli-0.0.7/codefly_cli/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1833 2024-05-18 18:07:17.063238 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/private.proto
+-rw-r--r--   0        0        0     2332 2024-05-16 14:53:37.503853 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/private_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504685 codefly_cli-0.0.7/codefly_cli/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.7/codefly_cli/buf/validate/validate.proto
+-rw-r--r--   0        0        0   144402 2024-05-16 14:53:37.506101 codefly_cli-0.0.7/codefly_cli/buf/validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504729 codefly_cli-0.0.7/codefly_cli/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/cli/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.7/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/cli/v0/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.7/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7582 2024-05-18 18:07:17.081796 codefly_cli-0.0.7/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    10048 2024-05-18 18:07:16.992597 codefly_cli-0.0.7/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0    11729 2024-05-16 14:53:37.505430 codefly_cli-0.0.7/codefly_cli/cli/v0/cli_pb2.py
+-rw-r--r--   0        0        0    28562 2024-05-16 14:53:37.504644 codefly_cli-0.0.7/codefly_cli/cli/v0/cli_pb2_grpc.py
+-rw-r--r--   0        0        0     4393 2024-05-18 18:05:46.058203 codefly_cli-0.0.7/codefly_cli/codefly.py
+-rw-r--r--   0        0        0     1517 2024-05-18 18:07:17.118704 codefly_cli-0.0.7/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1912 2024-05-18 18:07:17.120443 codefly_cli-0.0.7/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1792 2024-05-16 14:53:37.504861 codefly_cli-0.0.7/codefly_cli/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504934 codefly_cli-0.0.7/codefly_cli/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2690 2024-05-16 14:53:37.504907 codefly_cli-0.0.7/codefly_cli/google/api/http_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505129 codefly_cli-0.0.7/codefly_cli/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/observability/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.7/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/observability/v0/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-05-18 18:07:17.111714 codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1550 2024-05-18 18:07:17.109926 codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2265 2024-05-18 18:07:17.113715 codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2214 2024-05-18 18:07:17.115529 codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2474 2024-05-16 14:53:37.505558 codefly_cli-0.0.7/codefly_cli/observability/v0/dependencies_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506072 codefly_cli-0.0.7/codefly_cli/observability/v0/dependencies_pb2_grpc.py
+-rw-r--r--   0        0        0     1837 2024-05-16 14:53:37.505766 codefly_cli-0.0.7/codefly_cli/observability/v0/inventory_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505954 codefly_cli-0.0.7/codefly_cli/observability/v0/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2024-05-16 14:53:37.506417 codefly_cli-0.0.7/codefly_cli/observability/v0/logs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506415 codefly_cli-0.0.7/codefly_cli/observability/v0/logs_pb2_grpc.py
+-rw-r--r--   0        0        0     2098 2024-05-16 14:53:37.506262 codefly_cli-0.0.7/codefly_cli/observability/v0/metrics_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506455 codefly_cli-0.0.7/codefly_cli/observability/v0/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0     2985 2024-05-16 14:53:37.506432 codefly_cli-0.0.7/codefly_cli/observability/v0/sessions_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506726 codefly_cli-0.0.7/codefly_cli/observability/v0/sessions_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.7/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/agent/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.7/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/agent/v0/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.7/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3328 2024-05-18 18:07:17.092257 codefly_cli-0.0.7/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4050 2024-05-18 18:07:17.105805 codefly_cli-0.0.7/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     5107 2024-05-16 14:53:37.507542 codefly_cli-0.0.7/codefly_cli/services/agent/v0/agent_pb2.py
+-rw-r--r--   0        0        0     2895 2024-05-16 14:53:37.507520 codefly_cli-0.0.7/codefly_cli/services/agent/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     6560 2024-05-16 14:53:37.507558 codefly_cli-0.0.7/codefly_cli/services/agent/v0/communicate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507148 codefly_cli-0.0.7/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
+-rw-r--r--   0        0        0     2426 2024-05-16 14:53:37.507482 codefly_cli-0.0.7/codefly_cli/services/agent/v0/cyclonedx_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507429 codefly_cli-0.0.7/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/builder/v0/__init__.py
+-rw-r--r--   0        0        0    11603 2024-05-16 14:53:37.507453 codefly_cli-0.0.7/codefly_cli/services/builder/v0/builder_pb2.py
+-rw-r--r--   0        0        0    15720 2024-05-16 14:53:37.508035 codefly_cli-0.0.7/codefly_cli/services/builder/v0/builder_pb2_grpc.py
+-rw-r--r--   0        0        0     3239 2024-05-16 14:53:37.508589 codefly_cli-0.0.7/codefly_cli/services/builder/v0/deployment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508879 codefly_cli-0.0.7/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-05-16 14:53:37.508593 codefly_cli-0.0.7/codefly_cli/services/builder/v0/docker_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508837 codefly_cli-0.0.7/codefly_cli/services/builder/v0/docker_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/runtime/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.7/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.7/codefly_cli/services/runtime/v0/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.7/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7464 2024-05-18 18:07:17.096644 codefly_cli-0.0.7/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    11252 2024-05-16 14:53:37.509254 codefly_cli-0.0.7/codefly_cli/services/runtime/v0/runtime_pb2.py
+-rw-r--r--   0        0        0    15818 2024-05-16 14:53:37.509221 codefly_cli-0.0.7/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
+-rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.7/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.7/codefly_cli/tests/test_cli.py
+-rw-r--r--   0        0        0      481 2024-05-18 18:24:50.230894 codefly_cli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 codefly_cli-0.0.7/PKG-INFO
```

### Comparing `codefly_cli-0.0.6/codefly_cli/actions/v0/module_pb2.py` & `codefly_cli-0.0.7/codefly_cli/actions/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/actions/v0/organization_pb2.py` & `codefly_cli-0.0.7/codefly_cli/actions/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/actions/v0/service_pb2.py` & `codefly_cli-0.0.7/codefly_cli/actions/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/actions/v0/workspace_pb2.py` & `codefly_cli-0.0.7/codefly_cli/actions/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2399 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 5f09 0000  o.......Y.Bf_...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 5f09 0000  o.........Ff_...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6505 a00b a100 a010 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2500 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 c409 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 c409 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6505 a00b a100 a010 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 5828 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 c416 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 c416 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0002 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6505 a00b a100 a010 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2169 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 7908 0000  o.......Y.Bfy...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 7908 0000  o.........Ffy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6505 a00b a100 a010 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2402 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 6209 0000  o.......Y.Bfb...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 6209 0000  o.........Ffb...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ec00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c10 6d11 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 d00a 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 d00a 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c0d 6d10 5a11  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2390 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 5609 0000  o.......Y.BfV...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 5609 0000  o.........FfV...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6505 a00b a100 a010 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 4669 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 3d12 0000  o.......Y.Bf=...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 3d12 0000  o.........Ff=...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0002 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c10 6d11 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2414 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 6e09 0000  o.......Y.Bfn...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 6e09 0000  o.........Ffn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c01  ..e.....Z.d.d.l.
 00000070: 6d0d 5a0e 0100 6505 a00b a100 a00f 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 3318 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 f60c 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 f60c 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c10 6d11 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/agent_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/configuration_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/endpoint_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/environment_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/module_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/network_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/network_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/organization_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/scope_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/service_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/spec_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/base/v0/workspace_pb2.py` & `codefly_cli-0.0.7/codefly_cli/base/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/BUILD.bazel` & `codefly_cli-0.0.7/codefly_cli/buf/validate/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 f408 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 f408 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6505 a00b a100  ..e.....Z.e.....
 00000070: a00d 6406 a101 5a0e 650f 8300 5a10 650a  ..d...Z.e...Z.e.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 144402 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 1234 0200  o.......Y.Bf.4..
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 1234 0200  o.........Ff.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2217 0000 6400  .....@...s"...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c10 6d11 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/expression.proto` & `codefly_cli-0.0.7/codefly_cli/buf/validate/expression.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/expression_pb2.py` & `codefly_cli-0.0.7/codefly_cli/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/priv/BUILD.bazel` & `codefly_cli-0.0.7/codefly_cli/buf/validate/priv/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2332 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 1c09 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 1c09 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c01  ..e.....Z.d.d.l.
 00000070: 6d0d 5a0e 0100 6505 a00b a100 a00f 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/priv/private.proto` & `codefly_cli-0.0.7/codefly_cli/buf/validate/priv/private.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/priv/private_pb2.py` & `codefly_cli-0.0.7/codefly_cli/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/validate.proto` & `codefly_cli-0.0.7/codefly_cli/buf/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/buf/validate/validate_pb2.py` & `codefly_cli-0.0.7/codefly_cli/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 11732 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 d42d 0000  o.......Y.Bf.-..
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 d12d 0000  o.........Ff.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 1e04 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c0d 6d10 5a11  m.Z...d.d.l.m.Z.
@@ -80,15 +80,15 @@
 000004f0: 6e74 5f70 6232 2901 da0b 7275 6e74 696d  nt_pb2)...runtim
 00000500: 655f 7062 3229 01da 0d69 6e76 656e 746f  e_pb2)...invento
 00000510: 7279 5f70 6232 2901 da10 6465 7065 6e64  ry_pb2)...depend
 00000520: 656e 6369 6573 5f70 6232 2901 da08 6c6f  encies_pb2)...lo
 00000530: 6773 5f70 6232 2901 da09 656d 7074 795f  gs_pb2)...empty_
 00000540: 7062 3229 01da 0f61 6e6e 6f74 6174 696f  pb2)...annotatio
 00000550: 6e73 5f70 6232 2901 da0d 7469 6d65 7374  ns_pb2)...timest
-00000560: 616d 705f 7062 3273 1b0d 0000 0a10 636c  amp_pb2s......cl
+00000560: 616d 705f 7062 3273 1d0d 0000 0a10 636c  amp_pb2s......cl
 00000570: 692f 7630 2f63 6c69 2e70 726f 746f 1210  i/v0/cli.proto..
 00000580: 6f62 7365 7276 6162 696c 6974 792e 7630  observability.v0
 00000590: 1a16 6261 7365 2f76 302f 656e 6470 6f69  ..base/v0/endpoi
 000005a0: 6e74 2e70 726f 746f 1a17 6261 7365 2f76  nt.proto..base/v
 000005b0: 302f 776f 726b 7370 6163 652e 7072 6f74  0/workspace.prot
 000005c0: 6f1a 1b62 6173 652f 7630 2f63 6f6e 6669  o..base/v0/confi
 000005d0: 6775 7261 7469 6f6e 2e70 726f 746f 1a1d  guration.proto..
@@ -157,15 +157,15 @@
 000009c0: 7322 220a 0a46 6c6f 7753 7461 7475 7312  s""..FlowStatus.
 000009d0: 140a 0572 6561 6479 1801 2001 2808 5205  ...ready.. .(.R.
 000009e0: 7265 6164 7922 110a 0f53 746f 7046 6c6f  ready"...StopFlo
 000009f0: 7752 6571 7565 7374 2212 0a10 5374 6f70  wRequest"...Stop
 00000a00: 466c 6f77 5265 7370 6f6e 7365 2214 0a12  FlowResponse"...
 00000a10: 4465 7374 726f 7946 6c6f 7752 6571 7565  DestroyFlowReque
 00000a20: 7374 2215 0a13 4465 7374 726f 7946 6c6f  st"...DestroyFlo
-00000a30: 7752 6573 706f 6e73 6532 8e0f 0a03 434c  wResponse2....CL
+00000a30: 7752 6573 706f 6e73 6532 900f 0a03 434c  wResponse2....CL
 00000a40: 4912 450a 0450 696e 6712 162e 676f 6f67  I.E..Ping...goog
 00000a50: 6c65 2e70 726f 746f 6275 662e 456d 7074  le.protobuf.Empt
 00000a60: 791a 162e 676f 6f67 6c65 2e70 726f 746f  y...google.proto
 00000a70: 6275 662e 456d 7074 7922 0d82 d3e4 9302  buf.Empty"......
 00000a80: 0712 052f 7069 6e67 128c 010a 1347 6574  .../ping.....Get
 00000a90: 4167 656e 7449 6e66 6f72 6d61 7469 6f6e  AgentInformation
 00000aa0: 122c 2e6f 6273 6572 7661 6269 6c69 7479  .,.observability
@@ -186,289 +186,289 @@
 00000b90: 6365 4465 7065 6e64 656e 6379 4772 6170  ceDependencyGrap
 00000ba0: 6812 162e 676f 6f67 6c65 2e70 726f 746f  h...google.proto
 00000bb0: 6275 662e 456d 7074 791a 1f2e 6f62 7365  buf.Empty...obse
 00000bc0: 7276 6162 696c 6974 792e 7630 2e47 7261  rvability.v0.Gra
 00000bd0: 7068 5265 7370 6f6e 7365 222b 82d3 e493  phResponse"+....
 00000be0: 0225 1223 2f77 6f72 6b73 7061 6365 2f73  .%.#/workspace/s
 00000bf0: 6572 7669 6365 2d64 6570 656e 6465 6e63  ervice-dependenc
-00000c00: 792d 6772 6170 6812 9101 0a28 4765 7457  y-graph....(GetW
+00000c00: 792d 6772 6170 6812 9301 0a28 4765 7457  y-graph....(GetW
 00000c10: 6f72 6b73 7061 6365 5075 626c 6963 4d6f  orkspacePublicMo
 00000c20: 6475 6c65 7344 6570 656e 6465 6e63 7947  dulesDependencyG
 00000c30: 7261 7068 1216 2e67 6f6f 676c 652e 7072  raph...google.pr
 00000c40: 6f74 6f62 7566 2e45 6d70 7479 1a24 2e6f  otobuf.Empty.$.o
 00000c50: 6273 6572 7661 6269 6c69 7479 2e76 302e  bservability.v0.
 00000c60: 4d75 6c74 6947 7261 7068 5265 7370 6f6e  MultiGraphRespon
-00000c70: 7365 2227 82d3 e493 0221 121f 2f77 6f72  se"'.....!../wor
-00000c80: 6b73 7061 6365 2f70 7562 6c69 632d 6d6f  kspace/public-mo
-00000c90: 6475 6c65 732d 6772 6170 6812 650a 0947  dules-graph.e..G
-00000ca0: 6574 4163 7469 7665 1216 2e67 6f6f 676c  etActive...googl
-00000cb0: 652e 7072 6f74 6f62 7566 2e45 6d70 7479  e.protobuf.Empty
-00000cc0: 1a20 2e6f 6273 6572 7661 6269 6c69 7479  . .observability
-00000cd0: 2e76 302e 4163 7469 7665 5265 7370 6f6e  .v0.ActiveRespon
-00000ce0: 7365 221e 82d3 e493 0218 1216 2f77 6f72  se"........./wor
-00000cf0: 6b73 7061 6365 2f69 6e66 6f72 6d61 7469  kspace/informati
-00000d00: 6f6e 129b 010a 0c47 6574 4164 6472 6573  on.....GetAddres
-00000d10: 7365 7312 232e 6f62 7365 7276 6162 696c  ses.#.observabil
-00000d20: 6974 792e 7630 2e47 6574 4164 6472 6573  ity.v0.GetAddres
-00000d30: 7352 6571 7565 7374 1a24 2e6f 6273 6572  sRequest.$.obser
-00000d40: 7661 6269 6c69 7479 2e76 302e 4765 7441  vability.v0.GetA
-00000d50: 6464 7265 7373 5265 7370 6f6e 7365 2240  ddressResponse"@
-00000d60: 82d3 e493 023a 1238 2f77 6f72 6b73 7061  .....:.8/workspa
-00000d70: 6365 2f6e 6574 776f 726b 2d6d 6170 7069  ce/network-mappi
-00000d80: 6e67 2f7b 6d6f 6475 6c65 7d2f 7b73 6572  ng/{module}/{ser
-00000d90: 7669 6365 7d2f 7b65 6e64 706f 696e 747d  vice}/{endpoint}
-00000da0: 129e 010a 1047 6574 436f 6e66 6967 7572  .....GetConfigur
-00000db0: 6174 696f 6e12 292e 6f62 7365 7276 6162  ation.).observab
-00000dc0: 696c 6974 792e 7630 2e47 6574 436f 6e66  ility.v0.GetConf
-00000dd0: 6967 7572 6174 696f 6e52 6571 7565 7374  igurationRequest
-00000de0: 1a2a 2e6f 6273 6572 7661 6269 6c69 7479  .*.observability
-00000df0: 2e76 302e 4765 7443 6f6e 6669 6775 7261  .v0.GetConfigura
-00000e00: 7469 6f6e 5265 7370 6f6e 7365 2233 82d3  tionResponse"3..
-00000e10: e493 022d 122b 2f77 6f72 6b73 7061 6365  ...-.+/workspace
-00000e20: 2f63 6f6e 6669 6775 7261 7469 6f6e 2f7b  /configuration/{
-00000e30: 6d6f 6475 6c65 7d2f 7b73 6572 7669 6365  module}/{service
-00000e40: 7d12 ba01 0a1d 4765 7444 6570 656e 6465  }.....GetDepende
-00000e50: 6e63 6965 7343 6f6e 6669 6775 7261 7469  nciesConfigurati
-00000e60: 6f6e 7312 292e 6f62 7365 7276 6162 696c  ons.).observabil
-00000e70: 6974 792e 7630 2e47 6574 436f 6e66 6967  ity.v0.GetConfig
-00000e80: 7572 6174 696f 6e52 6571 7565 7374 1a2b  urationRequest.+
-00000e90: 2e6f 6273 6572 7661 6269 6c69 7479 2e76  .observability.v
-00000ea0: 302e 4765 7443 6f6e 6669 6775 7261 7469  0.GetConfigurati
-00000eb0: 6f6e 7352 6573 706f 6e73 6522 4182 d3e4  onsResponse"A...
-00000ec0: 9302 3b12 392f 776f 726b 7370 6163 652f  ..;.9/workspace/
-00000ed0: 6465 7065 6e64 656e 6369 6573 2d63 6f6e  dependencies-con
-00000ee0: 6669 6775 7261 7469 6f6e 732f 7b6d 6f64  figurations/{mod
-00000ef0: 756c 657d 2f7b 7365 7276 6963 657d 12b0  ule}/{service}..
-00000f00: 010a 1847 6574 5275 6e74 696d 6543 6f6e  ...GetRuntimeCon
-00000f10: 6669 6775 7261 7469 6f6e 7312 292e 6f62  figurations.).ob
-00000f20: 7365 7276 6162 696c 6974 792e 7630 2e47  servability.v0.G
-00000f30: 6574 436f 6e66 6967 7572 6174 696f 6e52  etConfigurationR
-00000f40: 6571 7565 7374 1a2b 2e6f 6273 6572 7661  equest.+.observa
-00000f50: 6269 6c69 7479 2e76 302e 4765 7443 6f6e  bility.v0.GetCon
-00000f60: 6669 6775 7261 7469 6f6e 7352 6573 706f  figurationsRespo
-00000f70: 6e73 6522 3c82 d3e4 9302 3612 342f 776f  nse"<.....6.4/wo
-00000f80: 726b 7370 6163 652f 7275 6e74 696d 652d  rkspace/runtime-
-00000f90: 636f 6e66 6967 7572 6174 696f 6e73 2f7b  configurations/{
-00000fa0: 6d6f 6475 6c65 7d2f 7b73 6572 7669 6365  module}/{service
-00000fb0: 7d12 500a 044c 6f67 7312 162e 676f 6f67  }.P..Logs...goog
-00000fc0: 6c65 2e70 726f 746f 6275 662e 456d 7074  le.protobuf.Empt
-00000fd0: 791a 152e 6f62 7365 7276 6162 696c 6974  y...observabilit
-00000fe0: 792e 7630 2e4c 6f67 2217 82d3 e493 0211  y.v0.Log".......
-00000ff0: 120f 2f77 6f72 6b73 7061 6365 2f6c 6f67  ../workspace/log
-00001000: 7330 0112 700a 1041 6374 6976 654c 6f67  s0..p..ActiveLog
-00001010: 4869 7374 6f72 7912 1c2e 6f62 7365 7276  History...observ
-00001020: 6162 696c 6974 792e 7630 2e4c 6f67 5265  ability.v0.LogRe
-00001030: 7175 6573 741a 1d2e 6f62 7365 7276 6162  quest...observab
-00001040: 696c 6974 792e 7630 2e4c 6f67 5265 7370  ility.v0.LogResp
-00001050: 6f6e 7365 221f 82d3 e493 0219 1217 2f77  onse"........./w
-00001060: 6f72 6b73 7061 6365 2f6c 6f67 732f 6869  orkspace/logs/hi
-00001070: 7374 6f72 7912 650a 0d47 6574 466c 6f77  story.e..GetFlow
-00001080: 5374 6174 7573 1216 2e67 6f6f 676c 652e  Status...google.
-00001090: 7072 6f74 6f62 7566 2e45 6d70 7479 1a1c  protobuf.Empty..
-000010a0: 2e6f 6273 6572 7661 6269 6c69 7479 2e76  .observability.v
-000010b0: 302e 466c 6f77 5374 6174 7573 221e 82d3  0.FlowStatus"...
-000010c0: e493 0218 1216 2f77 6f72 6b73 7061 6365  ....../workspace
-000010d0: 2f66 6c6f 772f 7374 6174 7573 126f 0a08  /flow/status.o..
-000010e0: 5374 6f70 466c 6f77 1221 2e6f 6273 6572  StopFlow.!.obser
-000010f0: 7661 6269 6c69 7479 2e76 302e 5374 6f70  vability.v0.Stop
-00001100: 466c 6f77 5265 7175 6573 741a 222e 6f62  FlowRequest.".ob
-00001110: 7365 7276 6162 696c 6974 792e 7630 2e53  servability.v0.S
-00001120: 746f 7046 6c6f 7752 6573 706f 6e73 6522  topFlowResponse"
-00001130: 1c82 d3e4 9302 1622 142f 776f 726b 7370  ......."./worksp
-00001140: 6163 652f 666c 6f77 2f73 746f 7012 7b0a  ace/flow/stop.{.
-00001150: 0b44 6573 7472 6f79 466c 6f77 1224 2e6f  .DestroyFlow.$.o
-00001160: 6273 6572 7661 6269 6c69 7479 2e76 302e  bservability.v0.
-00001170: 4465 7374 726f 7946 6c6f 7752 6571 7565  DestroyFlowReque
-00001180: 7374 1a25 2e6f 6273 6572 7661 6269 6c69  st.%.observabili
-00001190: 7479 2e76 302e 4465 7374 726f 7946 6c6f  ty.v0.DestroyFlo
-000011a0: 7752 6573 706f 6e73 6522 1f82 d3e4 9302  wResponse"......
-000011b0: 1922 172f 776f 726b 7370 6163 652f 666c  ."./workspace/fl
-000011c0: 6f77 2f64 6573 7472 6f79 42b2 010a 1463  ow/destroyB....c
-000011d0: 6f6d 2e6f 6273 6572 7661 6269 6c69 7479  om.observability
-000011e0: 2e76 3042 0843 6c69 5072 6f74 6f50 015a  .v0B.CliProtoP.Z
-000011f0: 2f67 6974 6875 622e 636f 6d2f 636f 6465  /github.com/code
-00001200: 666c 792d 6465 762f 636f 7265 2f67 656e  fly-dev/core/gen
-00001210: 6572 6174 6564 2f67 6f2f 636c 692f 7630  erated/go/cli/v0
-00001220: a202 034f 5658 aa02 104f 6273 6572 7661  ...OVX...Observa
-00001230: 6269 6c69 7479 2e56 30ca 0210 4f62 7365  bility.V0...Obse
-00001240: 7276 6162 696c 6974 795c 5630 e202 1c4f  rvability\V0...O
-00001250: 6273 6572 7661 6269 6c69 7479 5c56 305c  bservability\V0\
-00001260: 4750 424d 6574 6164 6174 61ea 0211 4f62  GPBMetadata...Ob
-00001270: 7365 7276 6162 696c 6974 793a 3a56 3062  servability::V0b
-00001280: 0670 726f 746f 337a 0e63 6c69 2e76 302e  .proto3z.cli.v0.
-00001290: 636c 695f 7062 324e da0a 4445 5343 5249  cli_pb2N..DESCRI
-000012a0: 5054 4f52 73b2 0000 000a 1463 6f6d 2e6f  PTORs......com.o
-000012b0: 6273 6572 7661 6269 6c69 7479 2e76 3042  bservability.v0B
-000012c0: 0843 6c69 5072 6f74 6f50 015a 2f67 6974  .CliProtoP.Z/git
-000012d0: 6875 622e 636f 6d2f 636f 6465 666c 792d  hub.com/codefly-
-000012e0: 6465 762f 636f 7265 2f67 656e 6572 6174  dev/core/generat
-000012f0: 6564 2f67 6f2f 636c 692f 7630 a202 034f  ed/go/cli/v0...O
-00001300: 5658 aa02 104f 6273 6572 7661 6269 6c69  VX...Observabili
-00001310: 7479 2e56 30ca 0210 4f62 7365 7276 6162  ty.V0...Observab
-00001320: 696c 6974 795c 5630 e202 1c4f 6273 6572  ility\V0...Obser
-00001330: 7661 6269 6c69 7479 5c56 305c 4750 424d  vability\V0\GPBM
-00001340: 6574 6164 6174 61ea 0211 4f62 7365 7276  etadata...Observ
-00001350: 6162 696c 6974 793a 3a56 305a 045f 434c  ability::V0Z._CL
-00001360: 49da 0450 696e 6773 0d00 0000 82d3 e493  I..Pings........
-00001370: 0207 1205 2f70 696e 67da 1347 6574 4167  ..../ping..GetAg
-00001380: 656e 7449 6e66 6f72 6d61 7469 6f6e 7322  entInformations"
-00001390: 0000 0082 d3e4 9302 1c12 1a2f 6167 656e  .........../agen
-000013a0: 742f 7b61 6765 6e74 7d2f 696e 666f 726d  t/{agent}/inform
-000013b0: 6174 696f 6eda 1547 6574 576f 726b 7370  ation..GetWorksp
-000013c0: 6163 6549 6e76 656e 746f 7279 731c 0000  aceInventorys...
-000013d0: 0082 d3e4 9302 1612 142f 776f 726b 7370  ........./worksp
-000013e0: 6163 652f 696e 7665 6e74 6f72 79da 2247  ace/inventory."G
-000013f0: 6574 576f 726b 7370 6163 6553 6572 7669  etWorkspaceServi
-00001400: 6365 4465 7065 6e64 656e 6379 4772 6170  ceDependencyGrap
-00001410: 6873 2b00 0000 82d3 e493 0225 1223 2f77  hs+........%.#/w
-00001420: 6f72 6b73 7061 6365 2f73 6572 7669 6365  orkspace/service
-00001430: 2d64 6570 656e 6465 6e63 792d 6772 6170  -dependency-grap
-00001440: 68da 2847 6574 576f 726b 7370 6163 6550  h.(GetWorkspaceP
-00001450: 7562 6c69 634d 6f64 756c 6573 4465 7065  ublicModulesDepe
-00001460: 6e64 656e 6379 4772 6170 6873 2700 0000  ndencyGraphs'...
-00001470: 82d3 e493 0221 121f 2f77 6f72 6b73 7061  .....!../workspa
-00001480: 6365 2f70 7562 6c69 632d 6d6f 6475 6c65  ce/public-module
-00001490: 732d 6772 6170 68da 0947 6574 4163 7469  s-graph..GetActi
-000014a0: 7665 731e 0000 0082 d3e4 9302 1812 162f  ves............/
-000014b0: 776f 726b 7370 6163 652f 696e 666f 726d  workspace/inform
-000014c0: 6174 696f 6eda 0c47 6574 4164 6472 6573  ation..GetAddres
-000014d0: 7365 7373 4000 0000 82d3 e493 023a 1238  sess@........:.8
-000014e0: 2f77 6f72 6b73 7061 6365 2f6e 6574 776f  /workspace/netwo
-000014f0: 726b 2d6d 6170 7069 6e67 2f7b 6d6f 6475  rk-mapping/{modu
-00001500: 6c65 7d2f 7b73 6572 7669 6365 7d2f 7b65  le}/{service}/{e
-00001510: 6e64 706f 696e 747d da10 4765 7443 6f6e  ndpoint}..GetCon
-00001520: 6669 6775 7261 7469 6f6e 7333 0000 0082  figurations3....
-00001530: d3e4 9302 2d12 2b2f 776f 726b 7370 6163  ....-.+/workspac
-00001540: 652f 636f 6e66 6967 7572 6174 696f 6e2f  e/configuration/
-00001550: 7b6d 6f64 756c 657d 2f7b 7365 7276 6963  {module}/{servic
-00001560: 657d da1d 4765 7444 6570 656e 6465 6e63  e}..GetDependenc
-00001570: 6965 7343 6f6e 6669 6775 7261 7469 6f6e  iesConfiguration
-00001580: 7373 4100 0000 82d3 e493 023b 1239 2f77  ssA........;.9/w
-00001590: 6f72 6b73 7061 6365 2f64 6570 656e 6465  orkspace/depende
-000015a0: 6e63 6965 732d 636f 6e66 6967 7572 6174  ncies-configurat
-000015b0: 696f 6e73 2f7b 6d6f 6475 6c65 7d2f 7b73  ions/{module}/{s
-000015c0: 6572 7669 6365 7dda 1847 6574 5275 6e74  ervice}..GetRunt
-000015d0: 696d 6543 6f6e 6669 6775 7261 7469 6f6e  imeConfiguration
-000015e0: 7373 3c00 0000 82d3 e493 0236 1234 2f77  ss<........6.4/w
-000015f0: 6f72 6b73 7061 6365 2f72 756e 7469 6d65  orkspace/runtime
-00001600: 2d63 6f6e 6669 6775 7261 7469 6f6e 732f  -configurations/
-00001610: 7b6d 6f64 756c 657d 2f7b 7365 7276 6963  {module}/{servic
-00001620: 657d da04 4c6f 6773 7317 0000 0082 d3e4  e}..Logss.......
-00001630: 9302 1112 0f2f 776f 726b 7370 6163 652f  ...../workspace/
-00001640: 6c6f 6773 da10 4163 7469 7665 4c6f 6748  logs..ActiveLogH
-00001650: 6973 746f 7279 731f 0000 0082 d3e4 9302  istorys.........
-00001660: 1912 172f 776f 726b 7370 6163 652f 6c6f  .../workspace/lo
-00001670: 6773 2f68 6973 746f 7279 da0d 4765 7446  gs/history..GetF
-00001680: 6c6f 7753 7461 7475 7373 1e00 0000 82d3  lowStatuss......
-00001690: e493 0218 1216 2f77 6f72 6b73 7061 6365  ....../workspace
-000016a0: 2f66 6c6f 772f 7374 6174 7573 da08 5374  /flow/status..St
-000016b0: 6f70 466c 6f77 731c 0000 0082 d3e4 9302  opFlows.........
-000016c0: 1622 142f 776f 726b 7370 6163 652f 666c  ."./workspace/fl
-000016d0: 6f77 2f73 746f 70da 0b44 6573 7472 6f79  ow/stop..Destroy
-000016e0: 466c 6f77 731f 0000 0082 d3e4 9302 1922  Flows.........."
-000016f0: 172f 776f 726b 7370 6163 652f 666c 6f77  ./workspace/flow
-00001700: 2f64 6573 7472 6f79 6976 0100 005a 1b5f  /destroyiv...Z._
-00001710: 4745 5441 4745 4e54 494e 464f 524d 4154  GETAGENTINFORMAT
-00001720: 494f 4e52 4551 5545 5354 69a8 0100 0069  IONREQUESTi....i
-00001730: aa01 0000 5a13 5f4d 554c 5449 4752 4150  ....Z._MULTIGRAP
-00001740: 4852 4553 504f 4e53 4569 f701 0000 69f9  HRESPONSEi....i.
-00001750: 0100 005a 0f5f 4143 5449 5645 5245 5350  ...Z._ACTIVERESP
-00001760: 4f4e 5345 6959 0200 0069 5b02 0000 5a13  ONSEiY...i[...Z.
-00001770: 5f52 554e 4e49 4e47 494e 464f 524d 4154  _RUNNINGINFORMAT
-00001780: 494f 4e69 be02 0000 69c0 0200 005a 125f  IONi....i....Z._
-00001790: 4745 5441 4444 5245 5353 5245 5155 4553  GETADDRESSREQUES
-000017a0: 5469 2103 0000 6923 0300 005a 135f 4745  Ti!...i#...Z._GE
-000017b0: 5441 4444 5245 5353 5245 5350 4f4e 5345  TADDRESSRESPONSE
-000017c0: 6951 0300 0069 5303 0000 5a18 5f47 4554  iQ...iS...Z._GET
-000017d0: 434f 4e46 4947 5552 4154 494f 4e52 4551  CONFIGURATIONREQ
-000017e0: 5545 5354 699e 0300 0069 a003 0000 5a19  UESTi....i....Z.
-000017f0: 5f47 4554 434f 4e46 4947 5552 4154 494f  _GETCONFIGURATIO
-00001800: 4e52 4553 504f 4e53 4569 f803 0000 69fa  NRESPONSEi....i.
-00001810: 0300 005a 1a5f 4745 5443 4f4e 4649 4755  ...Z._GETCONFIGU
-00001820: 5241 5449 4f4e 5352 4553 504f 4e53 4569  RATIONSRESPONSEi
-00001830: 5504 0000 6957 0400 005a 0b5f 464c 4f57  U...iW...Z._FLOW
-00001840: 5354 4154 5553 6979 0400 0069 7b04 0000  STATUSiy...i{...
-00001850: 5a10 5f53 544f 5046 4c4f 5752 4551 5545  Z._STOPFLOWREQUE
-00001860: 5354 698c 0400 0069 8e04 0000 5a11 5f53  STi....i....Z._S
-00001870: 544f 5046 4c4f 5752 4553 504f 4e53 4569  TOPFLOWRESPONSEi
-00001880: a004 0000 69a2 0400 005a 135f 4445 5354  ....i....Z._DEST
-00001890: 524f 5946 4c4f 5752 4551 5545 5354 69b6  ROYFLOWREQUESTi.
-000018a0: 0400 0069 b804 0000 5a14 5f44 4553 5452  ...i....Z._DESTR
-000018b0: 4f59 464c 4f57 5245 5350 4f4e 5345 69cd  OYFLOWRESPONSEi.
-000018c0: 0400 0069 d004 0000 695e 0c00 0029 34da  ...i....i^...)4.
-000018d0: 075f 5f64 6f63 5f5f da0f 676f 6f67 6c65  .__doc__..google
-000018e0: 2e70 726f 746f 6275 6672 0200 0000 da0b  .protobufr......
-000018f0: 5f64 6573 6372 6970 746f 7272 0300 0000  _descriptorr....
-00001900: da10 5f64 6573 6372 6970 746f 725f 706f  .._descriptor_po
-00001910: 6f6c 7204 0000 00da 105f 7379 6d62 6f6c  olr......_symbol
-00001920: 5f64 6174 6162 6173 65da 1867 6f6f 676c  _database..googl
-00001930: 652e 7072 6f74 6f62 7566 2e69 6e74 6572  e.protobuf.inter
-00001940: 6e61 6c72 0500 0000 da08 5f62 7569 6c64  nalr......_build
-00001950: 6572 da07 4465 6661 756c 74da 075f 7379  er..Default.._sy
-00001960: 6d5f 6462 da07 6261 7365 2e76 3072 0600  m_db..base.v0r..
-00001970: 0000 da1d 6261 7365 5f64 6f74 5f76 305f  ....base_dot_v0_
-00001980: 646f 745f 656e 6470 6f69 6e74 5f5f 7062  dot_endpoint__pb
-00001990: 3272 0700 0000 da1e 6261 7365 5f64 6f74  2r......base_dot
-000019a0: 5f76 305f 646f 745f 776f 726b 7370 6163  _v0_dot_workspac
-000019b0: 655f 5f70 6232 7208 0000 005a 2262 6173  e__pb2r....Z"bas
-000019c0: 655f 646f 745f 7630 5f64 6f74 5f63 6f6e  e_dot_v0_dot_con
-000019d0: 6669 6775 7261 7469 6f6e 5f5f 7062 32da  figuration__pb2.
-000019e0: 1173 6572 7669 6365 732e 6167 656e 742e  .services.agent.
-000019f0: 7630 7209 0000 00da 2873 6572 7669 6365  v0r.....(service
-00001a00: 735f 646f 745f 6167 656e 745f 646f 745f  s_dot_agent_dot_
-00001a10: 7630 5f64 6f74 5f61 6765 6e74 5f5f 7062  v0_dot_agent__pb
-00001a20: 325a 1373 6572 7669 6365 732e 7275 6e74  2Z.services.runt
-00001a30: 696d 652e 7630 720a 0000 005a 2c73 6572  ime.v0r....Z,ser
-00001a40: 7669 6365 735f 646f 745f 7275 6e74 696d  vices_dot_runtim
-00001a50: 655f 646f 745f 7630 5f64 6f74 5f72 756e  e_dot_v0_dot_run
-00001a60: 7469 6d65 5f5f 7062 32da 106f 6273 6572  time__pb2..obser
-00001a70: 7661 6269 6c69 7479 2e76 3072 0b00 0000  vability.v0r....
-00001a80: 5a27 6f62 7365 7276 6162 696c 6974 795f  Z'observability_
-00001a90: 646f 745f 7630 5f64 6f74 5f69 6e76 656e  dot_v0_dot_inven
-00001aa0: 746f 7279 5f5f 7062 3272 0c00 0000 da2a  tory__pb2r.....*
-00001ab0: 6f62 7365 7276 6162 696c 6974 795f 646f  observability_do
-00001ac0: 745f 7630 5f64 6f74 5f64 6570 656e 6465  t_v0_dot_depende
-00001ad0: 6e63 6965 735f 5f70 6232 720d 0000 00da  ncies__pb2r.....
-00001ae0: 226f 6273 6572 7661 6269 6c69 7479 5f64  "observability_d
-00001af0: 6f74 5f76 305f 646f 745f 6c6f 6773 5f5f  ot_v0_dot_logs__
-00001b00: 7062 3272 0e00 0000 da22 676f 6f67 6c65  pb2r....."google
-00001b10: 5f64 6f74 5f70 726f 746f 6275 665f 646f  _dot_protobuf_do
-00001b20: 745f 656d 7074 795f 5f70 6232 5a0a 676f  t_empty__pb2Z.go
-00001b30: 6f67 6c65 2e61 7069 720f 0000 005a 2367  ogle.apir....Z#g
-00001b40: 6f6f 676c 655f 646f 745f 6170 695f 646f  oogle_dot_api_do
-00001b50: 745f 616e 6e6f 7461 7469 6f6e 735f 5f70  t_annotations__p
-00001b60: 6232 7210 0000 00da 2667 6f6f 676c 655f  b2r.....&google_
-00001b70: 646f 745f 7072 6f74 6f62 7566 5f64 6f74  dot_protobuf_dot
-00001b80: 5f74 696d 6573 7461 6d70 5f5f 7062 32da  _timestamp__pb2.
-00001b90: 1141 6464 5365 7269 616c 697a 6564 4669  .AddSerializedFi
-00001ba0: 6c65 7211 0000 00da 0767 6c6f 6261 6c73  ler......globals
-00001bb0: da08 5f67 6c6f 6261 6c73 da1e 4275 696c  .._globals..Buil
-00001bc0: 644d 6573 7361 6765 416e 6445 6e75 6d44  dMessageAndEnumD
-00001bd0: 6573 6372 6970 746f 7273 da1e 4275 696c  escriptors..Buil
-00001be0: 6454 6f70 4465 7363 7269 7074 6f72 7341  dTopDescriptorsA
-00001bf0: 6e64 4d65 7373 6167 6573 da12 5f55 5345  ndMessages.._USE
-00001c00: 5f43 5f44 4553 4352 4950 544f 5253 da0f  _C_DESCRIPTORS..
-00001c10: 5f6c 6f61 6465 645f 6f70 7469 6f6e 73da  _loaded_options.
-00001c20: 135f 7365 7269 616c 697a 6564 5f6f 7074  ._serialized_opt
-00001c30: 696f 6e73 da0f 6d65 7468 6f64 735f 6279  ions..methods_by
-00001c40: 5f6e 616d 65da 115f 7365 7269 616c 697a  _name.._serializ
-00001c50: 6564 5f73 7461 7274 da0f 5f73 6572 6961  ed_start.._seria
-00001c60: 6c69 7a65 645f 656e 64a9 0072 3f00 0000  lized_end..r?...
-00001c70: 723f 0000 00fa 662f 5573 6572 732f 616e  r?....f/Users/an
-00001c80: 746f 696e 652f 4465 7665 6c6f 706d 656e  toine/Developmen
-00001c90: 742f 636f 6465 666c 792e 6465 762f 636f  t/codefly.dev/co
-00001ca0: 7265 2f67 656e 6572 6174 6564 2f70 7974  re/generated/pyt
-00001cb0: 686f 6e2f 636f 6465 666c 792d 636c 692f  hon/codefly-cli/
-00001cc0: 636f 6465 666c 795f 636c 692f 636c 692f  codefly_cli/cli/
-00001cd0: 7630 2f63 6c69 5f70 6232 2e70 79da 083c  v0/cli_pb2.py..<
-00001ce0: 6d6f 6475 6c65 3e01 0000 0073 aa00 0000  module>....s....
-00001cf0: 0404 0c01 0c01 0c01 0c01 0803 0c03 0c01  ................
-00001d00: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00001d10: 0c01 0e03 0602 0c01 0e01 0801 0a01 0a01  ................
-00001d20: 1001 1001 1001 1001 1001 1001 1001 1001  ................
+00000c70: 7365 2229 82d3 e493 0223 1221 2f77 6f72  se").....#.!/wor
+00000c80: 6b73 7061 6365 2f70 7562 6c69 632d 656e  kspace/public-en
+00000c90: 6470 6f69 6e74 732d 6772 6170 6812 650a  dpoints-graph.e.
+00000ca0: 0947 6574 4163 7469 7665 1216 2e67 6f6f  .GetActive...goo
+00000cb0: 676c 652e 7072 6f74 6f62 7566 2e45 6d70  gle.protobuf.Emp
+00000cc0: 7479 1a20 2e6f 6273 6572 7661 6269 6c69  ty. .observabili
+00000cd0: 7479 2e76 302e 4163 7469 7665 5265 7370  ty.v0.ActiveResp
+00000ce0: 6f6e 7365 221e 82d3 e493 0218 1216 2f77  onse"........./w
+00000cf0: 6f72 6b73 7061 6365 2f69 6e66 6f72 6d61  orkspace/informa
+00000d00: 7469 6f6e 129b 010a 0c47 6574 4164 6472  tion.....GetAddr
+00000d10: 6573 7365 7312 232e 6f62 7365 7276 6162  esses.#.observab
+00000d20: 696c 6974 792e 7630 2e47 6574 4164 6472  ility.v0.GetAddr
+00000d30: 6573 7352 6571 7565 7374 1a24 2e6f 6273  essRequest.$.obs
+00000d40: 6572 7661 6269 6c69 7479 2e76 302e 4765  ervability.v0.Ge
+00000d50: 7441 6464 7265 7373 5265 7370 6f6e 7365  tAddressResponse
+00000d60: 2240 82d3 e493 023a 1238 2f77 6f72 6b73  "@.....:.8/works
+00000d70: 7061 6365 2f6e 6574 776f 726b 2d6d 6170  pace/network-map
+00000d80: 7069 6e67 2f7b 6d6f 6475 6c65 7d2f 7b73  ping/{module}/{s
+00000d90: 6572 7669 6365 7d2f 7b65 6e64 706f 696e  ervice}/{endpoin
+00000da0: 747d 129e 010a 1047 6574 436f 6e66 6967  t}.....GetConfig
+00000db0: 7572 6174 696f 6e12 292e 6f62 7365 7276  uration.).observ
+00000dc0: 6162 696c 6974 792e 7630 2e47 6574 436f  ability.v0.GetCo
+00000dd0: 6e66 6967 7572 6174 696f 6e52 6571 7565  nfigurationReque
+00000de0: 7374 1a2a 2e6f 6273 6572 7661 6269 6c69  st.*.observabili
+00000df0: 7479 2e76 302e 4765 7443 6f6e 6669 6775  ty.v0.GetConfigu
+00000e00: 7261 7469 6f6e 5265 7370 6f6e 7365 2233  rationResponse"3
+00000e10: 82d3 e493 022d 122b 2f77 6f72 6b73 7061  .....-.+/workspa
+00000e20: 6365 2f63 6f6e 6669 6775 7261 7469 6f6e  ce/configuration
+00000e30: 2f7b 6d6f 6475 6c65 7d2f 7b73 6572 7669  /{module}/{servi
+00000e40: 6365 7d12 ba01 0a1d 4765 7444 6570 656e  ce}.....GetDepen
+00000e50: 6465 6e63 6965 7343 6f6e 6669 6775 7261  denciesConfigura
+00000e60: 7469 6f6e 7312 292e 6f62 7365 7276 6162  tions.).observab
+00000e70: 696c 6974 792e 7630 2e47 6574 436f 6e66  ility.v0.GetConf
+00000e80: 6967 7572 6174 696f 6e52 6571 7565 7374  igurationRequest
+00000e90: 1a2b 2e6f 6273 6572 7661 6269 6c69 7479  .+.observability
+00000ea0: 2e76 302e 4765 7443 6f6e 6669 6775 7261  .v0.GetConfigura
+00000eb0: 7469 6f6e 7352 6573 706f 6e73 6522 4182  tionsResponse"A.
+00000ec0: d3e4 9302 3b12 392f 776f 726b 7370 6163  ....;.9/workspac
+00000ed0: 652f 6465 7065 6e64 656e 6369 6573 2d63  e/dependencies-c
+00000ee0: 6f6e 6669 6775 7261 7469 6f6e 732f 7b6d  onfigurations/{m
+00000ef0: 6f64 756c 657d 2f7b 7365 7276 6963 657d  odule}/{service}
+00000f00: 12b0 010a 1847 6574 5275 6e74 696d 6543  .....GetRuntimeC
+00000f10: 6f6e 6669 6775 7261 7469 6f6e 7312 292e  onfigurations.).
+00000f20: 6f62 7365 7276 6162 696c 6974 792e 7630  observability.v0
+00000f30: 2e47 6574 436f 6e66 6967 7572 6174 696f  .GetConfiguratio
+00000f40: 6e52 6571 7565 7374 1a2b 2e6f 6273 6572  nRequest.+.obser
+00000f50: 7661 6269 6c69 7479 2e76 302e 4765 7443  vability.v0.GetC
+00000f60: 6f6e 6669 6775 7261 7469 6f6e 7352 6573  onfigurationsRes
+00000f70: 706f 6e73 6522 3c82 d3e4 9302 3612 342f  ponse"<.....6.4/
+00000f80: 776f 726b 7370 6163 652f 7275 6e74 696d  workspace/runtim
+00000f90: 652d 636f 6e66 6967 7572 6174 696f 6e73  e-configurations
+00000fa0: 2f7b 6d6f 6475 6c65 7d2f 7b73 6572 7669  /{module}/{servi
+00000fb0: 6365 7d12 500a 044c 6f67 7312 162e 676f  ce}.P..Logs...go
+00000fc0: 6f67 6c65 2e70 726f 746f 6275 662e 456d  ogle.protobuf.Em
+00000fd0: 7074 791a 152e 6f62 7365 7276 6162 696c  pty...observabil
+00000fe0: 6974 792e 7630 2e4c 6f67 2217 82d3 e493  ity.v0.Log".....
+00000ff0: 0211 120f 2f77 6f72 6b73 7061 6365 2f6c  ..../workspace/l
+00001000: 6f67 7330 0112 700a 1041 6374 6976 654c  ogs0..p..ActiveL
+00001010: 6f67 4869 7374 6f72 7912 1c2e 6f62 7365  ogHistory...obse
+00001020: 7276 6162 696c 6974 792e 7630 2e4c 6f67  rvability.v0.Log
+00001030: 5265 7175 6573 741a 1d2e 6f62 7365 7276  Request...observ
+00001040: 6162 696c 6974 792e 7630 2e4c 6f67 5265  ability.v0.LogRe
+00001050: 7370 6f6e 7365 221f 82d3 e493 0219 1217  sponse".........
+00001060: 2f77 6f72 6b73 7061 6365 2f6c 6f67 732f  /workspace/logs/
+00001070: 6869 7374 6f72 7912 650a 0d47 6574 466c  history.e..GetFl
+00001080: 6f77 5374 6174 7573 1216 2e67 6f6f 676c  owStatus...googl
+00001090: 652e 7072 6f74 6f62 7566 2e45 6d70 7479  e.protobuf.Empty
+000010a0: 1a1c 2e6f 6273 6572 7661 6269 6c69 7479  ...observability
+000010b0: 2e76 302e 466c 6f77 5374 6174 7573 221e  .v0.FlowStatus".
+000010c0: 82d3 e493 0218 1216 2f77 6f72 6b73 7061  ......../workspa
+000010d0: 6365 2f66 6c6f 772f 7374 6174 7573 126f  ce/flow/status.o
+000010e0: 0a08 5374 6f70 466c 6f77 1221 2e6f 6273  ..StopFlow.!.obs
+000010f0: 6572 7661 6269 6c69 7479 2e76 302e 5374  ervability.v0.St
+00001100: 6f70 466c 6f77 5265 7175 6573 741a 222e  opFlowRequest.".
+00001110: 6f62 7365 7276 6162 696c 6974 792e 7630  observability.v0
+00001120: 2e53 746f 7046 6c6f 7752 6573 706f 6e73  .StopFlowRespons
+00001130: 6522 1c82 d3e4 9302 1622 142f 776f 726b  e"......."./work
+00001140: 7370 6163 652f 666c 6f77 2f73 746f 7012  space/flow/stop.
+00001150: 7b0a 0b44 6573 7472 6f79 466c 6f77 1224  {..DestroyFlow.$
+00001160: 2e6f 6273 6572 7661 6269 6c69 7479 2e76  .observability.v
+00001170: 302e 4465 7374 726f 7946 6c6f 7752 6571  0.DestroyFlowReq
+00001180: 7565 7374 1a25 2e6f 6273 6572 7661 6269  uest.%.observabi
+00001190: 6c69 7479 2e76 302e 4465 7374 726f 7946  lity.v0.DestroyF
+000011a0: 6c6f 7752 6573 706f 6e73 6522 1f82 d3e4  lowResponse"....
+000011b0: 9302 1922 172f 776f 726b 7370 6163 652f  ..."./workspace/
+000011c0: 666c 6f77 2f64 6573 7472 6f79 42b2 010a  flow/destroyB...
+000011d0: 1463 6f6d 2e6f 6273 6572 7661 6269 6c69  .com.observabili
+000011e0: 7479 2e76 3042 0843 6c69 5072 6f74 6f50  ty.v0B.CliProtoP
+000011f0: 015a 2f67 6974 6875 622e 636f 6d2f 636f  .Z/github.com/co
+00001200: 6465 666c 792d 6465 762f 636f 7265 2f67  defly-dev/core/g
+00001210: 656e 6572 6174 6564 2f67 6f2f 636c 692f  enerated/go/cli/
+00001220: 7630 a202 034f 5658 aa02 104f 6273 6572  v0...OVX...Obser
+00001230: 7661 6269 6c69 7479 2e56 30ca 0210 4f62  vability.V0...Ob
+00001240: 7365 7276 6162 696c 6974 795c 5630 e202  servability\V0..
+00001250: 1c4f 6273 6572 7661 6269 6c69 7479 5c56  .Observability\V
+00001260: 305c 4750 424d 6574 6164 6174 61ea 0211  0\GPBMetadata...
+00001270: 4f62 7365 7276 6162 696c 6974 793a 3a56  Observability::V
+00001280: 3062 0670 726f 746f 337a 0e63 6c69 2e76  0b.proto3z.cli.v
+00001290: 302e 636c 695f 7062 324e da0a 4445 5343  0.cli_pb2N..DESC
+000012a0: 5249 5054 4f52 73b2 0000 000a 1463 6f6d  RIPTORs......com
+000012b0: 2e6f 6273 6572 7661 6269 6c69 7479 2e76  .observability.v
+000012c0: 3042 0843 6c69 5072 6f74 6f50 015a 2f67  0B.CliProtoP.Z/g
+000012d0: 6974 6875 622e 636f 6d2f 636f 6465 666c  ithub.com/codefl
+000012e0: 792d 6465 762f 636f 7265 2f67 656e 6572  y-dev/core/gener
+000012f0: 6174 6564 2f67 6f2f 636c 692f 7630 a202  ated/go/cli/v0..
+00001300: 034f 5658 aa02 104f 6273 6572 7661 6269  .OVX...Observabi
+00001310: 6c69 7479 2e56 30ca 0210 4f62 7365 7276  lity.V0...Observ
+00001320: 6162 696c 6974 795c 5630 e202 1c4f 6273  ability\V0...Obs
+00001330: 6572 7661 6269 6c69 7479 5c56 305c 4750  ervability\V0\GP
+00001340: 424d 6574 6164 6174 61ea 0211 4f62 7365  BMetadata...Obse
+00001350: 7276 6162 696c 6974 793a 3a56 305a 045f  rvability::V0Z._
+00001360: 434c 49da 0450 696e 6773 0d00 0000 82d3  CLI..Pings......
+00001370: e493 0207 1205 2f70 696e 67da 1347 6574  ....../ping..Get
+00001380: 4167 656e 7449 6e66 6f72 6d61 7469 6f6e  AgentInformation
+00001390: 7322 0000 0082 d3e4 9302 1c12 1a2f 6167  s".........../ag
+000013a0: 656e 742f 7b61 6765 6e74 7d2f 696e 666f  ent/{agent}/info
+000013b0: 726d 6174 696f 6eda 1547 6574 576f 726b  rmation..GetWork
+000013c0: 7370 6163 6549 6e76 656e 746f 7279 731c  spaceInventorys.
+000013d0: 0000 0082 d3e4 9302 1612 142f 776f 726b  .........../work
+000013e0: 7370 6163 652f 696e 7665 6e74 6f72 79da  space/inventory.
+000013f0: 2247 6574 576f 726b 7370 6163 6553 6572  "GetWorkspaceSer
+00001400: 7669 6365 4465 7065 6e64 656e 6379 4772  viceDependencyGr
+00001410: 6170 6873 2b00 0000 82d3 e493 0225 1223  aphs+........%.#
+00001420: 2f77 6f72 6b73 7061 6365 2f73 6572 7669  /workspace/servi
+00001430: 6365 2d64 6570 656e 6465 6e63 792d 6772  ce-dependency-gr
+00001440: 6170 68da 2847 6574 576f 726b 7370 6163  aph.(GetWorkspac
+00001450: 6550 7562 6c69 634d 6f64 756c 6573 4465  ePublicModulesDe
+00001460: 7065 6e64 656e 6379 4772 6170 6873 2900  pendencyGraphs).
+00001470: 0000 82d3 e493 0223 1221 2f77 6f72 6b73  .......#.!/works
+00001480: 7061 6365 2f70 7562 6c69 632d 656e 6470  pace/public-endp
+00001490: 6f69 6e74 732d 6772 6170 68da 0947 6574  oints-graph..Get
+000014a0: 4163 7469 7665 731e 0000 0082 d3e4 9302  Actives.........
+000014b0: 1812 162f 776f 726b 7370 6163 652f 696e  .../workspace/in
+000014c0: 666f 726d 6174 696f 6eda 0c47 6574 4164  formation..GetAd
+000014d0: 6472 6573 7365 7373 4000 0000 82d3 e493  dressess@.......
+000014e0: 023a 1238 2f77 6f72 6b73 7061 6365 2f6e  .:.8/workspace/n
+000014f0: 6574 776f 726b 2d6d 6170 7069 6e67 2f7b  etwork-mapping/{
+00001500: 6d6f 6475 6c65 7d2f 7b73 6572 7669 6365  module}/{service
+00001510: 7d2f 7b65 6e64 706f 696e 747d da10 4765  }/{endpoint}..Ge
+00001520: 7443 6f6e 6669 6775 7261 7469 6f6e 7333  tConfigurations3
+00001530: 0000 0082 d3e4 9302 2d12 2b2f 776f 726b  ........-.+/work
+00001540: 7370 6163 652f 636f 6e66 6967 7572 6174  space/configurat
+00001550: 696f 6e2f 7b6d 6f64 756c 657d 2f7b 7365  ion/{module}/{se
+00001560: 7276 6963 657d da1d 4765 7444 6570 656e  rvice}..GetDepen
+00001570: 6465 6e63 6965 7343 6f6e 6669 6775 7261  denciesConfigura
+00001580: 7469 6f6e 7373 4100 0000 82d3 e493 023b  tionssA........;
+00001590: 1239 2f77 6f72 6b73 7061 6365 2f64 6570  .9/workspace/dep
+000015a0: 656e 6465 6e63 6965 732d 636f 6e66 6967  endencies-config
+000015b0: 7572 6174 696f 6e73 2f7b 6d6f 6475 6c65  urations/{module
+000015c0: 7d2f 7b73 6572 7669 6365 7dda 1847 6574  }/{service}..Get
+000015d0: 5275 6e74 696d 6543 6f6e 6669 6775 7261  RuntimeConfigura
+000015e0: 7469 6f6e 7373 3c00 0000 82d3 e493 0236  tionss<........6
+000015f0: 1234 2f77 6f72 6b73 7061 6365 2f72 756e  .4/workspace/run
+00001600: 7469 6d65 2d63 6f6e 6669 6775 7261 7469  time-configurati
+00001610: 6f6e 732f 7b6d 6f64 756c 657d 2f7b 7365  ons/{module}/{se
+00001620: 7276 6963 657d da04 4c6f 6773 7317 0000  rvice}..Logss...
+00001630: 0082 d3e4 9302 1112 0f2f 776f 726b 7370  ........./worksp
+00001640: 6163 652f 6c6f 6773 da10 4163 7469 7665  ace/logs..Active
+00001650: 4c6f 6748 6973 746f 7279 731f 0000 0082  LogHistorys.....
+00001660: d3e4 9302 1912 172f 776f 726b 7370 6163  ......./workspac
+00001670: 652f 6c6f 6773 2f68 6973 746f 7279 da0d  e/logs/history..
+00001680: 4765 7446 6c6f 7753 7461 7475 7373 1e00  GetFlowStatuss..
+00001690: 0000 82d3 e493 0218 1216 2f77 6f72 6b73  ........../works
+000016a0: 7061 6365 2f66 6c6f 772f 7374 6174 7573  pace/flow/status
+000016b0: da08 5374 6f70 466c 6f77 731c 0000 0082  ..StopFlows.....
+000016c0: d3e4 9302 1622 142f 776f 726b 7370 6163  ....."./workspac
+000016d0: 652f 666c 6f77 2f73 746f 70da 0b44 6573  e/flow/stop..Des
+000016e0: 7472 6f79 466c 6f77 731f 0000 0082 d3e4  troyFlows.......
+000016f0: 9302 1922 172f 776f 726b 7370 6163 652f  ..."./workspace/
+00001700: 666c 6f77 2f64 6573 7472 6f79 6976 0100  flow/destroyiv..
+00001710: 005a 1b5f 4745 5441 4745 4e54 494e 464f  .Z._GETAGENTINFO
+00001720: 524d 4154 494f 4e52 4551 5545 5354 69a8  RMATIONREQUESTi.
+00001730: 0100 0069 aa01 0000 5a13 5f4d 554c 5449  ...i....Z._MULTI
+00001740: 4752 4150 4852 4553 504f 4e53 4569 f701  GRAPHRESPONSEi..
+00001750: 0000 69f9 0100 005a 0f5f 4143 5449 5645  ..i....Z._ACTIVE
+00001760: 5245 5350 4f4e 5345 6959 0200 0069 5b02  RESPONSEiY...i[.
+00001770: 0000 5a13 5f52 554e 4e49 4e47 494e 464f  ..Z._RUNNINGINFO
+00001780: 524d 4154 494f 4e69 be02 0000 69c0 0200  RMATIONi....i...
+00001790: 005a 125f 4745 5441 4444 5245 5353 5245  .Z._GETADDRESSRE
+000017a0: 5155 4553 5469 2103 0000 6923 0300 005a  QUESTi!...i#...Z
+000017b0: 135f 4745 5441 4444 5245 5353 5245 5350  ._GETADDRESSRESP
+000017c0: 4f4e 5345 6951 0300 0069 5303 0000 5a18  ONSEiQ...iS...Z.
+000017d0: 5f47 4554 434f 4e46 4947 5552 4154 494f  _GETCONFIGURATIO
+000017e0: 4e52 4551 5545 5354 699e 0300 0069 a003  NREQUESTi....i..
+000017f0: 0000 5a19 5f47 4554 434f 4e46 4947 5552  ..Z._GETCONFIGUR
+00001800: 4154 494f 4e52 4553 504f 4e53 4569 f803  ATIONRESPONSEi..
+00001810: 0000 69fa 0300 005a 1a5f 4745 5443 4f4e  ..i....Z._GETCON
+00001820: 4649 4755 5241 5449 4f4e 5352 4553 504f  FIGURATIONSRESPO
+00001830: 4e53 4569 5504 0000 6957 0400 005a 0b5f  NSEiU...iW...Z._
+00001840: 464c 4f57 5354 4154 5553 6979 0400 0069  FLOWSTATUSiy...i
+00001850: 7b04 0000 5a10 5f53 544f 5046 4c4f 5752  {...Z._STOPFLOWR
+00001860: 4551 5545 5354 698c 0400 0069 8e04 0000  EQUESTi....i....
+00001870: 5a11 5f53 544f 5046 4c4f 5752 4553 504f  Z._STOPFLOWRESPO
+00001880: 4e53 4569 a004 0000 69a2 0400 005a 135f  NSEi....i....Z._
+00001890: 4445 5354 524f 5946 4c4f 5752 4551 5545  DESTROYFLOWREQUE
+000018a0: 5354 69b6 0400 0069 b804 0000 5a14 5f44  STi....i....Z._D
+000018b0: 4553 5452 4f59 464c 4f57 5245 5350 4f4e  ESTROYFLOWRESPON
+000018c0: 5345 69cd 0400 0069 d004 0000 6960 0c00  SEi....i....i`..
+000018d0: 0029 34da 075f 5f64 6f63 5f5f da0f 676f  .)4..__doc__..go
+000018e0: 6f67 6c65 2e70 726f 746f 6275 6672 0200  ogle.protobufr..
+000018f0: 0000 da0b 5f64 6573 6372 6970 746f 7272  ...._descriptorr
+00001900: 0300 0000 da10 5f64 6573 6372 6970 746f  ......_descripto
+00001910: 725f 706f 6f6c 7204 0000 00da 105f 7379  r_poolr......_sy
+00001920: 6d62 6f6c 5f64 6174 6162 6173 65da 1867  mbol_database..g
+00001930: 6f6f 676c 652e 7072 6f74 6f62 7566 2e69  oogle.protobuf.i
+00001940: 6e74 6572 6e61 6c72 0500 0000 da08 5f62  nternalr......_b
+00001950: 7569 6c64 6572 da07 4465 6661 756c 74da  uilder..Default.
+00001960: 075f 7379 6d5f 6462 da07 6261 7365 2e76  ._sym_db..base.v
+00001970: 3072 0600 0000 da1d 6261 7365 5f64 6f74  0r......base_dot
+00001980: 5f76 305f 646f 745f 656e 6470 6f69 6e74  _v0_dot_endpoint
+00001990: 5f5f 7062 3272 0700 0000 da1e 6261 7365  __pb2r......base
+000019a0: 5f64 6f74 5f76 305f 646f 745f 776f 726b  _dot_v0_dot_work
+000019b0: 7370 6163 655f 5f70 6232 7208 0000 005a  space__pb2r....Z
+000019c0: 2262 6173 655f 646f 745f 7630 5f64 6f74  "base_dot_v0_dot
+000019d0: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f5f  _configuration__
+000019e0: 7062 32da 1173 6572 7669 6365 732e 6167  pb2..services.ag
+000019f0: 656e 742e 7630 7209 0000 00da 2873 6572  ent.v0r.....(ser
+00001a00: 7669 6365 735f 646f 745f 6167 656e 745f  vices_dot_agent_
+00001a10: 646f 745f 7630 5f64 6f74 5f61 6765 6e74  dot_v0_dot_agent
+00001a20: 5f5f 7062 325a 1373 6572 7669 6365 732e  __pb2Z.services.
+00001a30: 7275 6e74 696d 652e 7630 720a 0000 005a  runtime.v0r....Z
+00001a40: 2c73 6572 7669 6365 735f 646f 745f 7275  ,services_dot_ru
+00001a50: 6e74 696d 655f 646f 745f 7630 5f64 6f74  ntime_dot_v0_dot
+00001a60: 5f72 756e 7469 6d65 5f5f 7062 32da 106f  _runtime__pb2..o
+00001a70: 6273 6572 7661 6269 6c69 7479 2e76 3072  bservability.v0r
+00001a80: 0b00 0000 5a27 6f62 7365 7276 6162 696c  ....Z'observabil
+00001a90: 6974 795f 646f 745f 7630 5f64 6f74 5f69  ity_dot_v0_dot_i
+00001aa0: 6e76 656e 746f 7279 5f5f 7062 3272 0c00  nventory__pb2r..
+00001ab0: 0000 da2a 6f62 7365 7276 6162 696c 6974  ...*observabilit
+00001ac0: 795f 646f 745f 7630 5f64 6f74 5f64 6570  y_dot_v0_dot_dep
+00001ad0: 656e 6465 6e63 6965 735f 5f70 6232 720d  endencies__pb2r.
+00001ae0: 0000 00da 226f 6273 6572 7661 6269 6c69  ...."observabili
+00001af0: 7479 5f64 6f74 5f76 305f 646f 745f 6c6f  ty_dot_v0_dot_lo
+00001b00: 6773 5f5f 7062 3272 0e00 0000 da22 676f  gs__pb2r....."go
+00001b10: 6f67 6c65 5f64 6f74 5f70 726f 746f 6275  ogle_dot_protobu
+00001b20: 665f 646f 745f 656d 7074 795f 5f70 6232  f_dot_empty__pb2
+00001b30: 5a0a 676f 6f67 6c65 2e61 7069 720f 0000  Z.google.apir...
+00001b40: 005a 2367 6f6f 676c 655f 646f 745f 6170  .Z#google_dot_ap
+00001b50: 695f 646f 745f 616e 6e6f 7461 7469 6f6e  i_dot_annotation
+00001b60: 735f 5f70 6232 7210 0000 00da 2667 6f6f  s__pb2r.....&goo
+00001b70: 676c 655f 646f 745f 7072 6f74 6f62 7566  gle_dot_protobuf
+00001b80: 5f64 6f74 5f74 696d 6573 7461 6d70 5f5f  _dot_timestamp__
+00001b90: 7062 32da 1141 6464 5365 7269 616c 697a  pb2..AddSerializ
+00001ba0: 6564 4669 6c65 7211 0000 00da 0767 6c6f  edFiler......glo
+00001bb0: 6261 6c73 da08 5f67 6c6f 6261 6c73 da1e  bals.._globals..
+00001bc0: 4275 696c 644d 6573 7361 6765 416e 6445  BuildMessageAndE
+00001bd0: 6e75 6d44 6573 6372 6970 746f 7273 da1e  numDescriptors..
+00001be0: 4275 696c 6454 6f70 4465 7363 7269 7074  BuildTopDescript
+00001bf0: 6f72 7341 6e64 4d65 7373 6167 6573 da12  orsAndMessages..
+00001c00: 5f55 5345 5f43 5f44 4553 4352 4950 544f  _USE_C_DESCRIPTO
+00001c10: 5253 da0f 5f6c 6f61 6465 645f 6f70 7469  RS.._loaded_opti
+00001c20: 6f6e 73da 135f 7365 7269 616c 697a 6564  ons.._serialized
+00001c30: 5f6f 7074 696f 6e73 da0f 6d65 7468 6f64  _options..method
+00001c40: 735f 6279 5f6e 616d 65da 115f 7365 7269  s_by_name.._seri
+00001c50: 616c 697a 6564 5f73 7461 7274 da0f 5f73  alized_start.._s
+00001c60: 6572 6961 6c69 7a65 645f 656e 64a9 0072  erialized_end..r
+00001c70: 3f00 0000 723f 0000 00fa 662f 5573 6572  ?...r?....f/User
+00001c80: 732f 616e 746f 696e 652f 4465 7665 6c6f  s/antoine/Develo
+00001c90: 706d 656e 742f 636f 6465 666c 792e 6465  pment/codefly.de
+00001ca0: 762f 636f 7265 2f67 656e 6572 6174 6564  v/core/generated
+00001cb0: 2f70 7974 686f 6e2f 636f 6465 666c 792d  /python/codefly-
+00001cc0: 636c 692f 636f 6465 666c 795f 636c 692f  cli/codefly_cli/
+00001cd0: 636c 692f 7630 2f63 6c69 5f70 6232 2e70  cli/v0/cli_pb2.p
+00001ce0: 79da 083c 6d6f 6475 6c65 3e01 0000 0073  y..<module>....s
+00001cf0: aa00 0000 0404 0c01 0c01 0c01 0c01 0803  ................
+00001d00: 0c03 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001d10: 0c01 0c01 0c01 0e03 0602 0c01 0e01 0801  ................
+00001d20: 0a01 0a01 1001 1001 1001 1001 1001 1001  ................
 00001d30: 1001 1001 1001 1001 1001 1001 1001 1001  ................
 00001d40: 1001 1001 1001 1001 1001 1001 1001 1001  ................
-00001d50: 1001 1001 1001 1001 1001 1001 0a01 0a01  ................
+00001d50: 1001 1001 1001 1001 1001 1001 1001 1001  ................
 00001d60: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00001d70: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00001d80: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00001d90: 0a01 0a01 0a01 0e01 04c2                 ..........
+00001d90: 0a01 0a01 0a01 0a01 0a01 0e01 04c2       ..............
```

### Comparing `codefly_cli-0.0.6/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 28562 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 926f 0000  o.......Y.Bf.o..
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 926f 0000  o.........Ff.o..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 6401 6404 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c08 6d09 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c0b 6d0c 5a0d 0100 6401 6407 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6408 6c10 6d11 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/cli/v0/cli_pb2.py` & `codefly_cli-0.0.7/codefly_cli/cli/v0/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/cli/v0/cli_pb2_grpc.py` & `codefly_cli-0.0.7/codefly_cli/cli/v0/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/codefly.py` & `codefly_cli-0.0.7/codefly_cli/codefly.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 1792 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 0007 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 0007 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c01 6d10 5a11  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2690 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 820a 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 820a 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6505 a00b a100  ..e.....Z.e.....
 00000070: a00d 6406 a101 5a0e 650f 8300 5a10 650a  ..d...Z.e...Z.e.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/google/api/annotations_pb2.py` & `codefly_cli-0.0.7/codefly_cli/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/google/api/http_pb2.py` & `codefly_cli-0.0.7/codefly_cli/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2474 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 aa09 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 aa09 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6505 a00b a100  ..e.....Z.e.....
 00000070: a00d 6406 a101 5a0e 650f 8300 5a10 650a  ..d...Z.e...Z.e.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 1837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 2d07 0000  o.......Y.Bf-...
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 2d07 0000  o.........Ff-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6505 a00b a100 a010 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2961 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 910b 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 910b 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c10 6d11 5a12  m.Z...d.d.l.m.Z.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 2985 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 a90b 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 a90b 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c01  ..e.....Z.d.d.l.
 00000070: 6d0d 5a0e 0100 6505 a00b a100 a00f 6407  m.Z...e.......d.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/dependencies_pb2.py` & `codefly_cli-0.0.7/codefly_cli/observability/v0/dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/inventory_pb2.py` & `codefly_cli-0.0.7/codefly_cli/observability/v0/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/logs_pb2.py` & `codefly_cli-0.0.7/codefly_cli/observability/v0/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/metrics_pb2.py` & `codefly_cli-0.0.7/codefly_cli/observability/v0/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/observability/v0/sessions_pb2.py` & `codefly_cli-0.0.7/codefly_cli/observability/v0/sessions_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 5107 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 f313 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 f313 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6505 a00b a100  ..e.....Z.e.....
 00000070: a00d 6406 a101 5a0e 650f 8300 5a10 650a  ..d...Z.e...Z.e.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 6560 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 a019 0000  o.......Y.Bf....
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 a019 0000  o.........Ff....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 f401 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6505 a00b a100  ..e.....Z.e.....
 00000070: a00d 6406 a101 5a0e 650f 8300 5a10 650a  ..d...Z.e...Z.e.
```

### Comparing `codefly_cli-0.0.6/codefly_cli/services/agent/v0/agent_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/agent/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/agent/v0/agent_pb2_grpc.py` & `codefly_cli-0.0.7/codefly_cli/services/agent/v0/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/agent/v0/communicate_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/agent/v0/communicate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/agent/v0/cyclonedx_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/agent/v0/cyclonedx_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/builder/v0/builder_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/builder/v0/builder_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/builder/v0/builder_pb2_grpc.py` & `codefly_cli-0.0.7/codefly_cli/services/builder/v0/builder_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/builder/v0/deployment_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/builder/v0/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/builder/v0/docker_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/builder/v0/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc` & `codefly_cli-0.0.7/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May 13 13:49:13 2024 UTC, .py size: 11345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 591a 4266 512c 0000  o.......Y.BfQ,..
+00000000: 6f0d 0d0a 0000 0000 f11d 4666 f42b 0000  o.........Ff.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3e03 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c01 6d04 5a05 0100 6401 6404 6c01  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6401 6405 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6507 a00b a100 5a0c 6401 6406 6c0d  ..e.....Z.d.d.l.
 00000070: 6d0e 5a0f 0100 6401 6407 6c0d 6d10 5a11  m.Z...d.d.l.m.Z.
@@ -64,15 +64,15 @@
 000003f0: 656e 7669 726f 6e6d 656e 745f 7062 3229  environment_pb2)
 00000400: 01da 0b73 6572 7669 6365 5f70 6232 2901  ...service_pb2).
 00000410: da0c 656e 6470 6f69 6e74 5f70 6232 2901  ..endpoint_pb2).
 00000420: da0b 6e65 7477 6f72 6b5f 7062 3229 01da  ..network_pb2)..
 00000430: 1163 6f6e 6669 6775 7261 7469 6f6e 5f70  .configuration_p
 00000440: 6232 2901 da09 6167 656e 745f 7062 3229  b2)...agent_pb2)
 00000450: 01da 0f63 6f6d 6d75 6e69 6361 7465 5f70  ...communicate_p
-00000460: 6232 731b 1100 000a 2173 6572 7669 6365  b2s.....!service
+00000460: 6232 73d9 1000 000a 2173 6572 7669 6365  b2s.....!service
 00000470: 732f 7275 6e74 696d 652f 7630 2f72 756e  s/runtime/v0/run
 00000480: 7469 6d65 2e70 726f 746f 1213 7365 7276  time.proto..serv
 00000490: 6963 6573 2e72 756e 7469 6d65 2e76 301a  ices.runtime.v0.
 000004a0: 1362 6173 652f 7630 2f73 636f 7065 2e70  .base/v0/scope.p
 000004b0: 726f 746f 1a12 6261 7365 2f76 302f 7370  roto..base/v0/sp
 000004c0: 6563 2e70 726f 746f 1a19 6261 7365 2f76  ec.proto..base/v
 000004d0: 302f 656e 7669 726f 6e6d 656e 742e 7072  0/environment.pr
@@ -199,273 +199,269 @@
 00000c60: 0e32 262e 7365 7276 6963 6573 2e72 756e  .2&.services.run
 00000c70: 7469 6d65 2e76 302e 5465 7374 5374 6174  time.v0.TestStat
 00000c80: 7573 2e53 7461 7475 7352 0573 7461 7465  us.StatusR.state
 00000c90: 1218 0a07 6d65 7373 6167 6518 0220 0128  ....message.. .(
 00000ca0: 0952 076d 6573 7361 6765 222d 0a06 5374  .R.message"-..St
 00000cb0: 6174 7573 120b 0a07 554e 4b4e 4f57 4e10  atus....UNKNOWN.
 00000cc0: 0012 0b0a 0753 5543 4345 5353 1001 1209  .....SUCCESS....
-00000cd0: 0a05 4552 524f 5210 0222 4f0a 0b54 6573  ..ERROR.."O..Tes
-00000ce0: 7452 6571 7565 7374 1240 0a0f 7275 6e74  tRequest.@..runt
-00000cf0: 696d 655f 636f 6e74 6578 7418 0120 0128  ime_context.. .(
-00000d00: 0b32 172e 6261 7365 2e76 302e 5275 6e74  .2..base.v0.Runt
-00000d10: 696d 6543 6f6e 7465 7874 520e 7275 6e74  imeContextR.runt
-00000d20: 696d 6543 6f6e 7465 7874 2247 0a0c 5465  imeContext"G..Te
-00000d30: 7374 5265 7370 6f6e 7365 1237 0a06 7374  stResponse.7..st
-00000d40: 6174 7573 1801 2001 280b 321f 2e73 6572  atus.. .(.2..ser
-00000d50: 7669 6365 732e 7275 6e74 696d 652e 7630  vices.runtime.v0
-00000d60: 2e54 6573 7453 7461 7475 7352 0673 7461  .TestStatusR.sta
-00000d70: 7475 7322 0d0a 0b53 746f 7052 6571 7565  tus"...StopReque
-00000d80: 7374 2293 010a 0a53 746f 7053 7461 7475  st"....StopStatu
-00000d90: 7312 3c0a 0573 7461 7465 1801 2001 280e  s.<..state.. .(.
-00000da0: 3226 2e73 6572 7669 6365 732e 7275 6e74  2&.services.runt
-00000db0: 696d 652e 7630 2e53 746f 7053 7461 7475  ime.v0.StopStatu
-00000dc0: 732e 5374 6174 7573 5205 7374 6174 6512  s.StatusR.state.
-00000dd0: 180a 076d 6573 7361 6765 1802 2001 2809  ...message.. .(.
-00000de0: 5207 6d65 7373 6167 6522 2d0a 0653 7461  R.message"-..Sta
-00000df0: 7475 7312 0b0a 0755 4e4b 4e4f 574e 1000  tus....UNKNOWN..
-00000e00: 120b 0a07 5355 4343 4553 5310 0112 090a  ....SUCCESS.....
-00000e10: 0545 5252 4f52 1002 2247 0a0c 5374 6f70  .ERROR.."G..Stop
-00000e20: 5265 7370 6f6e 7365 1237 0a06 7374 6174  Response.7..stat
-00000e30: 7573 1801 2001 280b 321f 2e73 6572 7669  us.. .(.2..servi
-00000e40: 6365 732e 7275 6e74 696d 652e 7630 2e53  ces.runtime.v0.S
-00000e50: 746f 7053 7461 7475 7352 0673 7461 7475  topStatusR.statu
-00000e60: 7322 100a 0e44 6573 7472 6f79 5265 7175  s"...DestroyRequ
-00000e70: 6573 7422 9901 0a0d 4465 7374 726f 7953  est"....DestroyS
-00000e80: 7461 7475 7312 3f0a 0573 7461 7465 1801  tatus.?..state..
-00000e90: 2001 280e 3229 2e73 6572 7669 6365 732e   .(.2).services.
-00000ea0: 7275 6e74 696d 652e 7630 2e44 6573 7472  runtime.v0.Destr
-00000eb0: 6f79 5374 6174 7573 2e53 7461 7475 7352  oyStatus.StatusR
-00000ec0: 0573 7461 7465 1218 0a07 6d65 7373 6167  .state....messag
-00000ed0: 6518 0220 0128 0952 076d 6573 7361 6765  e.. .(.R.message
-00000ee0: 222d 0a06 5374 6174 7573 120b 0a07 554e  "-..Status....UN
-00000ef0: 4b4e 4f57 4e10 0012 0b0a 0753 5543 4345  KNOWN......SUCCE
-00000f00: 5353 1001 1209 0a05 4552 524f 5210 0222  SS......ERROR.."
-00000f10: 4d0a 0f44 6573 7472 6f79 5265 7370 6f6e  M..DestroyRespon
-00000f20: 7365 123a 0a06 7374 6174 7573 1801 2001  se.:..status.. .
-00000f30: 280b 3222 2e73 6572 7669 6365 732e 7275  (.2".services.ru
-00000f40: 6e74 696d 652e 7630 2e44 6573 7472 6f79  ntime.v0.Destroy
-00000f50: 5374 6174 7573 5206 7374 6174 7573 2214  StatusR.status".
-00000f60: 0a12 496e 666f 726d 6174 696f 6e52 6571  ..InformationReq
-00000f70: 7565 7374 228c 010a 0c44 6573 6972 6564  uest"....Desired
-00000f80: 5374 6174 6512 3d0a 0573 7461 6765 1801  State.=..stage..
-00000f90: 2001 280e 3227 2e73 6572 7669 6365 732e   .(.2'.services.
-00000fa0: 7275 6e74 696d 652e 7630 2e44 6573 6972  runtime.v0.Desir
-00000fb0: 6564 5374 6174 652e 5374 6167 6552 0573  edState.StageR.s
-00000fc0: 7461 6765 223d 0a05 5374 6167 6512 0b0a  tage"=..Stage...
-00000fd0: 0755 4e4b 4e4f 574e 1000 1208 0a04 4e4f  .UNKNOWN......NO
-00000fe0: 4f50 1001 1208 0a04 4c4f 4144 1002 1208  OP......LOAD....
-00000ff0: 0a04 494e 4954 1003 1209 0a05 5354 4152  ..INIT......STAR
-00001000: 5410 0422 f503 0a13 496e 666f 726d 6174  T.."....Informat
-00001010: 696f 6e52 6573 706f 6e73 6512 460a 0d64  ionResponse.F..d
-00001020: 6573 6972 6564 5f73 7461 7465 1801 2001  esired_state.. .
-00001030: 280b 3221 2e73 6572 7669 6365 732e 7275  (.2!.services.ru
-00001040: 6e74 696d 652e 7630 2e44 6573 6972 6564  ntime.v0.Desired
-00001050: 5374 6174 6552 0c64 6573 6972 6564 5374  StateR.desiredSt
-00001060: 6174 6512 400a 0b6c 6f61 645f 7374 6174  ate.@..load_stat
-00001070: 7573 1802 2001 280b 321f 2e73 6572 7669  us.. .(.2..servi
-00001080: 6365 732e 7275 6e74 696d 652e 7630 2e4c  ces.runtime.v0.L
-00001090: 6f61 6453 7461 7475 7352 0a6c 6f61 6453  oadStatusR.loadS
-000010a0: 7461 7475 7312 400a 0b69 6e69 745f 7374  tatus.@..init_st
-000010b0: 6174 7573 1803 2001 280b 321f 2e73 6572  atus.. .(.2..ser
-000010c0: 7669 6365 732e 7275 6e74 696d 652e 7630  vices.runtime.v0
-000010d0: 2e49 6e69 7453 7461 7475 7352 0a69 6e69  .InitStatusR.ini
-000010e0: 7453 7461 7475 7312 430a 0c73 7461 7274  tStatus.C..start
-000010f0: 5f73 7461 7475 7318 0420 0128 0b32 202e  _status.. .(.2 .
-00001100: 7365 7276 6963 6573 2e72 756e 7469 6d65  services.runtime
-00001110: 2e76 302e 5374 6172 7453 7461 7475 7352  .v0.StartStatusR
-00001120: 0b73 7461 7274 5374 6174 7573 1240 0a0b  .startStatus.@..
-00001130: 7374 6f70 5f73 7461 7475 7318 0520 0128  stop_status.. .(
-00001140: 0b32 1f2e 7365 7276 6963 6573 2e72 756e  .2..services.run
-00001150: 7469 6d65 2e76 302e 5374 6f70 5374 6174  time.v0.StopStat
-00001160: 7573 520a 7374 6f70 5374 6174 7573 1249  usR.stopStatus.I
-00001170: 0a0e 4465 7374 726f 795f 7374 6174 7573  ..Destroy_status
-00001180: 1806 2001 280b 3222 2e73 6572 7669 6365  .. .(.2".service
-00001190: 732e 7275 6e74 696d 652e 7630 2e44 6573  s.runtime.v0.Des
-000011a0: 7472 6f79 5374 6174 7573 520d 4465 7374  troyStatusR.Dest
-000011b0: 726f 7953 7461 7475 7312 400a 0b74 6573  royStatus.@..tes
-000011c0: 745f 7374 6174 7573 1807 2001 280b 321f  t_status.. .(.2.
-000011d0: 2e73 6572 7669 6365 732e 7275 6e74 696d  .services.runtim
-000011e0: 652e 7630 2e54 6573 7453 7461 7475 7352  e.v0.TestStatusR
-000011f0: 0a74 6573 7453 7461 7475 7332 a605 0a07  .testStatus2....
-00001200: 5275 6e74 696d 6512 4d0a 044c 6f61 6412  Runtime.M..Load.
-00001210: 202e 7365 7276 6963 6573 2e72 756e 7469   .services.runti
-00001220: 6d65 2e76 302e 4c6f 6164 5265 7175 6573  me.v0.LoadReques
-00001230: 741a 212e 7365 7276 6963 6573 2e72 756e  t.!.services.run
-00001240: 7469 6d65 2e76 302e 4c6f 6164 5265 7370  time.v0.LoadResp
-00001250: 6f6e 7365 2200 124d 0a04 496e 6974 1220  onse"..M..Init. 
-00001260: 2e73 6572 7669 6365 732e 7275 6e74 696d  .services.runtim
-00001270: 652e 7630 2e49 6e69 7452 6571 7565 7374  e.v0.InitRequest
-00001280: 1a21 2e73 6572 7669 6365 732e 7275 6e74  .!.services.runt
-00001290: 696d 652e 7630 2e49 6e69 7452 6573 706f  ime.v0.InitRespo
-000012a0: 6e73 6522 0012 500a 0553 7461 7274 1221  nse"..P..Start.!
-000012b0: 2e73 6572 7669 6365 732e 7275 6e74 696d  .services.runtim
-000012c0: 652e 7630 2e53 7461 7274 5265 7175 6573  e.v0.StartReques
-000012d0: 741a 222e 7365 7276 6963 6573 2e72 756e  t.".services.run
-000012e0: 7469 6d65 2e76 302e 5374 6172 7452 6573  time.v0.StartRes
-000012f0: 706f 6e73 6522 0012 4d0a 0453 746f 7012  ponse"..M..Stop.
-00001300: 202e 7365 7276 6963 6573 2e72 756e 7469   .services.runti
-00001310: 6d65 2e76 302e 5374 6f70 5265 7175 6573  me.v0.StopReques
-00001320: 741a 212e 7365 7276 6963 6573 2e72 756e  t.!.services.run
-00001330: 7469 6d65 2e76 302e 5374 6f70 5265 7370  time.v0.StopResp
-00001340: 6f6e 7365 2200 1256 0a07 4465 7374 726f  onse"..V..Destro
-00001350: 7912 232e 7365 7276 6963 6573 2e72 756e  y.#.services.run
-00001360: 7469 6d65 2e76 302e 4465 7374 726f 7952  time.v0.DestroyR
-00001370: 6571 7565 7374 1a24 2e73 6572 7669 6365  equest.$.service
-00001380: 732e 7275 6e74 696d 652e 7630 2e44 6573  s.runtime.v0.Des
-00001390: 7472 6f79 5265 7370 6f6e 7365 2200 124d  troyResponse"..M
-000013a0: 0a04 5465 7374 1220 2e73 6572 7669 6365  ..Test. .service
-000013b0: 732e 7275 6e74 696d 652e 7630 2e54 6573  s.runtime.v0.Tes
-000013c0: 7452 6571 7565 7374 1a21 2e73 6572 7669  tRequest.!.servi
-000013d0: 6365 732e 7275 6e74 696d 652e 7630 2e54  ces.runtime.v0.T
-000013e0: 6573 7452 6573 706f 6e73 6522 0012 620a  estResponse"..b.
-000013f0: 0b49 6e66 6f72 6d61 7469 6f6e 1227 2e73  .Information.'.s
-00001400: 6572 7669 6365 732e 7275 6e74 696d 652e  ervices.runtime.
-00001410: 7630 2e49 6e66 6f72 6d61 7469 6f6e 5265  v0.InformationRe
-00001420: 7175 6573 741a 282e 7365 7276 6963 6573  quest.(.services
-00001430: 2e72 756e 7469 6d65 2e76 302e 496e 666f  .runtime.v0.Info
-00001440: 726d 6174 696f 6e52 6573 706f 6e73 6522  rmationResponse"
-00001450: 0012 510a 0b43 6f6d 6d75 6e69 6361 7465  ..Q..Communicate
-00001460: 1219 2e73 6572 7669 6365 732e 6167 656e  ...services.agen
-00001470: 742e 7630 2e45 6e67 6167 651a 252e 7365  t.v0.Engage.%.se
-00001480: 7276 6963 6573 2e61 6765 6e74 2e76 302e  rvices.agent.v0.
-00001490: 496e 666f 726d 6174 696f 6e52 6571 7565  InformationReque
-000014a0: 7374 2200 42d3 010a 1763 6f6d 2e73 6572  st".B....com.ser
-000014b0: 7669 6365 732e 7275 6e74 696d 652e 7630  vices.runtime.v0
-000014c0: 420c 5275 6e74 696d 6550 726f 746f 5001  B.RuntimeProtoP.
-000014d0: 5a3c 6769 7468 7562 2e63 6f6d 2f63 6f64  Z<github.com/cod
-000014e0: 6566 6c79 2d64 6576 2f63 6f72 652f 6765  efly-dev/core/ge
-000014f0: 6e65 7261 7465 642f 676f 2f73 6572 7669  nerated/go/servi
-00001500: 6365 732f 7275 6e74 696d 652f 7630 a202  ces/runtime/v0..
-00001510: 0353 5256 aa02 1353 6572 7669 6365 732e  .SRV...Services.
-00001520: 5275 6e74 696d 652e 5630 ca02 1353 6572  Runtime.V0...Ser
-00001530: 7669 6365 735c 5275 6e74 696d 655c 5630  vices\Runtime\V0
-00001540: e202 1f53 6572 7669 6365 735c 5275 6e74  ...Services\Runt
-00001550: 696d 655c 5630 5c47 5042 4d65 7461 6461  ime\V0\GPBMetada
-00001560: 7461 ea02 1553 6572 7669 6365 733a 3a52  ta...Services::R
-00001570: 756e 7469 6d65 3a3a 5630 6206 7072 6f74  untime::V0b.prot
-00001580: 6f33 7a1f 7365 7276 6963 6573 2e72 756e  o3z.services.run
-00001590: 7469 6d65 2e76 302e 7275 6e74 696d 655f  time.v0.runtime_
-000015a0: 7062 324e da0a 4445 5343 5249 5054 4f52  pb2N..DESCRIPTOR
-000015b0: 73d3 0000 000a 1763 6f6d 2e73 6572 7669  s......com.servi
-000015c0: 6365 732e 7275 6e74 696d 652e 7630 420c  ces.runtime.v0B.
-000015d0: 5275 6e74 696d 6550 726f 746f 5001 5a3c  RuntimeProtoP.Z<
-000015e0: 6769 7468 7562 2e63 6f6d 2f63 6f64 6566  github.com/codef
-000015f0: 6c79 2d64 6576 2f63 6f72 652f 6765 6e65  ly-dev/core/gene
-00001600: 7261 7465 642f 676f 2f73 6572 7669 6365  rated/go/service
-00001610: 732f 7275 6e74 696d 652f 7630 a202 0353  s/runtime/v0...S
-00001620: 5256 aa02 1353 6572 7669 6365 732e 5275  RV...Services.Ru
-00001630: 6e74 696d 652e 5630 ca02 1353 6572 7669  ntime.V0...Servi
-00001640: 6365 735c 5275 6e74 696d 655c 5630 e202  ces\Runtime\V0..
-00001650: 1f53 6572 7669 6365 735c 5275 6e74 696d  .Services\Runtim
-00001660: 655c 5630 5c47 5042 4d65 7461 6461 7461  e\V0\GPBMetadata
-00001670: ea02 1553 6572 7669 6365 733a 3a52 756e  ...Services::Run
-00001680: 7469 6d65 3a3a 5630 6926 0100 005a 0b5f  time::V0i&...Z._
-00001690: 4c4f 4144 5354 4154 5553 69b7 0100 0069  LOADSTATUSi....i
-000016a0: 8c01 0000 5a12 5f4c 4f41 4453 5441 5455  ....Z._LOADSTATU
-000016b0: 535f 5354 4154 5553 69ba 0100 005a 0c5f  S_STATUSi....Z._
-000016c0: 4c4f 4144 5245 5155 4553 5469 8302 0000  LOADREQUESTi....
-000016d0: 6986 0200 005a 0d5f 4c4f 4144 5245 5350  i....Z._LOADRESP
-000016e0: 4f4e 5345 692a 0300 0069 2d03 0000 5a0b  ONSEi*...i-...Z.
-000016f0: 5f49 4e49 5453 5441 5455 5369 be03 0000  _INITSTATUSi....
-00001700: 5a12 5f49 4e49 5453 5441 5455 535f 5354  Z._INITSTATUS_ST
-00001710: 4154 5553 69c1 0300 005a 0c5f 494e 4954  ATUSi....Z._INIT
-00001720: 5245 5155 4553 5469 4605 0000 6949 0500  REQUESTiF...iI..
-00001730: 005a 0d5f 494e 4954 5245 5350 4f4e 5345  .Z._INITRESPONSE
-00001740: 6965 0600 0069 6806 0000 5a0d 5f53 5441  ie...ih...Z._STA
-00001750: 5254 5245 5155 4553 5469 f906 0000 69fc  RTREQUESTi....i.
-00001760: 0600 005a 0c5f 5354 4152 5453 5441 5455  ...Z._STARTSTATU
-00001770: 5369 9107 0000 6964 0700 005a 135f 5354  Si....id...Z._ST
-00001780: 4152 5453 5441 5455 535f 5354 4154 5553  ARTSTATUS_STATUS
-00001790: 6993 0700 005a 0e5f 5354 4152 5452 4553  i....Z._STARTRES
-000017a0: 504f 4e53 4569 dc07 0000 69df 0700 005a  PONSEi....i....Z
-000017b0: 0b5f 5445 5354 5354 4154 5553 6972 0800  ._TESTSTATUSir..
-000017c0: 0069 4508 0000 5a12 5f54 4553 5453 5441  .iE...Z._TESTSTA
-000017d0: 5455 535f 5354 4154 5553 6974 0800 005a  TUS_STATUSit...Z
-000017e0: 0c5f 5445 5354 5245 5155 4553 5469 c308  ._TESTREQUESTi..
-000017f0: 0000 69c5 0800 005a 0d5f 5445 5354 5245  ..i....Z._TESTRE
-00001800: 5350 4f4e 5345 690c 0900 0069 0e09 0000  SPONSEi....i....
-00001810: 5a0c 5f53 544f 5052 4551 5545 5354 691b  Z._STOPREQUESTi.
-00001820: 0900 0069 1e09 0000 5a0b 5f53 544f 5053  ...i....Z._STOPS
-00001830: 5441 5455 5369 b109 0000 5a12 5f53 544f  TATUSi....Z._STO
-00001840: 5053 5441 5455 535f 5354 4154 5553 69b3  PSTATUS_STATUSi.
-00001850: 0900 005a 0d5f 5354 4f50 5245 5350 4f4e  ...Z._STOPRESPON
-00001860: 5345 69fa 0900 0069 fc09 0000 5a0f 5f44  SEi....i....Z._D
-00001870: 4553 5452 4f59 5245 5155 4553 5469 0c0a  ESTROYREQUESTi..
-00001880: 0000 690f 0a00 005a 0e5f 4445 5354 524f  ..i....Z._DESTRO
-00001890: 5953 5441 5455 5369 a80a 0000 5a15 5f44  YSTATUSi....Z._D
-000018a0: 4553 5452 4f59 5354 4154 5553 5f53 5441  ESTROYSTATUS_STA
-000018b0: 5455 5369 aa0a 0000 5a10 5f44 4553 5452  TUSi....Z._DESTR
-000018c0: 4f59 5245 5350 4f4e 5345 69f7 0a00 0069  OYRESPONSEi....i
-000018d0: f90a 0000 5a13 5f49 4e46 4f52 4d41 5449  ....Z._INFORMATI
-000018e0: 4f4e 5245 5155 4553 5469 0d0b 0000 6910  ONREQUESTi....i.
-000018f0: 0b00 005a 0d5f 4445 5349 5245 4453 5441  ...Z._DESIREDSTA
-00001900: 5445 699c 0b00 0069 5f0b 0000 5a13 5f44  TEi....i_...Z._D
-00001910: 4553 4952 4544 5354 4154 455f 5354 4147  ESIREDSTATE_STAG
-00001920: 4569 9f0b 0000 5a14 5f49 4e46 4f52 4d41  Ei....Z._INFORMA
-00001930: 5449 4f4e 5245 5350 4f4e 5345 6994 0d00  TIONRESPONSEi...
-00001940: 0069 970d 0000 5a08 5f52 554e 5449 4d45  .i....Z._RUNTIME
-00001950: 693d 1000 0029 2cda 075f 5f64 6f63 5f5f  i=...),..__doc__
-00001960: da0f 676f 6f67 6c65 2e70 726f 746f 6275  ..google.protobu
-00001970: 6672 0200 0000 da0b 5f64 6573 6372 6970  fr......_descrip
-00001980: 746f 7272 0300 0000 da10 5f64 6573 6372  torr......_descr
-00001990: 6970 746f 725f 706f 6f6c 7204 0000 00da  iptor_poolr.....
-000019a0: 105f 7379 6d62 6f6c 5f64 6174 6162 6173  ._symbol_databas
-000019b0: 65da 1867 6f6f 676c 652e 7072 6f74 6f62  e..google.protob
-000019c0: 7566 2e69 6e74 6572 6e61 6c72 0500 0000  uf.internalr....
-000019d0: da08 5f62 7569 6c64 6572 da07 4465 6661  .._builder..Defa
-000019e0: 756c 74da 075f 7379 6d5f 6462 da07 6261  ult.._sym_db..ba
-000019f0: 7365 2e76 3072 0600 0000 da1a 6261 7365  se.v0r......base
-00001a00: 5f64 6f74 5f76 305f 646f 745f 7363 6f70  _dot_v0_dot_scop
-00001a10: 655f 5f70 6232 7207 0000 005a 1962 6173  e__pb2r....Z.bas
-00001a20: 655f 646f 745f 7630 5f64 6f74 5f73 7065  e_dot_v0_dot_spe
-00001a30: 635f 5f70 6232 7208 0000 005a 2062 6173  c__pb2r....Z bas
-00001a40: 655f 646f 745f 7630 5f64 6f74 5f65 6e76  e_dot_v0_dot_env
-00001a50: 6972 6f6e 6d65 6e74 5f5f 7062 3272 0900  ironment__pb2r..
-00001a60: 0000 da1c 6261 7365 5f64 6f74 5f76 305f  ....base_dot_v0_
-00001a70: 646f 745f 7365 7276 6963 655f 5f70 6232  dot_service__pb2
-00001a80: 720a 0000 00da 1d62 6173 655f 646f 745f  r......base_dot_
-00001a90: 7630 5f64 6f74 5f65 6e64 706f 696e 745f  v0_dot_endpoint_
-00001aa0: 5f70 6232 720b 0000 005a 1c62 6173 655f  _pb2r....Z.base_
-00001ab0: 646f 745f 7630 5f64 6f74 5f6e 6574 776f  dot_v0_dot_netwo
-00001ac0: 726b 5f5f 7062 3272 0c00 0000 da22 6261  rk__pb2r....."ba
-00001ad0: 7365 5f64 6f74 5f76 305f 646f 745f 636f  se_dot_v0_dot_co
-00001ae0: 6e66 6967 7572 6174 696f 6e5f 5f70 6232  nfiguration__pb2
-00001af0: da11 7365 7276 6963 6573 2e61 6765 6e74  ..services.agent
-00001b00: 2e76 3072 0d00 0000 da28 7365 7276 6963  .v0r.....(servic
-00001b10: 6573 5f64 6f74 5f61 6765 6e74 5f64 6f74  es_dot_agent_dot
-00001b20: 5f76 305f 646f 745f 6167 656e 745f 5f70  _v0_dot_agent__p
-00001b30: 6232 720e 0000 005a 2e73 6572 7669 6365  b2r....Z.service
-00001b40: 735f 646f 745f 6167 656e 745f 646f 745f  s_dot_agent_dot_
-00001b50: 7630 5f64 6f74 5f63 6f6d 6d75 6e69 6361  v0_dot_communica
-00001b60: 7465 5f5f 7062 32da 1141 6464 5365 7269  te__pb2..AddSeri
-00001b70: 616c 697a 6564 4669 6c65 720f 0000 00da  alizedFiler.....
-00001b80: 0767 6c6f 6261 6c73 da08 5f67 6c6f 6261  .globals.._globa
-00001b90: 6c73 da1e 4275 696c 644d 6573 7361 6765  ls..BuildMessage
-00001ba0: 416e 6445 6e75 6d44 6573 6372 6970 746f  AndEnumDescripto
-00001bb0: 7273 da1e 4275 696c 6454 6f70 4465 7363  rs..BuildTopDesc
-00001bc0: 7269 7074 6f72 7341 6e64 4d65 7373 6167  riptorsAndMessag
-00001bd0: 6573 da12 5f55 5345 5f43 5f44 4553 4352  es.._USE_C_DESCR
-00001be0: 4950 544f 5253 da0f 5f6c 6f61 6465 645f  IPTORS.._loaded_
-00001bf0: 6f70 7469 6f6e 73da 135f 7365 7269 616c  options.._serial
-00001c00: 697a 6564 5f6f 7074 696f 6e73 da11 5f73  ized_options.._s
-00001c10: 6572 6961 6c69 7a65 645f 7374 6172 74da  erialized_start.
-00001c20: 0f5f 7365 7269 616c 697a 6564 5f65 6e64  ._serialized_end
-00001c30: a900 722a 0000 0072 2a00 0000 fa77 2f55  ..r*...r*....w/U
-00001c40: 7365 7273 2f61 6e74 6f69 6e65 2f44 6576  sers/antoine/Dev
-00001c50: 656c 6f70 6d65 6e74 2f63 6f64 6566 6c79  elopment/codefly
-00001c60: 2e64 6576 2f63 6f72 652f 6765 6e65 7261  .dev/core/genera
-00001c70: 7465 642f 7079 7468 6f6e 2f63 6f64 6566  ted/python/codef
-00001c80: 6c79 2d63 6c69 2f63 6f64 6566 6c79 5f63  ly-cli/codefly_c
-00001c90: 6c69 2f73 6572 7669 6365 732f 7275 6e74  li/services/runt
-00001ca0: 696d 652f 7630 2f72 756e 7469 6d65 5f70  ime/v0/runtime_p
-00001cb0: 6232 2e70 79da 083c 6d6f 6475 6c65 3e01  b2.py..<module>.
-00001cc0: 0000 0073 a200 0000 0404 0c01 0c01 0c01  ...s............
-00001cd0: 0c01 0803 0c03 0c01 0c01 0c01 0c01 0c01  ................
-00001ce0: 0c01 0c01 0c01 0e03 0602 0c01 0e01 0801  ................
+00000cd0: 0a05 4552 524f 5210 0222 0d0a 0b54 6573  ..ERROR.."...Tes
+00000ce0: 7452 6571 7565 7374 2247 0a0c 5465 7374  tRequest"G..Test
+00000cf0: 5265 7370 6f6e 7365 1237 0a06 7374 6174  Response.7..stat
+00000d00: 7573 1801 2001 280b 321f 2e73 6572 7669  us.. .(.2..servi
+00000d10: 6365 732e 7275 6e74 696d 652e 7630 2e54  ces.runtime.v0.T
+00000d20: 6573 7453 7461 7475 7352 0673 7461 7475  estStatusR.statu
+00000d30: 7322 0d0a 0b53 746f 7052 6571 7565 7374  s"...StopRequest
+00000d40: 2293 010a 0a53 746f 7053 7461 7475 7312  "....StopStatus.
+00000d50: 3c0a 0573 7461 7465 1801 2001 280e 3226  <..state.. .(.2&
+00000d60: 2e73 6572 7669 6365 732e 7275 6e74 696d  .services.runtim
+00000d70: 652e 7630 2e53 746f 7053 7461 7475 732e  e.v0.StopStatus.
+00000d80: 5374 6174 7573 5205 7374 6174 6512 180a  StatusR.state...
+00000d90: 076d 6573 7361 6765 1802 2001 2809 5207  .message.. .(.R.
+00000da0: 6d65 7373 6167 6522 2d0a 0653 7461 7475  message"-..Statu
+00000db0: 7312 0b0a 0755 4e4b 4e4f 574e 1000 120b  s....UNKNOWN....
+00000dc0: 0a07 5355 4343 4553 5310 0112 090a 0545  ..SUCCESS......E
+00000dd0: 5252 4f52 1002 2247 0a0c 5374 6f70 5265  RROR.."G..StopRe
+00000de0: 7370 6f6e 7365 1237 0a06 7374 6174 7573  sponse.7..status
+00000df0: 1801 2001 280b 321f 2e73 6572 7669 6365  .. .(.2..service
+00000e00: 732e 7275 6e74 696d 652e 7630 2e53 746f  s.runtime.v0.Sto
+00000e10: 7053 7461 7475 7352 0673 7461 7475 7322  pStatusR.status"
+00000e20: 100a 0e44 6573 7472 6f79 5265 7175 6573  ...DestroyReques
+00000e30: 7422 9901 0a0d 4465 7374 726f 7953 7461  t"....DestroySta
+00000e40: 7475 7312 3f0a 0573 7461 7465 1801 2001  tus.?..state.. .
+00000e50: 280e 3229 2e73 6572 7669 6365 732e 7275  (.2).services.ru
+00000e60: 6e74 696d 652e 7630 2e44 6573 7472 6f79  ntime.v0.Destroy
+00000e70: 5374 6174 7573 2e53 7461 7475 7352 0573  Status.StatusR.s
+00000e80: 7461 7465 1218 0a07 6d65 7373 6167 6518  tate....message.
+00000e90: 0220 0128 0952 076d 6573 7361 6765 222d  . .(.R.message"-
+00000ea0: 0a06 5374 6174 7573 120b 0a07 554e 4b4e  ..Status....UNKN
+00000eb0: 4f57 4e10 0012 0b0a 0753 5543 4345 5353  OWN......SUCCESS
+00000ec0: 1001 1209 0a05 4552 524f 5210 0222 4d0a  ......ERROR.."M.
+00000ed0: 0f44 6573 7472 6f79 5265 7370 6f6e 7365  .DestroyResponse
+00000ee0: 123a 0a06 7374 6174 7573 1801 2001 280b  .:..status.. .(.
+00000ef0: 3222 2e73 6572 7669 6365 732e 7275 6e74  2".services.runt
+00000f00: 696d 652e 7630 2e44 6573 7472 6f79 5374  ime.v0.DestroySt
+00000f10: 6174 7573 5206 7374 6174 7573 2214 0a12  atusR.status"...
+00000f20: 496e 666f 726d 6174 696f 6e52 6571 7565  InformationReque
+00000f30: 7374 228c 010a 0c44 6573 6972 6564 5374  st"....DesiredSt
+00000f40: 6174 6512 3d0a 0573 7461 6765 1801 2001  ate.=..stage.. .
+00000f50: 280e 3227 2e73 6572 7669 6365 732e 7275  (.2'.services.ru
+00000f60: 6e74 696d 652e 7630 2e44 6573 6972 6564  ntime.v0.Desired
+00000f70: 5374 6174 652e 5374 6167 6552 0573 7461  State.StageR.sta
+00000f80: 6765 223d 0a05 5374 6167 6512 0b0a 0755  ge"=..Stage....U
+00000f90: 4e4b 4e4f 574e 1000 1208 0a04 4e4f 4f50  NKNOWN......NOOP
+00000fa0: 1001 1208 0a04 4c4f 4144 1002 1208 0a04  ......LOAD......
+00000fb0: 494e 4954 1003 1209 0a05 5354 4152 5410  INIT......START.
+00000fc0: 0422 f503 0a13 496e 666f 726d 6174 696f  ."....Informatio
+00000fd0: 6e52 6573 706f 6e73 6512 460a 0d64 6573  nResponse.F..des
+00000fe0: 6972 6564 5f73 7461 7465 1801 2001 280b  ired_state.. .(.
+00000ff0: 3221 2e73 6572 7669 6365 732e 7275 6e74  2!.services.runt
+00001000: 696d 652e 7630 2e44 6573 6972 6564 5374  ime.v0.DesiredSt
+00001010: 6174 6552 0c64 6573 6972 6564 5374 6174  ateR.desiredStat
+00001020: 6512 400a 0b6c 6f61 645f 7374 6174 7573  e.@..load_status
+00001030: 1802 2001 280b 321f 2e73 6572 7669 6365  .. .(.2..service
+00001040: 732e 7275 6e74 696d 652e 7630 2e4c 6f61  s.runtime.v0.Loa
+00001050: 6453 7461 7475 7352 0a6c 6f61 6453 7461  dStatusR.loadSta
+00001060: 7475 7312 400a 0b69 6e69 745f 7374 6174  tus.@..init_stat
+00001070: 7573 1803 2001 280b 321f 2e73 6572 7669  us.. .(.2..servi
+00001080: 6365 732e 7275 6e74 696d 652e 7630 2e49  ces.runtime.v0.I
+00001090: 6e69 7453 7461 7475 7352 0a69 6e69 7453  nitStatusR.initS
+000010a0: 7461 7475 7312 430a 0c73 7461 7274 5f73  tatus.C..start_s
+000010b0: 7461 7475 7318 0420 0128 0b32 202e 7365  tatus.. .(.2 .se
+000010c0: 7276 6963 6573 2e72 756e 7469 6d65 2e76  rvices.runtime.v
+000010d0: 302e 5374 6172 7453 7461 7475 7352 0b73  0.StartStatusR.s
+000010e0: 7461 7274 5374 6174 7573 1240 0a0b 7374  tartStatus.@..st
+000010f0: 6f70 5f73 7461 7475 7318 0520 0128 0b32  op_status.. .(.2
+00001100: 1f2e 7365 7276 6963 6573 2e72 756e 7469  ..services.runti
+00001110: 6d65 2e76 302e 5374 6f70 5374 6174 7573  me.v0.StopStatus
+00001120: 520a 7374 6f70 5374 6174 7573 1249 0a0e  R.stopStatus.I..
+00001130: 4465 7374 726f 795f 7374 6174 7573 1806  Destroy_status..
+00001140: 2001 280b 3222 2e73 6572 7669 6365 732e   .(.2".services.
+00001150: 7275 6e74 696d 652e 7630 2e44 6573 7472  runtime.v0.Destr
+00001160: 6f79 5374 6174 7573 520d 4465 7374 726f  oyStatusR.Destro
+00001170: 7953 7461 7475 7312 400a 0b74 6573 745f  yStatus.@..test_
+00001180: 7374 6174 7573 1807 2001 280b 321f 2e73  status.. .(.2..s
+00001190: 6572 7669 6365 732e 7275 6e74 696d 652e  ervices.runtime.
+000011a0: 7630 2e54 6573 7453 7461 7475 7352 0a74  v0.TestStatusR.t
+000011b0: 6573 7453 7461 7475 7332 a605 0a07 5275  estStatus2....Ru
+000011c0: 6e74 696d 6512 4d0a 044c 6f61 6412 202e  ntime.M..Load. .
+000011d0: 7365 7276 6963 6573 2e72 756e 7469 6d65  services.runtime
+000011e0: 2e76 302e 4c6f 6164 5265 7175 6573 741a  .v0.LoadRequest.
+000011f0: 212e 7365 7276 6963 6573 2e72 756e 7469  !.services.runti
+00001200: 6d65 2e76 302e 4c6f 6164 5265 7370 6f6e  me.v0.LoadRespon
+00001210: 7365 2200 124d 0a04 496e 6974 1220 2e73  se"..M..Init. .s
+00001220: 6572 7669 6365 732e 7275 6e74 696d 652e  ervices.runtime.
+00001230: 7630 2e49 6e69 7452 6571 7565 7374 1a21  v0.InitRequest.!
+00001240: 2e73 6572 7669 6365 732e 7275 6e74 696d  .services.runtim
+00001250: 652e 7630 2e49 6e69 7452 6573 706f 6e73  e.v0.InitRespons
+00001260: 6522 0012 500a 0553 7461 7274 1221 2e73  e"..P..Start.!.s
+00001270: 6572 7669 6365 732e 7275 6e74 696d 652e  ervices.runtime.
+00001280: 7630 2e53 7461 7274 5265 7175 6573 741a  v0.StartRequest.
+00001290: 222e 7365 7276 6963 6573 2e72 756e 7469  ".services.runti
+000012a0: 6d65 2e76 302e 5374 6172 7452 6573 706f  me.v0.StartRespo
+000012b0: 6e73 6522 0012 4d0a 0453 746f 7012 202e  nse"..M..Stop. .
+000012c0: 7365 7276 6963 6573 2e72 756e 7469 6d65  services.runtime
+000012d0: 2e76 302e 5374 6f70 5265 7175 6573 741a  .v0.StopRequest.
+000012e0: 212e 7365 7276 6963 6573 2e72 756e 7469  !.services.runti
+000012f0: 6d65 2e76 302e 5374 6f70 5265 7370 6f6e  me.v0.StopRespon
+00001300: 7365 2200 1256 0a07 4465 7374 726f 7912  se"..V..Destroy.
+00001310: 232e 7365 7276 6963 6573 2e72 756e 7469  #.services.runti
+00001320: 6d65 2e76 302e 4465 7374 726f 7952 6571  me.v0.DestroyReq
+00001330: 7565 7374 1a24 2e73 6572 7669 6365 732e  uest.$.services.
+00001340: 7275 6e74 696d 652e 7630 2e44 6573 7472  runtime.v0.Destr
+00001350: 6f79 5265 7370 6f6e 7365 2200 124d 0a04  oyResponse"..M..
+00001360: 5465 7374 1220 2e73 6572 7669 6365 732e  Test. .services.
+00001370: 7275 6e74 696d 652e 7630 2e54 6573 7452  runtime.v0.TestR
+00001380: 6571 7565 7374 1a21 2e73 6572 7669 6365  equest.!.service
+00001390: 732e 7275 6e74 696d 652e 7630 2e54 6573  s.runtime.v0.Tes
+000013a0: 7452 6573 706f 6e73 6522 0012 620a 0b49  tResponse"..b..I
+000013b0: 6e66 6f72 6d61 7469 6f6e 1227 2e73 6572  nformation.'.ser
+000013c0: 7669 6365 732e 7275 6e74 696d 652e 7630  vices.runtime.v0
+000013d0: 2e49 6e66 6f72 6d61 7469 6f6e 5265 7175  .InformationRequ
+000013e0: 6573 741a 282e 7365 7276 6963 6573 2e72  est.(.services.r
+000013f0: 756e 7469 6d65 2e76 302e 496e 666f 726d  untime.v0.Inform
+00001400: 6174 696f 6e52 6573 706f 6e73 6522 0012  ationResponse"..
+00001410: 510a 0b43 6f6d 6d75 6e69 6361 7465 1219  Q..Communicate..
+00001420: 2e73 6572 7669 6365 732e 6167 656e 742e  .services.agent.
+00001430: 7630 2e45 6e67 6167 651a 252e 7365 7276  v0.Engage.%.serv
+00001440: 6963 6573 2e61 6765 6e74 2e76 302e 496e  ices.agent.v0.In
+00001450: 666f 726d 6174 696f 6e52 6571 7565 7374  formationRequest
+00001460: 2200 42d3 010a 1763 6f6d 2e73 6572 7669  ".B....com.servi
+00001470: 6365 732e 7275 6e74 696d 652e 7630 420c  ces.runtime.v0B.
+00001480: 5275 6e74 696d 6550 726f 746f 5001 5a3c  RuntimeProtoP.Z<
+00001490: 6769 7468 7562 2e63 6f6d 2f63 6f64 6566  github.com/codef
+000014a0: 6c79 2d64 6576 2f63 6f72 652f 6765 6e65  ly-dev/core/gene
+000014b0: 7261 7465 642f 676f 2f73 6572 7669 6365  rated/go/service
+000014c0: 732f 7275 6e74 696d 652f 7630 a202 0353  s/runtime/v0...S
+000014d0: 5256 aa02 1353 6572 7669 6365 732e 5275  RV...Services.Ru
+000014e0: 6e74 696d 652e 5630 ca02 1353 6572 7669  ntime.V0...Servi
+000014f0: 6365 735c 5275 6e74 696d 655c 5630 e202  ces\Runtime\V0..
+00001500: 1f53 6572 7669 6365 735c 5275 6e74 696d  .Services\Runtim
+00001510: 655c 5630 5c47 5042 4d65 7461 6461 7461  e\V0\GPBMetadata
+00001520: ea02 1553 6572 7669 6365 733a 3a52 756e  ...Services::Run
+00001530: 7469 6d65 3a3a 5630 6206 7072 6f74 6f33  time::V0b.proto3
+00001540: 7a1f 7365 7276 6963 6573 2e72 756e 7469  z.services.runti
+00001550: 6d65 2e76 302e 7275 6e74 696d 655f 7062  me.v0.runtime_pb
+00001560: 324e da0a 4445 5343 5249 5054 4f52 73d3  2N..DESCRIPTORs.
+00001570: 0000 000a 1763 6f6d 2e73 6572 7669 6365  .....com.service
+00001580: 732e 7275 6e74 696d 652e 7630 420c 5275  s.runtime.v0B.Ru
+00001590: 6e74 696d 6550 726f 746f 5001 5a3c 6769  ntimeProtoP.Z<gi
+000015a0: 7468 7562 2e63 6f6d 2f63 6f64 6566 6c79  thub.com/codefly
+000015b0: 2d64 6576 2f63 6f72 652f 6765 6e65 7261  -dev/core/genera
+000015c0: 7465 642f 676f 2f73 6572 7669 6365 732f  ted/go/services/
+000015d0: 7275 6e74 696d 652f 7630 a202 0353 5256  runtime/v0...SRV
+000015e0: aa02 1353 6572 7669 6365 732e 5275 6e74  ...Services.Runt
+000015f0: 696d 652e 5630 ca02 1353 6572 7669 6365  ime.V0...Service
+00001600: 735c 5275 6e74 696d 655c 5630 e202 1f53  s\Runtime\V0...S
+00001610: 6572 7669 6365 735c 5275 6e74 696d 655c  ervices\Runtime\
+00001620: 5630 5c47 5042 4d65 7461 6461 7461 ea02  V0\GPBMetadata..
+00001630: 1553 6572 7669 6365 733a 3a52 756e 7469  .Services::Runti
+00001640: 6d65 3a3a 5630 6926 0100 005a 0b5f 4c4f  me::V0i&...Z._LO
+00001650: 4144 5354 4154 5553 69b7 0100 0069 8c01  ADSTATUSi....i..
+00001660: 0000 5a12 5f4c 4f41 4453 5441 5455 535f  ..Z._LOADSTATUS_
+00001670: 5354 4154 5553 69ba 0100 005a 0c5f 4c4f  STATUSi....Z._LO
+00001680: 4144 5245 5155 4553 5469 8302 0000 6986  ADREQUESTi....i.
+00001690: 0200 005a 0d5f 4c4f 4144 5245 5350 4f4e  ...Z._LOADRESPON
+000016a0: 5345 692a 0300 0069 2d03 0000 5a0b 5f49  SEi*...i-...Z._I
+000016b0: 4e49 5453 5441 5455 5369 be03 0000 5a12  NITSTATUSi....Z.
+000016c0: 5f49 4e49 5453 5441 5455 535f 5354 4154  _INITSTATUS_STAT
+000016d0: 5553 69c1 0300 005a 0c5f 494e 4954 5245  USi....Z._INITRE
+000016e0: 5155 4553 5469 4605 0000 6949 0500 005a  QUESTiF...iI...Z
+000016f0: 0d5f 494e 4954 5245 5350 4f4e 5345 6965  ._INITRESPONSEie
+00001700: 0600 0069 6806 0000 5a0d 5f53 5441 5254  ...ih...Z._START
+00001710: 5245 5155 4553 5469 f906 0000 69fc 0600  REQUESTi....i...
+00001720: 005a 0c5f 5354 4152 5453 5441 5455 5369  .Z._STARTSTATUSi
+00001730: 9107 0000 6964 0700 005a 135f 5354 4152  ....id...Z._STAR
+00001740: 5453 5441 5455 535f 5354 4154 5553 6993  TSTATUS_STATUSi.
+00001750: 0700 005a 0e5f 5354 4152 5452 4553 504f  ...Z._STARTRESPO
+00001760: 4e53 4569 dc07 0000 69df 0700 005a 0b5f  NSEi....i....Z._
+00001770: 5445 5354 5354 4154 5553 6972 0800 0069  TESTSTATUSir...i
+00001780: 4508 0000 5a12 5f54 4553 5453 5441 5455  E...Z._TESTSTATU
+00001790: 535f 5354 4154 5553 6974 0800 005a 0c5f  S_STATUSit...Z._
+000017a0: 5445 5354 5245 5155 4553 5469 8108 0000  TESTREQUESTi....
+000017b0: 6983 0800 005a 0d5f 5445 5354 5245 5350  i....Z._TESTRESP
+000017c0: 4f4e 5345 69ca 0800 0069 cc08 0000 5a0c  ONSEi....i....Z.
+000017d0: 5f53 544f 5052 4551 5545 5354 69d9 0800  _STOPREQUESTi...
+000017e0: 0069 dc08 0000 5a0b 5f53 544f 5053 5441  .i....Z._STOPSTA
+000017f0: 5455 5369 6f09 0000 5a12 5f53 544f 5053  TUSio...Z._STOPS
+00001800: 5441 5455 535f 5354 4154 5553 6971 0900  TATUS_STATUSiq..
+00001810: 005a 0d5f 5354 4f50 5245 5350 4f4e 5345  .Z._STOPRESPONSE
+00001820: 69b8 0900 0069 ba09 0000 5a0f 5f44 4553  i....i....Z._DES
+00001830: 5452 4f59 5245 5155 4553 5469 ca09 0000  TROYREQUESTi....
+00001840: 69cd 0900 005a 0e5f 4445 5354 524f 5953  i....Z._DESTROYS
+00001850: 5441 5455 5369 660a 0000 5a15 5f44 4553  TATUSif...Z._DES
+00001860: 5452 4f59 5354 4154 5553 5f53 5441 5455  TROYSTATUS_STATU
+00001870: 5369 680a 0000 5a10 5f44 4553 5452 4f59  Sih...Z._DESTROY
+00001880: 5245 5350 4f4e 5345 69b5 0a00 0069 b70a  RESPONSEi....i..
+00001890: 0000 5a13 5f49 4e46 4f52 4d41 5449 4f4e  ..Z._INFORMATION
+000018a0: 5245 5155 4553 5469 cb0a 0000 69ce 0a00  REQUESTi....i...
+000018b0: 005a 0d5f 4445 5349 5245 4453 5441 5445  .Z._DESIREDSTATE
+000018c0: 695a 0b00 0069 1d0b 0000 5a13 5f44 4553  iZ...i....Z._DES
+000018d0: 4952 4544 5354 4154 455f 5354 4147 4569  IREDSTATE_STAGEi
+000018e0: 5d0b 0000 5a14 5f49 4e46 4f52 4d41 5449  ]...Z._INFORMATI
+000018f0: 4f4e 5245 5350 4f4e 5345 6952 0d00 0069  ONRESPONSEiR...i
+00001900: 550d 0000 5a08 5f52 554e 5449 4d45 69fb  U...Z._RUNTIMEi.
+00001910: 0f00 0029 2cda 075f 5f64 6f63 5f5f da0f  ...),..__doc__..
+00001920: 676f 6f67 6c65 2e70 726f 746f 6275 6672  google.protobufr
+00001930: 0200 0000 da0b 5f64 6573 6372 6970 746f  ......_descripto
+00001940: 7272 0300 0000 da10 5f64 6573 6372 6970  rr......_descrip
+00001950: 746f 725f 706f 6f6c 7204 0000 00da 105f  tor_poolr......_
+00001960: 7379 6d62 6f6c 5f64 6174 6162 6173 65da  symbol_database.
+00001970: 1867 6f6f 676c 652e 7072 6f74 6f62 7566  .google.protobuf
+00001980: 2e69 6e74 6572 6e61 6c72 0500 0000 da08  .internalr......
+00001990: 5f62 7569 6c64 6572 da07 4465 6661 756c  _builder..Defaul
+000019a0: 74da 075f 7379 6d5f 6462 da07 6261 7365  t.._sym_db..base
+000019b0: 2e76 3072 0600 0000 da1a 6261 7365 5f64  .v0r......base_d
+000019c0: 6f74 5f76 305f 646f 745f 7363 6f70 655f  ot_v0_dot_scope_
+000019d0: 5f70 6232 7207 0000 005a 1962 6173 655f  _pb2r....Z.base_
+000019e0: 646f 745f 7630 5f64 6f74 5f73 7065 635f  dot_v0_dot_spec_
+000019f0: 5f70 6232 7208 0000 005a 2062 6173 655f  _pb2r....Z base_
+00001a00: 646f 745f 7630 5f64 6f74 5f65 6e76 6972  dot_v0_dot_envir
+00001a10: 6f6e 6d65 6e74 5f5f 7062 3272 0900 0000  onment__pb2r....
+00001a20: da1c 6261 7365 5f64 6f74 5f76 305f 646f  ..base_dot_v0_do
+00001a30: 745f 7365 7276 6963 655f 5f70 6232 720a  t_service__pb2r.
+00001a40: 0000 00da 1d62 6173 655f 646f 745f 7630  .....base_dot_v0
+00001a50: 5f64 6f74 5f65 6e64 706f 696e 745f 5f70  _dot_endpoint__p
+00001a60: 6232 720b 0000 005a 1c62 6173 655f 646f  b2r....Z.base_do
+00001a70: 745f 7630 5f64 6f74 5f6e 6574 776f 726b  t_v0_dot_network
+00001a80: 5f5f 7062 3272 0c00 0000 da22 6261 7365  __pb2r....."base
+00001a90: 5f64 6f74 5f76 305f 646f 745f 636f 6e66  _dot_v0_dot_conf
+00001aa0: 6967 7572 6174 696f 6e5f 5f70 6232 da11  iguration__pb2..
+00001ab0: 7365 7276 6963 6573 2e61 6765 6e74 2e76  services.agent.v
+00001ac0: 3072 0d00 0000 da28 7365 7276 6963 6573  0r.....(services
+00001ad0: 5f64 6f74 5f61 6765 6e74 5f64 6f74 5f76  _dot_agent_dot_v
+00001ae0: 305f 646f 745f 6167 656e 745f 5f70 6232  0_dot_agent__pb2
+00001af0: 720e 0000 005a 2e73 6572 7669 6365 735f  r....Z.services_
+00001b00: 646f 745f 6167 656e 745f 646f 745f 7630  dot_agent_dot_v0
+00001b10: 5f64 6f74 5f63 6f6d 6d75 6e69 6361 7465  _dot_communicate
+00001b20: 5f5f 7062 32da 1141 6464 5365 7269 616c  __pb2..AddSerial
+00001b30: 697a 6564 4669 6c65 720f 0000 00da 0767  izedFiler......g
+00001b40: 6c6f 6261 6c73 da08 5f67 6c6f 6261 6c73  lobals.._globals
+00001b50: da1e 4275 696c 644d 6573 7361 6765 416e  ..BuildMessageAn
+00001b60: 6445 6e75 6d44 6573 6372 6970 746f 7273  dEnumDescriptors
+00001b70: da1e 4275 696c 6454 6f70 4465 7363 7269  ..BuildTopDescri
+00001b80: 7074 6f72 7341 6e64 4d65 7373 6167 6573  ptorsAndMessages
+00001b90: da12 5f55 5345 5f43 5f44 4553 4352 4950  .._USE_C_DESCRIP
+00001ba0: 544f 5253 da0f 5f6c 6f61 6465 645f 6f70  TORS.._loaded_op
+00001bb0: 7469 6f6e 73da 135f 7365 7269 616c 697a  tions.._serializ
+00001bc0: 6564 5f6f 7074 696f 6e73 da11 5f73 6572  ed_options.._ser
+00001bd0: 6961 6c69 7a65 645f 7374 6172 74da 0f5f  ialized_start.._
+00001be0: 7365 7269 616c 697a 6564 5f65 6e64 a900  serialized_end..
+00001bf0: 722a 0000 0072 2a00 0000 fa77 2f55 7365  r*...r*....w/Use
+00001c00: 7273 2f61 6e74 6f69 6e65 2f44 6576 656c  rs/antoine/Devel
+00001c10: 6f70 6d65 6e74 2f63 6f64 6566 6c79 2e64  opment/codefly.d
+00001c20: 6576 2f63 6f72 652f 6765 6e65 7261 7465  ev/core/generate
+00001c30: 642f 7079 7468 6f6e 2f63 6f64 6566 6c79  d/python/codefly
+00001c40: 2d63 6c69 2f63 6f64 6566 6c79 5f63 6c69  -cli/codefly_cli
+00001c50: 2f73 6572 7669 6365 732f 7275 6e74 696d  /services/runtim
+00001c60: 652f 7630 2f72 756e 7469 6d65 5f70 6232  e/v0/runtime_pb2
+00001c70: 2e70 79da 083c 6d6f 6475 6c65 3e01 0000  .py..<module>...
+00001c80: 0073 a200 0000 0404 0c01 0c01 0c01 0c01  .s..............
+00001c90: 0803 0c03 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00001ca0: 0c01 0c01 0e03 0602 0c01 0e01 0801 0a01  ................
+00001cb0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00001cc0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00001cd0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+00001ce0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00001cf0: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00001d00: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
 00001d10: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00001d20: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00001d30: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00001d40: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00001d50: 0a01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
-00001d60: 0a01 0a01 0a01 0e01 04c4                 ..........
+00001d20: 0a01 0a01 0e01 04c4                      ........
```

### Comparing `codefly_cli-0.0.6/codefly_cli/services/runtime/v0/runtime_pb2.py` & `codefly_cli-0.0.7/codefly_cli/services/runtime/v0/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py` & `codefly_cli-0.0.7/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc` & `codefly_cli-0.0.7/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.6/PKG-INFO` & `codefly_cli-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefly-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Antoine Toussaint
 Author-email: antoine.toussaint@codefly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


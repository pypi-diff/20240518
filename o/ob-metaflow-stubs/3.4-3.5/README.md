# Comparing `tmp/ob-metaflow-stubs-3.4.tar.gz` & `tmp/ob-metaflow-stubs-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-3.4.tar", last modified: Fri May 17 19:44:45 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.5.tar", last modified: Fri May 17 23:07:06 2024, max compression
```

## Comparing `ob-metaflow-stubs-3.4.tar` & `ob-metaflow-stubs-3.5.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.560221 ob-metaflow-stubs-3.4/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.564221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.564221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.564221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.568221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.572221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/logs_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/perimeters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.576221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/procpoll.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/metaflow-stubs/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/profilers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-17 19:44:44.000000 ob-metaflow-stubs-3.4/metaflow-stubs/tagging_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 19:44:45.000000 ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:44:45.580221 ob-metaflow-stubs-3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 19:44:28.000000 ob-metaflow-stubs-3.4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.573435 ob-metaflow-stubs-3.5/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.577435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.581435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.581435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.581435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.585435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/logs_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-17 23:07:04.000000 ob-metaflow-stubs-3.5/metaflow-stubs/tagging_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 23:07:06.000000 ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:07:06.589435 ob-metaflow-stubs-3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 23:06:40.000000 ob-metaflow-stubs-3.5/version.py
```

### Comparing `ob-metaflow-stubs-3.4/PKG-INFO` & `ob-metaflow-stubs-3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.4
+Version: 3.5
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.623630                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.406286                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import typing
+    import metaflow.datastore.inputs
+    import metaflow.plugins.datatools.s3.s3
+    import metaflow.events
     import datetime
+    import metaflow._vendor.click.types
+    import metaflow.client.core
     import io
-    import metaflow.events
     import metaflow.parameters
-    import typing
     import metaflow.metaflow_current
-    import metaflow.client.core
-    import metaflow._vendor.click.types
-    import metaflow.plugins.datatools.s3.s3
-    import metaflow.datastore.inputs
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,203 +722,59 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the Conda environment for the step.
+    Specifies the PyPI packages for the step.
     
     Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
+    packages : Dict[str, str], default: {}
         Packages to use for this step. The key is the name of the package
         and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
+    python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies the Conda environment for the step.
+    Specifies the PyPI packages for the step.
     
     Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    packages : Dict[str, str], default {}
+    packages : Dict[str, str], default: {}
         Packages to use for this step. The key is the name of the package
         and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
+    python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
-    """
-    ...
-
-def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies that this step should execute on Kubernetes.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    disk : int, default 10240
-        Disk size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on Kubernetes. If not specified, and
-        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
-        If given, the imagePullPolicy to be applied to the Docker image of the step.
-    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
-        Kubernetes service account to use when launching pod in Kubernetes.
-    secrets : List[str], optional, default None
-        Kubernetes secrets to use when launching pod in Kubernetes. These
-        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
-        in Metaflow configuration.
-    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
-        Kubernetes namespace to use when launching pod in Kubernetes.
-    gpu : int, optional, default None
-        Number of GPUs required for this step. A value of zero implies that
-        the scheduled node should not have GPUs.
-    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
-        The vendor of the GPUs to be used for this step.
-    tolerations : List[str], default []
-        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
-        Kubernetes tolerations to use when launching pod in Kubernetes.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step.
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default: None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default /metaflow_temp
-        Path to tmpfs mount for this step.
-    persistent_volume_claims : Dict[str, str], optional, default None
-        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
-        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
-    shared_memory: int, optional
-        Shared memory size (in MiB) required for this step
-    port: int, optional
-        Port number to specify in the Kubernetes job object
-    """
-    ...
-
-@typing.overload
-def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
-    
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    """
-    ...
-
-@typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
-    """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
-    
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
@@ -1061,14 +917,130 @@
     log_options: List[str], optional, default None
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
+def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies that this step should execute on Kubernetes.
+    
+    Parameters
+    ----------
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    disk : int, default 10240
+        Disk size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on Kubernetes. If not specified, and
+        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
+        If given, the imagePullPolicy to be applied to the Docker image of the step.
+    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
+        Kubernetes service account to use when launching pod in Kubernetes.
+    secrets : List[str], optional, default None
+        Kubernetes secrets to use when launching pod in Kubernetes. These
+        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
+        in Metaflow configuration.
+    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
+        Kubernetes namespace to use when launching pod in Kubernetes.
+    gpu : int, optional, default None
+        Number of GPUs required for this step. A value of zero implies that
+        the scheduled node should not have GPUs.
+    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
+        The vendor of the GPUs to be used for this step.
+    tolerations : List[str], default []
+        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
+        Kubernetes tolerations to use when launching pod in Kubernetes.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default: None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default /metaflow_temp
+        Path to tmpfs mount for this step.
+    persistent_volume_claims : Dict[str, str], optional, default None
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
+    shared_memory: int, optional
+        Shared memory size (in MiB) required for this step
+    port: int, optional
+        Port number to specify in the Kubernetes job object
+    """
+    ...
+
+@typing.overload
+def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies the Conda environment for the step.
+    
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
+    """
+    ...
+
+@typing.overload
+def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+    """
+    Specifies the Conda environment for the step.
+    
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
+    """
+    ...
+
 @typing.overload
 def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that the step will success under all circumstances.
     
     The decorator will create an optional artifact, specified by `var`, which
     contains the exception raised. You can use it to detect the presence
@@ -1111,94 +1083,67 @@
     print_exception : bool, default True
         Determines whether or not the exception is printed to
         stdout when caught.
     """
     ...
 
 @typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies environment variables to be set prior to the execution of a step.
-    
-    Parameters
-    ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
-    """
-    ...
-
-@typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies a timeout for your step.
     
-    Parameters
-    ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
-    """
-    ...
-
-@typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
+    This decorator is useful if this step may hang indefinitely.
     
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
+    Specifies a timeout for your step.
     
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    This decorator is useful if this step may hang indefinitely.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
 def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Creates a human-readable report, a Metaflow Card, after this step completes.
@@ -1246,116 +1191,140 @@
         Interrupt reporting if it takes more than this many seconds.
     
     
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
+    Specifies the resources needed when executing this step.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
+    Specifies the resources needed when executing this step.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the PyPI packages for the step.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
     """
-    Specifies the PyPI packages for the step.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
 def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies secrets to be retrieved and injected as environment variables prior to
@@ -1385,14 +1354,45 @@
     ----------
     sources : List[Union[str, Dict[str, Any]]], default: []
         List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies environment variables to be set prior to the execution of a step.
+    
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+    """
+    Specifies environment variables to be set prior to the execution of a step.
+    
+    Parameters
+    ----------
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
+    """
+    ...
+
+@typing.overload
 def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the PyPI packages for all steps of the flow.
     
     Use `@pypi_base` to set common packages required by all
     steps and use `@pypi` to specify step-specific overrides.
     Parameters
@@ -1423,135 +1423,193 @@
         and the value is the version to use.
     python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
+    """
+    ...
+
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    """
+    ...
+
 @typing.overload
-def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies the flow(s) that this flow depends on.
+    Specifies the event(s) that this flow depends on.
     
     ```
-    @trigger_on_finish(flow='FooFlow')
+    @trigger(event='foo')
     ```
     or
     ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    @trigger(events=['foo', 'bar'])
     ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
     
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
+    Additionally, you can specify the parameter mappings
+    to map event payload to Metaflow parameters for the flow.
     ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
     ```
     or
     ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
     ```
     
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
+    'parameters' can also be a list of strings and tuples like so:
     ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
     ```
-    
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
     
     Parameters
     ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
+    event : Union[str, Dict[str, Any]], optional, default None
+        Event dependency for this flow.
+    events : List[Union[str, Dict[str, Any]]], default []
+        Events dependency for this flow.
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
 @typing.overload
-def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+def trigger(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
+def trigger(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}):
     """
-    Specifies the flow(s) that this flow depends on.
+    Specifies the event(s) that this flow depends on.
     
     ```
-    @trigger_on_finish(flow='FooFlow')
+    @trigger(event='foo')
     ```
     or
     ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    @trigger(events=['foo', 'bar'])
     ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
     
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
+    Additionally, you can specify the parameter mappings
+    to map event payload to Metaflow parameters for the flow.
     ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
     ```
     or
     ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
+                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
     ```
     
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
+    'parameters' can also be a list of strings and tuples like so:
     ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
+    ```
+    This is equivalent to:
+    ```
+    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
     ```
-    
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
     
     Parameters
     ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
+    event : Union[str, Dict[str, Any]], optional, default None
+        Event dependency for this flow.
+    events : List[Union[str, Dict[str, Any]]], default []
+        Events dependency for this flow.
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
-def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies what flows belong to the same project.
-    
-    A project-specific namespace is created for all flows that
-    use the same `@project(name)`.
-    
-    Parameters
-    ----------
-    name : str
-        Project name. Make sure that the name is unique amongst all
-        projects that use the same production scheduler. The name may
-        contain only lowercase alphanumeric characters and underscores.
-    
-    
-    """
-    ...
-
 @typing.overload
 def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the Conda environment for all steps of the flow.
     
     Use `@conda_base` to set common libraries required by all
     steps and use `@conda` to specify step-specific additions.
@@ -1593,104 +1651,27 @@
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables Conda.
     """
     ...
 
-@typing.overload
-def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the event(s) that this flow depends on.
-    
-    ```
-    @trigger(event='foo')
-    ```
-    or
-    ```
-    @trigger(events=['foo', 'bar'])
-    ```
-    
-    Additionally, you can specify the parameter mappings
-    to map event payload to Metaflow parameters for the flow.
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
-    ```
-    or
-    ```
-    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
-    ```
-    
-    'parameters' can also be a list of strings and tuples like so:
-    ```
-    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
-    ```
-    This is equivalent to:
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
-    ```
-    
-    Parameters
-    ----------
-    event : Union[str, Dict[str, Any]], optional, default None
-        Event dependency for this flow.
-    events : List[Union[str, Dict[str, Any]]], default []
-        Events dependency for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
-@typing.overload
-def trigger(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def trigger(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}):
+def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies the event(s) that this flow depends on.
-    
-    ```
-    @trigger(event='foo')
-    ```
-    or
-    ```
-    @trigger(events=['foo', 'bar'])
-    ```
-    
-    Additionally, you can specify the parameter mappings
-    to map event payload to Metaflow parameters for the flow.
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'flow_param': 'event_field'}})
-    ```
-    or
-    ```
-    @trigger(events=[{'name':'foo', 'parameters':{'flow_param_1': 'event_field_1'},
-                     {'name':'bar', 'parameters':{'flow_param_2': 'event_field_2'}])
-    ```
+    Specifies what flows belong to the same project.
     
-    'parameters' can also be a list of strings and tuples like so:
-    ```
-    @trigger(event={'name':'foo', 'parameters':['common_name', ('flow_param', 'event_field')]})
-    ```
-    This is equivalent to:
-    ```
-    @trigger(event={'name':'foo', 'parameters':{'common_name': 'common_name', 'flow_param': 'event_field'}})
-    ```
+    A project-specific namespace is created for all flows that
+    use the same `@project(name)`.
     
     Parameters
     ----------
-    event : Union[str, Dict[str, Any]], optional, default None
-        Event dependency for this flow.
-    events : List[Union[str, Dict[str, Any]]], default []
-        Events dependency for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
+    name : str
+        Project name. Make sure that the name is unique amongst all
+        projects that use the same production scheduler. The name may
+        contain only lowercase alphanumeric characters and underscores.
     
     
     """
     ...
 
 @typing.overload
 def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
@@ -1737,95 +1718,114 @@
         specified by this expression.
     timezone : str, optional, default None
         Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
         which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+@typing.overload
+def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
     
     Parameters
     ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
     """
     ...
 
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+@typing.overload
+def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
     """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
     
     Parameters
     ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
     """
     ...
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/cards.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.643816                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.426484                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
     import typing
-    import metaflow.plugins.cards.card_modules.card
-    import metaflow.plugins.cards.card_modules.components
-    import metaflow
     import metaflow.plugins.cards.card_client
+    import metaflow
+    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.card
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/cli.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.648874                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.431329                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.646582                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.428982                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import datetime
-    import metaflow.client.core
     import metaflow.events
+    import metaflow.client.core
+    import datetime
     import typing
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.632810                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.415443                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import typing
     import tarfile
-    import metaflow.events
     import metaflow.exception
-    import typing
-    import metaflow.metaflow_current
-    import metaflow.client.core
-    import datetime
     import metaflow
+    import metaflow.events
+    import datetime
+    import metaflow.client.core
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/client/filecache.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.649759                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.432173                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.datastore.content_addressed_store
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/clone_util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.647139                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.429538                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/events.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.634704                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.417317                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.events
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/exception.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.625479                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.408075                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/flowspec.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.634133                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.416745                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
-    import metaflow.parameters
     import typing
-    import metaflow.exception
     import metaflow.datastore.inputs
+    import metaflow.exception
+    import metaflow.unbounded_foreach
+    import metaflow.parameters
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.642120                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.424730                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
-    import metaflow.parameters
     import typing
-    import metaflow._vendor.click.types
     import metaflow.plugins.datatools.s3.s3
+    import metaflow._vendor.click.types
+    import io
+    import metaflow.parameters
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/metadata/metadata.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.670701                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.450367                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.metadata.metadata
+    import metaflow.exception
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowTaggingError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/metadata/util.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.701876                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.492339                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_config.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.626459                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.409083                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/metaflow_current.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.715308                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.494647                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import typing
+    import metaflow
+    import metaflow.events
     import metaflow.plugins.cards.component_serializer
     import metaflow.metaflow_current
-    import metaflow
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -240,15 +240,15 @@
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
     def trigger(self) -> "metaflow.events.Trigger":
         """
-        (only in the presence of the @trigger_on_finish, or @trigger decorators)
+        (only in the presence of the @trigger, or @trigger_on_finish decorators)
         
         Returns `Trigger` if the current run is triggered by an event
         
         Returns
         -------
         Trigger
             `Trigger` if triggered by an event
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/mflog/mflog.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/mflog/mflog.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.671013                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.450679                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/multicore_utils.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.626879                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.409498                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/parameters.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.627936                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.410594                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import typing
     import metaflow.parameters
-    import metaflow._vendor.click.types
     import metaflow.exception
-    import typing
+    import metaflow._vendor.click.types
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.636187                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.418834                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow.unbounded_foreach
+    import metaflow.plugins.cards.card_modules.card
 
 CLIS_DESC: list
 
 class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
     def __init__(self, iterable):
         ...
     def __iter__(self):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.681992                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.454060                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.metaflow_current
     import metaflow._vendor.click.types
-    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.682927                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.455472                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.680096                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.452012                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.679724                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.451642                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.680320                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.452232                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.680552                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.452451                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.711398                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.482092                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
 class AirflowTask(object, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.711782                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.482473                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.712261                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.482812                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.691761                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.471450                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.690461                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.470142                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.695820                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.475477                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
+    import metaflow.exception
     import metaflow.parameters
+    import metaflow.metaflow_current
     import metaflow._vendor.click.types
-    import metaflow.exception
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.697365                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.476966                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.parameters
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
+    import metaflow.parameters
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.691205                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.470895                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.events
-    import metaflow
     import metaflow.decorators
+    import metaflow
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.646882                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.429283                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.676265                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.456054                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.704014                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.490116                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.705349                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.491394                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.703038                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.489097                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.704725                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.490817                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.710576                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.491786                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
+    import abc
     import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.705577                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.483597                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.706759                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.484424                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.706174                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.484156                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.708932                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.486752                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.710171                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.487959                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.parameters
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
+    import metaflow.parameters
+    import metaflow.metaflow_current
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.707073                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.484731                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 AWS_SANDBOX_ENABLED: bool
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.706003                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.483986                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.698509                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.478498                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.698729                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.478712                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.699883                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.479877                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
+    import abc
     import metaflow.exception
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.699129                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.479111                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.699459                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.479450                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.665638                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.445315                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.690045                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.469694                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.parameters
     import typing
-    import metaflow.client.core
-    import datetime
     import metaflow.exception
+    import datetime
+    import metaflow.client.core
+    import metaflow.parameters
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.667182                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.446900                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow
+    import metaflow.exception
     import metaflow.plugins.cards.card_client
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.685990                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.465629                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.687424                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.467172                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.686683                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.466447                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class CardComponentCollector(object, metaclass=type):
     def __init__(self, logger = None, card_creator = None):
         ...
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.683748                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.463562                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.660268                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.441045                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
-    import metaflow
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow
+    import metaflow.plugins.cards.card_modules.card
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.667596                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.447294                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.712745                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.483134                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.714161                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.493476                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.713771                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.493096                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.713388                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.492728                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.669521                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.449158                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.components
-    import metaflow.plugins.cards.card_modules.card
     import typing
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.card
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.701397                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.481344                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.701585                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.480288                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.exception
 
-class SerializationErrorComponent(metaflow.plugins.cards.card_modules.basic.ErrorComponent, metaclass=type):
-    def __init__(self, component_name, error_message):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
         ...
     ...
 
-def render_safely(func):
-    """
-    This is a decorator that can be added to any `MetaflowCardComponent.render`
-    The goal is to render subcomponents safely and ensure that they are JSON serializable.
-    """
+class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.661463                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.442223                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow
+    import metaflow.plugins.cards.card_modules.card
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.687908                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.467650                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.685742                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.465382                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
-    import metaflow.plugins.cards.card_modules.card
     import metaflow.exception
-    import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.card
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
     def component_id(self, value):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.684301                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.464122                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.653136                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.435882                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.652616                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.435119                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.datatools.s3.s3
-    import metaflow.exception
     import io
+    import metaflow.exception
+    import metaflow.plugins.datatools.s3.s3
 
 def read_in_chunks(dst, src, src_sz, max_chunk_size):
     ...
 
 class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.665107                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.444844                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.678723                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.460482                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.datatools.s3.s3
     import metaflow.exception
     import io
+    import metaflow.plugins.datatools.s3.s3
 
 class RangeInfo(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, total_size: int, request_offset: int = 0, request_length: int = -1):
         """
         Create new instance of RangeInfo(total_size, request_offset, request_length)
         """
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.639354                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.422024                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
     import typing
-    import metaflow.metaflow_current
-    import metaflow.plugins.datatools.s3.s3
-    import metaflow.exception
     import metaflow.datastore.inputs
+    import metaflow.exception
+    import metaflow.plugins.datatools.s3.s3
+    import io
+    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.710910                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.492112                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.664387                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.444331                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_logger.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.657172                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.438347                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.event_logger
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.657613                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.438574                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.653442                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.436844                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.655291                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.436472                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
 
-current: metaflow.metaflow_current.Current
-
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
-    ...
+MAX_ATTEMPTS: int
 
-class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
-    def get_top_level_options(self):
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.683300                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.477348                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.plugins.parallel_decorator
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.701015                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.480991                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
+    import abc
     import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.700303                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.433428                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+MAGIC_FILE: str
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.700590                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.480570                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.666107                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.445848                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.674222                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.461401                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.675921                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.463091                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow._vendor.click.types
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
+    import metaflow._vendor.click.types
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.624217                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.406863                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.675117                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.462311                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/logs_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/logs_cli.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.663746                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.442639                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow._vendor.click.core
-    import metaflow.exception
     import metaflow.plugins.logs_cli
+    import metaflow.exception
 
 LOGGER_TIMESTAMP: str
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 LOG_SOURCES: list
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.650587                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.432988                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/perimeters.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/perimeters.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.624515                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.407159                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.655839                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.437478                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.650793                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.430285                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAGIC_FILE: str
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
+        ...
+    def run(self, logger = None, warnings = False, pylint_config = []):
+        ...
+    ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.671582                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.456935                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.672889                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.458135                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
+    import io
     import metaflow.metaflow_environment
     import metaflow.exception
-    import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.671823                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.456403                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.673326                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.458525                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.pypi.conda_environment
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.672115                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.457227                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/resources_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.651005                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.433559                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.654744                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.436685                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.698288                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.478286                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
+    import abc
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.698043                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.478049                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/storage_executor.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.656529                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.437970                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.662773                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.443780                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.events
+    import datetime
     import metaflow.client.core
     import metaflow.metaflow_current
-    import datetime
-    import metaflow.exception
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.650258                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.432659                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
     import metaflow.decorators
+    import metaflow.unbounded_foreach
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.651369                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.433982                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/procpoll.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.647545                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.429992                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/profilers/__init__.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/profilers/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.624745                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.407392                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class gpu_profile(object, metaclass=type):
     def __init__(self, include_artifacts = True, artifact_prefix = "gpu_profile_", interval = 1):
```

### Comparing `ob-metaflow-stubs-3.4/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.5/metaflow-stubs/tagging_util.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.15.2+ob(v1)                                                   #
-# Generated on 2024-05-17T19:44:44.628239                                        #
+# MF version: 2.11.15.3+ob(v1)                                                   #
+# Generated on 2024-05-17T23:07:04.410906                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.4
+Version: 3.5
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.4/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.5/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-stubs-3.4/setup.py` & `ob-metaflow-stubs-3.5/setup.py`

 * *Files identical despite different names*


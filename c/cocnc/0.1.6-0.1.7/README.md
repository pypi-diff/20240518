# Comparing `tmp/cocnc-0.1.6.tar.gz` & `tmp/cocnc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocnc-0.1.6.tar", max compression
+gzip compressed data, was "cocnc-0.1.7.tar", max compression
```

## Comparing `cocnc-0.1.6.tar` & `cocnc-0.1.7.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0    35148 2024-05-17 15:26:32.121952 cocnc-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     5336 2024-05-17 15:26:32.121952 cocnc-0.1.6/README.md
--rw-r--r--   0        0        0      945 2024-05-17 15:26:32.121952 cocnc-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      199 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/__init__.py
--rw-r--r--   0        0        0      498 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/check_dependencies.py
--rw-r--r--   0        0        0        0 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/commands/__init__.py
--rw-r--r--   0        0        0     1590 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/commands/build.py
--rw-r--r--   0        0        0     1545 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/commands/deploy.py
--rw-r--r--   0        0        0     2409 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/commands/info.py
--rw-r--r--   0        0        0     4136 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/commands/provision.py
--rw-r--r--   0        0        0      753 2024-05-17 15:26:32.121952 cocnc-0.1.6/src/cnc/commands/render.py
--rw-r--r--   0        0        0      663 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/commands/shell.py
--rw-r--r--   0        0        0     1079 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/commands/telemetry.py
--rw-r--r--   0        0        0        0 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/commands/template_editor/__init__.py
--rw-r--r--   0        0        0     5650 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/commands/template_editor/inspector.py
--rw-r--r--   0        0        0     2956 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/commands/toolbox.py
--rw-r--r--   0        0        0     1807 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/commands/update.py
--rw-r--r--   0        0        0      739 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/constants.py
--rw-r--r--   0        0        0     3780 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2
--rw-r--r--   0        0        0      689 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/build/main.sh.j2
--rw-r--r--   0        0        0       43 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0     2427 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2
--rw-r--r--   0        0        0     1257 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     1623 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2
--rw-r--r--   0        0        0     2468 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2
--rw-r--r--   0        0        0      766 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2
--rw-r--r--   0        0        0      645 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2
--rw-r--r--   0        0        0      200 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy.sh.j2
--rw-r--r--   0        0        0     1047 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2
--rw-r--r--   0        0        0     1478 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2
--rw-r--r--   0        0        0      396 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/frontend_routing_lambda/index.js
--rw-r--r--   0        0        0      561 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2
--rw-r--r--   0        0        0     4651 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2
--rw-r--r--   0        0        0     5481 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2
--rw-r--r--   0        0        0     5640 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2
--rw-r--r--   0        0        0     1759 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2
--rw-r--r--   0        0        0    11529 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2
--rw-r--r--   0        0        0      813 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2
--rw-r--r--   0        0        0     8800 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2
--rw-r--r--   0        0        0     1888 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2
--rw-r--r--   0        0        0     1432 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2
--rw-r--r--   0        0        0     1886 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2
--rw-r--r--   0        0        0    26090 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2
--rw-r--r--   0        0        0     9699 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2
--rw-r--r--   0        0        0     6430 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2
--rw-r--r--   0        0        0     2382 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2
--rw-r--r--   0        0        0     5446 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2
--rw-r--r--   0        0        0      965 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2
--rw-r--r--   0        0        0    11326 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2
--rw-r--r--   0        0        0      336 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/shared/toolbox/Dockerfile.j2
--rw-r--r--   0        0        0     4184 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/aws/shared/toolbox/main.sh.j2
--rw-r--r--   0        0        0      615 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2
--rw-r--r--   0        0        0      290 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0     1953 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2
--rw-r--r--   0        0        0     1189 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2
--rw-r--r--   0        0        0     4347 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2
--rw-r--r--   0        0        0      299 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/build/main.sh.j2
--rw-r--r--   0        0        0      104 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/cnc-flavor.yml
--rw-r--r--   0        0        0      661 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2
--rw-r--r--   0        0        0       43 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0      303 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     2512 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run/1/provision/main.tf.j2
--rw-r--r--   0        0        0      299 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/build/main.sh.j2
--rw-r--r--   0        0        0      493 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/deploy/base.sh.j2
--rw-r--r--   0        0        0      331 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0      303 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     1778 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2
--rw-r--r--   0        0        0     1364 2024-05-17 15:26:32.125952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2
--rw-r--r--   0        0        0     1926 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2
--rw-r--r--   0        0        0      273 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/Dockerfile.run.j2
--rw-r--r--   0        0        0     1017 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/base.sh.j2
--rw-r--r--   0        0        0     4542 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2
--rw-r--r--   0        0        0     3555 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/nginx.conf.j2
--rw-r--r--   0        0        0       59 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/all-access-policy.yml.j2
--rw-r--r--   0        0        0     4572 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2
--rw-r--r--   0        0        0     2241 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml
--rw-r--r--   0        0        0      828 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml
--rw-r--r--   0        0        0     1391 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml
--rw-r--r--   0        0        0     2083 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2
--rw-r--r--   0        0        0      165 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/run-job.yml.j2
--rw-r--r--   0        0        0      278 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/run-svc.yml.j2
--rw-r--r--   0        0        0     1496 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2
--rw-r--r--   0        0        0     3790 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2
--rw-r--r--   0        0        0     2503 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2
--rw-r--r--   0        0        0     3338 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2
--rw-r--r--   0        0        0      794 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2
--rw-r--r--   0        0        0     8353 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2
--rw-r--r--   0        0        0     3584 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2
--rw-r--r--   0        0        0     1332 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2
--rw-r--r--   0        0        0      463 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/environment/resource_managed_secrets.tf.j2
--rw-r--r--   0        0        0     1142 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2
--rw-r--r--   0        0        0     1342 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2
--rw-r--r--   0        0        0     1755 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2
--rw-r--r--   0        0        0      332 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/toolbox/Dockerfile.j2
--rw-r--r--   0        0        0     4484 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2
--rw-r--r--   0        0        0      912 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/logger.py
--rw-r--r--   0        0        0     2120 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/main.py
--rw-r--r--   0        0        0      426 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/__init__.py
--rw-r--r--   0        0        0     4488 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/application.py
--rw-r--r--   0        0        0      906 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/base_model.py
--rw-r--r--   0        0        0     3088 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/builder.py
--rw-r--r--   0        0        0       30 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/__init__.py
--rw-r--r--   0        0        0     7925 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/config.py
--rw-r--r--   0        0        0      355 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/deploy_resource_limits.py
--rw-r--r--   0        0        0    17833 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/resource.py
--rw-r--r--   0        0        0    11842 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/service.py
--rw-r--r--   0        0        0    10437 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/settings.py
--rw-r--r--   0        0        0      119 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/config/utils.py
--rw-r--r--   0        0        0      257 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/custom_header.py
--rw-r--r--   0        0        0     8616 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/cycle_stage_base.py
--rw-r--r--   0        0        0     3692 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/deployer.py
--rw-r--r--   0        0        0     8062 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/environment.py
--rw-r--r--   0        0        0    10653 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/environment_collection.py
--rw-r--r--   0        0        0     3646 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/environment_variable.py
--rw-r--r--   0        0        0        0 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/__init__.py
--rw-r--r--   0        0        0      288 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/__init__.py
--rw-r--r--   0        0        0      485 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/cache_resource_settings.py
--rw-r--r--   0        0        0     7166 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/custom_headers.py
--rw-r--r--   0        0        0     3187 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/database_resource_settings.py
--rw-r--r--   0        0        0     3377 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/deploy_resource_limits.py
--rw-r--r--   0        0        0     5530 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/environment_collection.py
--rw-r--r--   0        0        0      168 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/amazon/service_account.py
--rw-r--r--   0        0        0      190 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/google/__init__.py
--rw-r--r--   0        0        0      756 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/google/cache_resource_settings.py
--rw-r--r--   0        0        0     2074 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/google/database_resource_settings.py
--rw-r--r--   0        0        0     2837 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/google/deploy_resource_limits.py
--rw-r--r--   0        0        0     9942 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/google/environment_collection.py
--rw-r--r--   0        0        0        0 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/providers/google/service_account.py
--rw-r--r--   0        0        0    14435 2024-05-17 15:26:32.129952 cocnc-0.1.6/src/cnc/models/provisioner.py
--rw-r--r--   0        0        0      802 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/models/resource_use_existing.py
--rw-r--r--   0        0        0      779 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/models/stage.py
--rw-r--r--   0        0        0     4279 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/models/toolbox.py
--rw-r--r--   0        0        0        0 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/__init__.py
--rw-r--r--   0        0        0     1071 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/base_test_class.py
--rw-r--r--   0        0        0       75 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service/cnc.yml
--rw-r--r--   0        0        0      153 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db/cnc.yml
--rw-r--r--   0        0        0      609 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml
--rw-r--r--   0        0        0      673 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml
--rw-r--r--   0        0        0      153 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/cnc.yml
--rw-r--r--   0        0        0      472 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/environments.yml
--rw-r--r--   0        0        0      153 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/cnc.yml
--rw-r--r--   0        0        0      379 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/environments.yml
--rw-r--r--   0        0        0      153 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/cnc.yml
--rw-r--r--   0        0        0      564 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml
--rw-r--r--   0        0        0      231 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-2-db/cnc.yml
--rw-r--r--   0        0        0      231 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/cnc.yml
--rw-r--r--   0        0        0      373 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments.yml
--rw-r--r--   0        0        0      479 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_aws_ecs.yml
--rw-r--r--   0        0        0      392 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_gcp_run_region_settings.yml
--rw-r--r--   0        0        0       75 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-custom/cnc.yml
--rw-r--r--   0        0        0       22 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-custom/custom/deploy/main.sh.j2
--rw-r--r--   0        0        0      341 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-custom/environments.yml
--rw-r--r--   0        0        0      228 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-2-service-1-db/cnc.yml
--rw-r--r--   0        0        0      322 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/backend-2-service-2-db/cnc.yml
--rw-r--r--   0        0        0      153 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/shared/cnc.yml
--rw-r--r--   0        0        0      340 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/shared/environments-custom-provision.yml
--rw-r--r--   0        0        0      294 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/shared/environments.yml
--rw-r--r--   0        0        0      400 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/shared/environments_aws_ecs.yml
--rw-r--r--   0        0        0      474 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/shared/environments_aws_ecs_existing_vpc.yml
--rw-r--r--   0        0        0      299 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/fixtures/shared/environments_gcp_run_lite.yml
--rw-r--r--   0        0        0     5373 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_builder.py
--rw-r--r--   0        0        0     2683 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_deployer.py
--rw-r--r--   0        0        0     2445 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_environment_collection.py
--rw-r--r--   0        0        0     2287 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_environment_variables.py
--rw-r--r--   0        0        0     1872 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_environments.py
--rw-r--r--   0        0        0    13574 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_provisioner.py
--rw-r--r--   0        0        0     2898 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_services.py
--rw-r--r--   0        0        0     2224 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/tests/test_toolbox.py
--rw-r--r--   0        0        0       38 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-05-17 15:26:32.133952 cocnc-0.1.6/src/cnc/utils/string.py
--rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 cocnc-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-18 00:09:14.603470 cocnc-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     5336 2024-05-18 00:09:14.603470 cocnc-0.1.7/README.md
+-rw-r--r--   0        0        0      945 2024-05-18 00:09:14.607470 cocnc-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/__init__.py
+-rw-r--r--   0        0        0      701 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/check_dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/__init__.py
+-rw-r--r--   0        0        0     1590 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/build.py
+-rw-r--r--   0        0        0     1545 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/deploy.py
+-rw-r--r--   0        0        0     2409 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/info.py
+-rw-r--r--   0        0        0     4136 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/provision.py
+-rw-r--r--   0        0        0      753 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/render.py
+-rw-r--r--   0        0        0      663 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/shell.py
+-rw-r--r--   0        0        0     1079 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/telemetry.py
+-rw-r--r--   0        0        0        0 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/template_editor/__init__.py
+-rw-r--r--   0        0        0     5650 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/template_editor/inspector.py
+-rw-r--r--   0        0        0     2949 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/toolbox.py
+-rw-r--r--   0        0        0     1807 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/commands/update.py
+-rw-r--r--   0        0        0      739 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/constants.py
+-rw-r--r--   0        0        0     3780 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2
+-rw-r--r--   0        0        0      689 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/build/main.sh.j2
+-rw-r--r--   0        0        0       43 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0     2427 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2
+-rw-r--r--   0        0        0     1257 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     1623 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2
+-rw-r--r--   0        0        0     2468 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2
+-rw-r--r--   0        0        0      766 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2
+-rw-r--r--   0        0        0      645 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2
+-rw-r--r--   0        0        0      200 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy.sh.j2
+-rw-r--r--   0        0        0     1047 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2
+-rw-r--r--   0        0        0     1478 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      396 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/frontend_routing_lambda/index.js
+-rw-r--r--   0        0        0      561 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     4651 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2
+-rw-r--r--   0        0        0     5481 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2
+-rw-r--r--   0        0        0     5640 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2
+-rw-r--r--   0        0        0     1759 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2
+-rw-r--r--   0        0        0    11529 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2
+-rw-r--r--   0        0        0      813 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2
+-rw-r--r--   0        0        0     8800 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2
+-rw-r--r--   0        0        0     1888 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2
+-rw-r--r--   0        0        0     1432 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2
+-rw-r--r--   0        0        0     1886 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2
+-rw-r--r--   0        0        0    26090 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2
+-rw-r--r--   0        0        0     9699 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2
+-rw-r--r--   0        0        0     6430 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2
+-rw-r--r--   0        0        0     2382 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2
+-rw-r--r--   0        0        0     5446 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2
+-rw-r--r--   0        0        0      965 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2
+-rw-r--r--   0        0        0    11326 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2
+-rw-r--r--   0        0        0      336 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/shared/toolbox/Dockerfile.j2
+-rw-r--r--   0        0        0     4184 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/aws/shared/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      615 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2
+-rw-r--r--   0        0        0      290 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0     1953 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     1189 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2
+-rw-r--r--   0        0        0     4347 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2
+-rw-r--r--   0        0        0      299 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/build/main.sh.j2
+-rw-r--r--   0        0        0      104 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/cnc-flavor.yml
+-rw-r--r--   0        0        0      661 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2
+-rw-r--r--   0        0        0       43 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0      303 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     2512 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run/1/provision/main.tf.j2
+-rw-r--r--   0        0        0      299 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/build/main.sh.j2
+-rw-r--r--   0        0        0      493 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/deploy/base.sh.j2
+-rw-r--r--   0        0        0      331 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0      303 2024-05-18 00:09:14.607470 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     1778 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2
+-rw-r--r--   0        0        0     1364 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     1926 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      273 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/Dockerfile.run.j2
+-rw-r--r--   0        0        0     1017 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/base.sh.j2
+-rw-r--r--   0        0        0     4542 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2
+-rw-r--r--   0        0        0     3555 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/nginx.conf.j2
+-rw-r--r--   0        0        0       59 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/all-access-policy.yml.j2
+-rw-r--r--   0        0        0     4572 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2
+-rw-r--r--   0        0        0     2241 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml
+-rw-r--r--   0        0        0      828 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml
+-rw-r--r--   0        0        0     1391 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml
+-rw-r--r--   0        0        0     2083 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2
+-rw-r--r--   0        0        0      165 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/run-job.yml.j2
+-rw-r--r--   0        0        0      278 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/run-svc.yml.j2
+-rw-r--r--   0        0        0     1496 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2
+-rw-r--r--   0        0        0     3790 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2
+-rw-r--r--   0        0        0     2503 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2
+-rw-r--r--   0        0        0     3338 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2
+-rw-r--r--   0        0        0      794 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2
+-rw-r--r--   0        0        0     8353 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2
+-rw-r--r--   0        0        0     3584 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2
+-rw-r--r--   0        0        0     1332 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2
+-rw-r--r--   0        0        0      463 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/environment/resource_managed_secrets.tf.j2
+-rw-r--r--   0        0        0     1142 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2
+-rw-r--r--   0        0        0     1342 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2
+-rw-r--r--   0        0        0     1755 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2
+-rw-r--r--   0        0        0      332 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/toolbox/Dockerfile.j2
+-rw-r--r--   0        0        0     4484 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      912 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/logger.py
+-rw-r--r--   0        0        0     2131 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/main.py
+-rw-r--r--   0        0        0      426 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/__init__.py
+-rw-r--r--   0        0        0     4505 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/application.py
+-rw-r--r--   0        0        0      906 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/base_model.py
+-rw-r--r--   0        0        0     3088 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/builder.py
+-rw-r--r--   0        0        0       30 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/__init__.py
+-rw-r--r--   0        0        0     7925 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/config.py
+-rw-r--r--   0        0        0      355 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/deploy_resource_limits.py
+-rw-r--r--   0        0        0    17969 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/resource.py
+-rw-r--r--   0        0        0    11842 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/service.py
+-rw-r--r--   0        0        0    10437 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/settings.py
+-rw-r--r--   0        0        0      119 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/config/utils.py
+-rw-r--r--   0        0        0      257 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/custom_header.py
+-rw-r--r--   0        0        0     8616 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/cycle_stage_base.py
+-rw-r--r--   0        0        0     3692 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/deployer.py
+-rw-r--r--   0        0        0     8062 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/environment.py
+-rw-r--r--   0        0        0    10653 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/environment_collection.py
+-rw-r--r--   0        0        0     3646 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/environment_variable.py
+-rw-r--r--   0        0        0        0 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/__init__.py
+-rw-r--r--   0        0        0      485 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/cache_resource_settings.py
+-rw-r--r--   0        0        0     7166 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/custom_headers.py
+-rw-r--r--   0        0        0     3187 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/database_resource_settings.py
+-rw-r--r--   0        0        0     3377 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/deploy_resource_limits.py
+-rw-r--r--   0        0        0     5530 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/environment_collection.py
+-rw-r--r--   0        0        0      168 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/amazon/service_account.py
+-rw-r--r--   0        0        0      190 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/google/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/google/cache_resource_settings.py
+-rw-r--r--   0        0        0     2074 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/google/database_resource_settings.py
+-rw-r--r--   0        0        0     2837 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/google/deploy_resource_limits.py
+-rw-r--r--   0        0        0     9942 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/google/environment_collection.py
+-rw-r--r--   0        0        0        0 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/providers/google/service_account.py
+-rw-r--r--   0        0        0    14435 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/provisioner.py
+-rw-r--r--   0        0        0      802 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/resource_use_existing.py
+-rw-r--r--   0        0        0      779 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/stage.py
+-rw-r--r--   0        0        0     4279 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/models/toolbox.py
+-rw-r--r--   0        0        0        0 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/tests/__init__.py
+-rw-r--r--   0        0        0     1071 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/tests/base_test_class.py
+-rw-r--r--   0        0        0       75 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service/cnc.yml
+-rw-r--r--   0        0        0      153 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db/cnc.yml
+-rw-r--r--   0        0        0      609 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml
+-rw-r--r--   0        0        0      673 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml
+-rw-r--r--   0        0        0      153 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/cnc.yml
+-rw-r--r--   0        0        0      472 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/environments.yml
+-rw-r--r--   0        0        0      153 2024-05-18 00:09:14.611471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/cnc.yml
+-rw-r--r--   0        0        0      379 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/environments.yml
+-rw-r--r--   0        0        0      153 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/cnc.yml
+-rw-r--r--   0        0        0      564 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml
+-rw-r--r--   0        0        0      231 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-2-db/cnc.yml
+-rw-r--r--   0        0        0      231 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/cnc.yml
+-rw-r--r--   0        0        0      373 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments.yml
+-rw-r--r--   0        0        0      479 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_aws_ecs.yml
+-rw-r--r--   0        0        0      392 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_gcp_run_region_settings.yml
+-rw-r--r--   0        0        0       75 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-custom/cnc.yml
+-rw-r--r--   0        0        0       22 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-custom/custom/deploy/main.sh.j2
+-rw-r--r--   0        0        0      341 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-custom/environments.yml
+-rw-r--r--   0        0        0      228 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-2-service-1-db/cnc.yml
+-rw-r--r--   0        0        0      322 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/backend-2-service-2-db/cnc.yml
+-rw-r--r--   0        0        0      153 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/shared/cnc.yml
+-rw-r--r--   0        0        0      340 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/shared/environments-custom-provision.yml
+-rw-r--r--   0        0        0      294 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/shared/environments.yml
+-rw-r--r--   0        0        0      400 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/shared/environments_aws_ecs.yml
+-rw-r--r--   0        0        0      474 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/shared/environments_aws_ecs_existing_vpc.yml
+-rw-r--r--   0        0        0      299 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/fixtures/shared/environments_gcp_run_lite.yml
+-rw-r--r--   0        0        0     5373 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_builder.py
+-rw-r--r--   0        0        0     2683 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_deployer.py
+-rw-r--r--   0        0        0     2445 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_environment_collection.py
+-rw-r--r--   0        0        0     2287 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_environment_variables.py
+-rw-r--r--   0        0        0     1872 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_environments.py
+-rw-r--r--   0        0        0    13574 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_provisioner.py
+-rw-r--r--   0        0        0     2898 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_services.py
+-rw-r--r--   0        0        0     2224 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/tests/test_toolbox.py
+-rw-r--r--   0        0        0       38 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-18 00:09:14.615471 cocnc-0.1.7/src/cnc/utils/string.py
+-rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 cocnc-0.1.7/PKG-INFO
```

### Comparing `cocnc-0.1.6/LICENSE.txt` & `cocnc-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/README.md` & `cocnc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/pyproject.toml` & `cocnc-0.1.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cocnc"
-version = "0.1.6"
+version = "0.1.7"
 description = "CNC is the first framework for application deployment, a fully distributed and customizable PaaS developer experience, based on docker-compose config files"
 authors = [
     "Adam Abdelaziz <adam.abdelaziz@withcoherence.com>",
     "Zachary Zaro <zach@withcoherence.com>",
 ]
 readme = "README.md"
 packages = [
```

### Comparing `cocnc-0.1.6/src/cnc/commands/build.py` & `cocnc-0.1.7/src/cnc/commands/build.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/deploy.py` & `cocnc-0.1.7/src/cnc/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/info.py` & `cocnc-0.1.7/src/cnc/commands/info.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/provision.py` & `cocnc-0.1.7/src/cnc/commands/provision.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/render.py` & `cocnc-0.1.7/src/cnc/commands/render.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/shell.py` & `cocnc-0.1.7/src/cnc/commands/shell.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/telemetry.py` & `cocnc-0.1.7/src/cnc/commands/telemetry.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/template_editor/inspector.py` & `cocnc-0.1.7/src/cnc/commands/template_editor/inspector.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/commands/toolbox.py` & `cocnc-0.1.7/src/cnc/commands/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 app = typer.Typer()
 
 
 @app.callback()
 def add_common(
     ctx: typer.Context,
     collection_name: str = typer.Option(
-        default="preview", envvar="CNC_COLLECTION_NAME", help="Collection name"
+        default="", envvar="CNC_COLLECTION_NAME", help="Collection name"
     ),
 ):
     """Common Entry Point for Toolbox"""
     print(ctx.obj)
     collection = ctx.obj.application.collection_by_name(collection_name)
     if not collection:
         log.error(
```

### Comparing `cocnc-0.1.6/src/cnc/commands/update.py` & `cocnc-0.1.7/src/cnc/commands/update.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/constants.py` & `cocnc-0.1.7/src/cnc/constants.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/build/main.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/build/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/aws/shared/toolbox/main.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/aws/shared/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run/1/provision/base.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run/1/provision/main.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/base.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/build/nginx.conf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/build/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2` & `cocnc-0.1.7/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/logger.py` & `cocnc-0.1.7/src/cnc/logger.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/main.py` & `cocnc-0.1.7/src/cnc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,14 @@
         help="Environments data file path",
     ),
 ):
     """Common Entry Point for whole app"""
     if "--help" in sys.argv:
         return True
 
-    check_deps()
-
     if not config_file_path.is_file():
         log.error(f"Config file not found: {config_file_path}")
         raise typer.Exit(code=1)
 
     if not environments_file_path.is_file():
         log.error(f"Environments data file not found: {environments_file_path}")
         raise typer.Exit(code=1)
@@ -61,14 +59,16 @@
         environments_file_path,
         config_file_path,
     )
     if not application:
         log.error(f"No application for: {environments_file_path}")
         raise typer.Exit(code=1)
 
+    check_deps(application)
+
     ctx.obj = Common(application)
 
 
 @app.command()
 def hello():
     send_event("hello")
     print("[bold red]Welcome[/bold red] to [bold purple]" "CNC[/bold purple]")
```

### Comparing `cocnc-0.1.6/src/cnc/models/application.py` & `cocnc-0.1.7/src/cnc/models/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def enabled(self):
         return bool(self.template_directory)
 
 
 class Application(BaseModel):
     name: str
     provider: str
-    region: str
+    region: Optional[str] = None
     flavor: str
     version: Union[int, float]
     collections: List[Union[AWSEnvironmentCollection, GCPEnvironmentCollection]] = (
         Field(discriminator="provider")
     )
     template_config: Optional[TemplateConfig] = Field(default_factory=TemplateConfig)
```

### Comparing `cocnc-0.1.6/src/cnc/models/base_model.py` & `cocnc-0.1.7/src/cnc/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/builder.py` & `cocnc-0.1.7/src/cnc/models/builder.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/config/config.py` & `cocnc-0.1.7/src/cnc/models/config/config.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/config/resource.py` & `cocnc-0.1.7/src/cnc/models/config/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,16 @@
 
     @property
     def managed_environment_variables(self):
         _env = self.common_managed_environment_variables
 
         _env.update(
             {
+                f"{self.env_var_base}_IP": self.database_endpoint,
+                f"{self.env_var_base}_HOST": self.database_endpoint,
                 f"{self.env_var_base}_ENDPOINT": self.database_endpoint,
                 f"{self.env_var_base}_PORT": str(STARTING_PORTS[self.engine.upper()]),
                 "DB_NAME": self.db_name,
                 "DB_USER": self.username,
                 "DB_ENGINE": self.engine.lower(),
             }
         )
```

### Comparing `cocnc-0.1.6/src/cnc/models/config/service.py` & `cocnc-0.1.7/src/cnc/models/config/service.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/config/settings.py` & `cocnc-0.1.7/src/cnc/models/config/settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/cycle_stage_base.py` & `cocnc-0.1.7/src/cnc/models/cycle_stage_base.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/deployer.py` & `cocnc-0.1.7/src/cnc/models/deployer.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/environment.py` & `cocnc-0.1.7/src/cnc/models/environment.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/environment_collection.py` & `cocnc-0.1.7/src/cnc/models/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/environment_variable.py` & `cocnc-0.1.7/src/cnc/models/environment_variable.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/amazon/custom_headers.py` & `cocnc-0.1.7/src/cnc/models/providers/amazon/custom_headers.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/amazon/database_resource_settings.py` & `cocnc-0.1.7/src/cnc/models/providers/amazon/database_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/amazon/deploy_resource_limits.py` & `cocnc-0.1.7/src/cnc/models/providers/amazon/deploy_resource_limits.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/amazon/environment_collection.py` & `cocnc-0.1.7/src/cnc/models/providers/amazon/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/google/cache_resource_settings.py` & `cocnc-0.1.7/src/cnc/models/providers/google/cache_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/google/database_resource_settings.py` & `cocnc-0.1.7/src/cnc/models/providers/google/database_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/google/deploy_resource_limits.py` & `cocnc-0.1.7/src/cnc/models/providers/google/deploy_resource_limits.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/providers/google/environment_collection.py` & `cocnc-0.1.7/src/cnc/models/providers/google/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/provisioner.py` & `cocnc-0.1.7/src/cnc/models/provisioner.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/resource_use_existing.py` & `cocnc-0.1.7/src/cnc/models/resource_use_existing.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/stage.py` & `cocnc-0.1.7/src/cnc/models/stage.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/models/toolbox.py` & `cocnc-0.1.7/src/cnc/models/toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/base_test_class.py` & `cocnc-0.1.7/src/cnc/tests/base_test_class.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml` & `cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml` & `cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml` & `cocnc-0.1.7/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_builder.py` & `cocnc-0.1.7/src/cnc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_deployer.py` & `cocnc-0.1.7/src/cnc/tests/test_deployer.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_environment_collection.py` & `cocnc-0.1.7/src/cnc/tests/test_environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_environment_variables.py` & `cocnc-0.1.7/src/cnc/tests/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_environments.py` & `cocnc-0.1.7/src/cnc/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_provisioner.py` & `cocnc-0.1.7/src/cnc/tests/test_provisioner.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/tests/test_services.py` & `cocnc-0.1.7/src/cnc/tests/test_services.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,8 +64,8 @@
         # num standard vars - 2
         num_service_env_vars = 5
 
         for svc in self.environment.config.services:
             num_service_env_vars += len(svc.settings.managed_environment_variables)
 
         service_vars = self.service.environment_variables
-        self.assertEqual(len(service_vars), 12)
+        self.assertEqual(len(service_vars), 14)
```

### Comparing `cocnc-0.1.6/src/cnc/tests/test_toolbox.py` & `cocnc-0.1.7/src/cnc/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/src/cnc/utils/string.py` & `cocnc-0.1.7/src/cnc/utils/string.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.6/PKG-INFO` & `cocnc-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocnc
-Version: 0.1.6
+Version: 0.1.7
 Summary: CNC is the first framework for application deployment, a fully distributed and customizable PaaS developer experience, based on docker-compose config files
 Author: Adam Abdelaziz
 Author-email: adam.abdelaziz@withcoherence.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


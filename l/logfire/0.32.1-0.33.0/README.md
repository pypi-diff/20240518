# Comparing `tmp/logfire-0.32.1.tar.gz` & `tmp/logfire-0.33.0.tar.gz`

## Comparing `logfire-0.32.1.tar` & `logfire-0.33.0.tar`

### file list

```diff
@@ -1,123 +1,127 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.32.1/Makefile
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    55429 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/openai.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 logfire-0.32.1/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_logfire.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    43200 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.32.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.32.1/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.32.1/README.md
--rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 logfire-0.32.1/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.32.1/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.33.0/Makefile
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    58309 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/anthropic.py
+-rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/llm_provider.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/openai.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/types.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0    24452 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_anthropic.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    44176 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.33.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.33.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.33.0/README.md
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.33.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.33.0/PKG-INFO
```

### Comparing `logfire-0.32.1/Makefile` & `logfire-0.33.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/__init__.py` & `logfire-0.33.0/logfire/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 span = DEFAULT_LOGFIRE_INSTANCE.span
 instrument = DEFAULT_LOGFIRE_INSTANCE.instrument
 force_flush = DEFAULT_LOGFIRE_INSTANCE.force_flush
 log_slow_async_callbacks = DEFAULT_LOGFIRE_INSTANCE.log_slow_async_callbacks
 install_auto_tracing = DEFAULT_LOGFIRE_INSTANCE.install_auto_tracing
 instrument_fastapi = DEFAULT_LOGFIRE_INSTANCE.instrument_fastapi
 instrument_openai = DEFAULT_LOGFIRE_INSTANCE.instrument_openai
+instrument_anthropic = DEFAULT_LOGFIRE_INSTANCE.instrument_anthropic
 instrument_asyncpg = DEFAULT_LOGFIRE_INSTANCE.instrument_asyncpg
 instrument_psycopg = DEFAULT_LOGFIRE_INSTANCE.instrument_psycopg
 shutdown = DEFAULT_LOGFIRE_INSTANCE.shutdown
 with_tags = DEFAULT_LOGFIRE_INSTANCE.with_tags
 # with_trace_sample_rate = DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate
 with_settings = DEFAULT_LOGFIRE_INSTANCE.with_settings
```

### Comparing `logfire-0.32.1/logfire/propagate.py` & `logfire-0.33.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/testing.py` & `logfire-0.33.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/ast_utils.py` & `logfire-0.33.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/async_.py` & `logfire-0.33.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/auth.py` & `logfire-0.33.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/backfill.py` & `logfire-0.33.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/cli.py` & `logfire-0.33.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/config.py` & `logfire-0.33.0/logfire/_internal/config.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/config_params.py` & `logfire-0.33.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/constants.py` & `logfire-0.33.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/formatter.py` & `logfire-0.33.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/instrument.py` & `logfire-0.33.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/json_encoder.py` & `logfire-0.33.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/json_formatter.py` & `logfire-0.33.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/json_schema.py` & `logfire-0.33.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/json_types.py` & `logfire-0.33.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/main.py` & `logfire-0.33.0/logfire/_internal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 )
 from .metrics import ProxyMeterProvider
 from .stack_info import get_user_stack_info
 from .tracer import ProxyTracerProvider
 from .utils import uniquify_sequence
 
 if TYPE_CHECKING:
+    import anthropic
     import openai
     from fastapi import FastAPI
     from opentelemetry.metrics import _Gauge as Gauge
     from starlette.requests import Request
     from starlette.websockets import WebSocket
 
 try:
@@ -560,14 +561,19 @@
                 fstring_frame=fstring_frame,
             )
             if extra_attrs:
                 merged_attributes.update(extra_attrs)
                 # Only do this if extra_attrs is not empty since the copy of `attributes` might be expensive.
                 # We update both because attributes_json_schema_properties looks at `attributes`.
                 attributes = {**attributes, **extra_attrs}
+        else:
+            # The message has already been filled in, presumably by a logging integration.
+            # Make sure it's a string.
+            msg = merged_attributes[ATTRIBUTES_MESSAGE_KEY] = str(msg)
+            msg_template = str(msg_template)
 
         otlp_attributes = user_attributes(merged_attributes)
         otlp_attributes = {
             ATTRIBUTES_SPAN_TYPE_KEY: 'log',
             **log_level_attributes(level),
             ATTRIBUTES_MESSAGE_TEMPLATE_KEY: msg_template,
             ATTRIBUTES_MESSAGE_KEY: msg,
@@ -854,17 +860,83 @@
                 enabled. In reality, this means the HTTPX instrumentation, which could otherwise be called since
                 OpenAI uses HTTPX to make HTTP requests.
 
         Returns:
             A context manager that will revert the instrumentation when exited.
                 Use of this context manager is optional.
         """
-        from .integrations.openai import instrument_openai
+        from .integrations.llm_providers.llm_provider import instrument_llm_provider
+        from .integrations.llm_providers.openai import get_endpoint_config, is_async_client, on_response
+
+        return instrument_llm_provider(
+            self,
+            openai_client,
+            suppress_other_instrumentation,
+            'OpenAI',
+            get_endpoint_config,
+            on_response,
+            is_async_client,
+        )
+
+    def instrument_anthropic(
+        self,
+        anthropic_client: anthropic.Anthropic | anthropic.AsyncAnthropic,
+        *,
+        suppress_other_instrumentation: bool = True,
+    ) -> ContextManager[None]:
+        """Instrument an Anthropic client so that spans are automatically created for each request.
+
+        The following methods are instrumented for both the sync and the async clients:
+
+        - [`client.messages.create`](https://docs.anthropic.com/claude/reference/messages_post) — with and without `stream=True`
+        - [`client.beta.tools.messages.create`](https://docs.anthropic.com/claude/docs/tool-use-examples) — with and without `stream=True`
+
+        When `stream=True` a second span is created to instrument the streamed response.
+
+        Example usage:
+
+        ```python
+        import logfire
+        import anthropic
+
+        client = anthropic.Anthropic()
+        logfire.instrument_anthropic(client)
 
-        return instrument_openai(self, openai_client, suppress_other_instrumentation)
+        response = client.messages.create(
+            model='claude-3-haiku-20240307',
+            system='You are a helpful assistant.',
+            messages=[
+                {'role': 'user', 'content': 'What is four plus five?'},
+            ],
+        )
+        print('answer:', response.content[0].text)
+        ```
+
+        Args:
+            anthropic_client: The Anthropic client to instrument, either `anthropic.Anthropic` or `anthropic.AsyncAnthropic`.
+            suppress_other_instrumentation: If True, suppress any other OTEL instrumentation that may be otherwise
+                enabled. In reality, this means the HTTPX instrumentation, which could otherwise be called since
+                OpenAI uses HTTPX to make HTTP requests.
+
+        Returns:
+            A context manager that will revert the instrumentation when exited.
+                Use of this context manager is optional.
+        """
+        from .integrations.llm_providers.anthropic import get_endpoint_config, is_async_client, on_response
+        from .integrations.llm_providers.llm_provider import instrument_llm_provider
+
+        return instrument_llm_provider(
+            self,
+            anthropic_client,
+            suppress_other_instrumentation,
+            'Anthropic',
+            get_endpoint_config,
+            on_response,
+            is_async_client,
+        )
 
     def instrument_asyncpg(self):
         """Instrument the `asyncpg` module so that spans are automatically created for each query."""
         from .integrations.asyncpg import instrument_asyncpg
 
         return instrument_asyncpg()
```

### Comparing `logfire-0.32.1/logfire/_internal/metrics.py` & `logfire-0.33.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/scrubbing.py` & `logfire-0.33.0/logfire/_internal/scrubbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         # See scrubbing_patterns and scrubbing_callback in logfire.configure for more info on these parameters.
         patterns = [*DEFAULT_PATTERNS, *(patterns or [])]
         self._pattern = re.compile('|'.join(patterns), re.IGNORECASE | re.DOTALL)
         self._callback = callback
 
     def scrub_span(self, span: ReadableSpanDict):
         scope = span['instrumentation_scope']
-        if scope and scope.name == 'logfire.openai':
+        if scope and scope.name in ['logfire.openai', 'logfire.anthropic']:
             return
 
         # We need to use BoundedAttributes because:
         # 1. For events and links, we get an error otherwise:
         #      https://github.com/open-telemetry/opentelemetry-python/issues/3761
         # 2. The callback might return a value that isn't of the type required by OTEL,
         #      in which case BoundAttributes will discard it to prevent an error.
```

### Comparing `logfire-0.32.1/logfire/_internal/stack_info.py` & `logfire-0.33.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/tracer.py` & `logfire-0.33.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/utils.py` & `logfire-0.33.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/auto_trace/__init__.py` & `logfire-0.33.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.33.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.33.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/auto_trace/types.py` & `logfire-0.33.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/console.py` & `logfire-0.33.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/fallback.py` & `logfire-0.33.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/file.py` & `logfire-0.33.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/otlp.py` & `logfire-0.33.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.33.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/remove_pending.py` & `logfire-0.33.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/exporters/wrapper.py` & `logfire-0.33.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/integrations/executors.py` & `logfire-0.33.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/integrations/fastapi.py` & `logfire-0.33.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/_internal/integrations/psycopg.py` & `logfire-0.33.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/integrations/logging.py` & `logfire-0.33.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/integrations/loguru.py` & `logfire-0.33.0/logfire/integrations/loguru.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         assert not record.args
 
         if _LOG_METHOD_CODE:  # pragma: no branch
             frame = inspect.currentframe()
             while frame:  # pragma: no branch
                 if frame.f_code is _LOG_METHOD_CODE:
                     msg_template = frame.f_locals.get('message')
-                    if isinstance(msg_template, str):
+                    if msg_template is not None:
                         attributes[ATTRIBUTES_MESSAGE_TEMPLATE_KEY] = msg_template
                     else:  # pragma: no cover
                         _warn_inspection_failure()
 
                     args = frame.f_locals.get('args')
                     if isinstance(args, (tuple, list)):
                         if args:
```

### Comparing `logfire-0.32.1/logfire/integrations/pydantic.py` & `logfire-0.33.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/logfire/integrations/structlog.py` & `logfire-0.33.0/logfire/integrations/structlog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Logfire processor for structlog."""
 
 from structlog.types import EventDict, WrappedLogger
 
 import logfire
 
+from .._internal.constants import ATTRIBUTES_MESSAGE_KEY
 from .logging import RESERVED_ATTRS as LOGGING_RESERVED_ATTRS
 
 RESERVED_ATTRS = LOGGING_RESERVED_ATTRS | {'level', 'event', 'timestamp'}
 """Attributes to strip from the event before sending to Logfire."""
 
 
 class LogfireProcessor:
@@ -17,16 +18,16 @@
         self.console_log = console_log
 
     def __call__(self, logger: WrappedLogger, name: str, event_dict: EventDict) -> EventDict:
         """A middleware to process structlog event, and send it to **Logfire**."""
         attributes = {k: v for k, v in event_dict.items() if k not in RESERVED_ATTRS}
         level = event_dict.get('level', 'info').lower()
         # NOTE: An event can be `None` in structlog. We may want to create a default msg in those cases.
-        msg_template = event_dict.get('event') or 'structlog event'
+        attributes[ATTRIBUTES_MESSAGE_KEY] = message = event_dict.get('event') or 'structlog event'
         logfire.log(
             level=level,  # type: ignore
-            msg_template=msg_template,
+            msg_template=message,
             attributes=attributes,
             console_log=self.console_log,
             custom_scope_suffix='structlog',
         )
         return event_dict
```

### Comparing `logfire-0.32.1/tests/conftest.py` & `logfire-0.33.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_auto_trace.py` & `logfire-0.33.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_backfill.py` & `logfire-0.33.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_cli.py` & `logfire-0.33.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_collect_package_resources.py` & `logfire-0.33.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_configure.py` & `logfire-0.33.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_console_exporter.py` & `logfire-0.33.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_formatter.py` & `logfire-0.33.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_json_args.py` & `logfire-0.33.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_json_args_formatting.py` & `logfire-0.33.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_logfire.py` & `logfire-0.33.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_loguru.py` & `logfire-0.33.0/tests/test_loguru.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 
 def test_loguru(exporter: TestExporter) -> None:
     logger.success('Positional arguments are merged to the message: {}', 'positional')
     logger.info('Keyword arguments are stored in the "extra", we extra them from there: {name}', name='named')
 
     try:
         raise ValueError('This is a test exception')
-    except ValueError:
+    except ValueError as e:
         logger.exception('An exception was raised: {foo}', foo='bar')
+        # Test logging a non-string message.
+        logger.warning(e)
 
     assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
         [
             {
                 'name': 'Positional arguments are merged to the message: {}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
@@ -89,9 +91,25 @@
                             'exception.message': 'This is a test exception',
                             'exception.stacktrace': 'ValueError: This is a test exception',
                             'exception.escaped': 'False',
                         },
                     }
                 ],
             },
+            {
+                'name': 'This is a test exception',
+                'context': {'trace_id': 4, 'span_id': 4, 'is_remote': False},
+                'parent': None,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 13,
+                    'logfire.msg_template': 'This is a test exception',
+                    'logfire.msg': 'This is a test exception',
+                    'code.filepath': 'test_loguru.py',
+                    'code.function': 'test_loguru',
+                    'code.lineno': 28,
+                },
+            },
         ]
     )
```

### Comparing `logfire-0.32.1/tests/test_metrics.py` & `logfire-0.33.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_no_production.py` & `logfire-0.33.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_pydantic_plugin.py` & `logfire-0.33.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_sampling.py` & `logfire-0.33.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_secret_scrubbing.py` & `logfire-0.33.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_slow_async_callbacks.py` & `logfire-0.33.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_source_code_extraction.py` & `logfire-0.33.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_stdlib_logging.py` & `logfire-0.33.0/tests/test_stdlib_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,7 +273,32 @@
                     'code.filepath': 'status.py',
                     'code.function': '__init__',
                     'code.lineno': 123,
                 },
             },
         ]
     )
+
+
+def test_logging_non_string(exporter: TestExporter, logger: Logger):
+    logger.error(123)
+
+    assert exporter.exported_spans_as_dict() == snapshot(
+        [
+            {
+                'name': '123',
+                'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
+                'parent': None,
+                'start_time': 1000000000,
+                'end_time': 1000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': '123',
+                    'logfire.msg': '123',
+                    'code.filepath': 'test_stdlib_logging.py',
+                    'code.function': 'test_logging_non_string',
+                    'code.lineno': 123,
+                },
+            }
+        ]
+    )
```

### Comparing `logfire-0.32.1/tests/test_structlog.py` & `logfire-0.33.0/tests/test_structlog.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,29 +26,48 @@
 
 @pytest.fixture(scope='module')
 def logger() -> Any:
     return structlog.get_logger()
 
 
 def test_structlog(exporter: TestExporter, logger: Logger) -> None:
-    logger.info('This is now being logged.')
+    logger.info('This is now being logged: %s', 123)
+    logger.error(456)
+
     assert exporter.exported_spans_as_dict(fixed_line_number=None) == snapshot(
         [
             {
-                'name': 'This is now being logged.',
+                'name': 'This is now being logged: 123',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 1000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
                     'logfire.level_num': 9,
-                    'logfire.msg_template': 'This is now being logged.',
-                    'logfire.msg': 'This is now being logged.',
+                    'logfire.msg_template': 'This is now being logged: 123',
+                    'logfire.msg': 'This is now being logged: 123',
                     'code.filepath': 'test_structlog.py',
                     'code.function': 'test_structlog',
                     'code.lineno': 33,
                     'logfire.disable_console_log': True,
                 },
-            }
+            },
+            {
+                'name': '456',
+                'context': {'trace_id': 2, 'span_id': 2, 'is_remote': False},
+                'parent': None,
+                'start_time': 2000000000,
+                'end_time': 2000000000,
+                'attributes': {
+                    'logfire.span_type': 'log',
+                    'logfire.level_num': 17,
+                    'logfire.msg_template': '456',
+                    'logfire.msg': '456',
+                    'code.filepath': 'test_structlog.py',
+                    'code.function': 'test_structlog',
+                    'code.lineno': 34,
+                    'logfire.disable_console_log': True,
+                },
+            },
         ]
     )
```

### Comparing `logfire-0.32.1/tests/test_testing.py` & `logfire-0.33.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/test_utils.py` & `logfire-0.33.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/utils.py` & `logfire-0.33.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/exporters/test_fallback_exporter.py` & `logfire-0.33.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/exporters/test_file_exporter.py` & `logfire-0.33.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/exporters/test_otlp_session.py` & `logfire-0.33.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/exporters/test_remove_pending.py` & `logfire-0.33.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.33.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.33.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_asgi.py` & `logfire-0.33.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_asyncpg.py` & `logfire-0.33.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_django.py` & `logfire-0.33.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_fastapi.py` & `logfire-0.33.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_flask.py` & `logfire-0.33.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_httpx.py` & `logfire-0.33.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_openai.py` & `logfire-0.33.0/tests/otel_integrations/test_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     images_response,
 )
 from openai.types.chat import chat_completion, chat_completion_chunk as cc_chunk, chat_completion_message
 from opentelemetry import context
 from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 
 import logfire
-from logfire._internal.integrations.openai import get_endpoint_config
+from logfire._internal.integrations.llm_providers.openai import get_endpoint_config
 from logfire.testing import TestExporter
 
 
 def request_handler(request: httpx.Request) -> httpx.Response:
     """Used to mock httpx requests
 
     We do this instead of using pytest-httpx since 1) it's nearly as simple 2) pytest-httpx doesn't support Python 3.8.
@@ -243,14 +243,15 @@
                             'model': 'gpt-4',
                         }
                     ),
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': IsJson(
                         {
                             'message': {
                                 'content': 'Nine',
                                 'role': 'assistant',
                                 'function_call': None,
                                 'tool_calls': None,
@@ -318,14 +319,15 @@
                             'model': 'gpt-4',
                         }
                     ),
                     'async': True,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': IsJson(
                         {
                             'message': {
                                 'content': 'Nine',
                                 'role': 'assistant',
                                 'function_call': None,
                                 'tool_calls': None,
@@ -385,14 +387,15 @@
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                 },
             },
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
@@ -403,14 +406,15 @@
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': 'test_sync_chat_empty_response_chunk',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"","chunk_count":0}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
@@ -439,14 +443,15 @@
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"empty choices in response chunk"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                 },
             },
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
@@ -457,14 +462,15 @@
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': 'test_sync_chat_empty_response_choices',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"","chunk_count":0}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
@@ -495,14 +501,15 @@
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                 },
             },
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
@@ -513,14 +520,15 @@
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': '<genexpr>',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is secret","chunk_count":2}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
@@ -554,14 +562,15 @@
                     'code.lineno': 123,
                     'request_data': '{"messages":[{"role":"system","content":"You are a helpful assistant."},{"role":"user","content":"What is four plus five?"}],"model":"gpt-4","stream":true}',
                     'async': True,
                     'logfire.msg_template': 'Chat Completion with {request_data[model]!r}',
                     'logfire.msg': "Chat Completion with 'gpt-4'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                 },
             },
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
@@ -572,14 +581,15 @@
                     'async': True,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': 'test_async_chat_completions_stream',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-4' took 1.00s",
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is secret","chunk_count":2}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
@@ -604,14 +614,15 @@
                     'code.function': 'test_completions',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"What is four plus five?"}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': '{"finish_reason":"stop","text":"Nine","usage":null}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
                 },
             }
         ]
     )
 
@@ -638,14 +649,15 @@
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"What is four plus five?","stream":true}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{}}}',
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                 },
             },
             {
                 'name': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                 'context': {'trace_id': 2, 'span_id': 3, 'is_remote': False},
                 'parent': None,
                 'start_time': 5000000000,
@@ -656,14 +668,15 @@
                     'async': False,
                     'logfire.msg_template': 'streaming response from {request_data[model]!r} took {duration:.2f}s',
                     'code.filepath': 'test_openai.py',
                     'code.function': '<genexpr>',
                     'code.lineno': 123,
                     'logfire.msg': "streaming response from 'gpt-3.5-turbo-instruct' took 1.00s",
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
                     'duration': 1.0,
                     'response_data': '{"combined_chunk_content":"The answer is Nine","chunk_count":3}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"duration":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
@@ -688,14 +701,15 @@
                     'code.function': 'test_embeddings',
                     'code.lineno': 123,
                     'request_data': '{"input":"This is a sentence to embed.","model":"text-embedding-3-small","encoding_format":"base64"}',
                     'async': False,
                     'logfire.msg_template': 'Embedding Creation with {request_data[model]!r}',
                     'logfire.msg': "Embedding Creation with 'text-embedding-3-small'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': '{"usage":{"prompt_tokens":1,"total_tokens":2}}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object","properties":{"usage":{"type":"object","title":"Usage","x-python-datatype":"PydanticModel"}}}}}',
                 },
             }
         ]
     )
 
@@ -720,14 +734,15 @@
                     'code.function': 'test_images',
                     'code.lineno': 123,
                     'request_data': '{"prompt":"A picture of a cat.","model":"dall-e-3"}',
                     'async': False,
                     'logfire.msg_template': 'Image Generation with {request_data[model]!r}',
                     'logfire.msg': "Image Generation with 'dall-e-3'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': '{"images":[{"b64_json":null,"revised_prompt":"revised prompt","url":"https://example.com/image.jpg"}]}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object","properties":{"images":{"type":"array","items":{"type":"object","title":"Image","x-python-datatype":"PydanticModel"}}}}}}',
                 },
             }
         ]
     )
 
@@ -772,14 +787,15 @@
                     'code.function': 'test_dont_suppress_httpx',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"xxx"}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': '{"finish_reason":"stop","text":"Nine","usage":null}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
@@ -808,14 +824,15 @@
                     'code.function': 'test_suppress_httpx',
                     'code.lineno': 123,
                     'request_data': '{"model":"gpt-3.5-turbo-instruct","prompt":"xxx"}',
                     'async': False,
                     'logfire.msg_template': 'Completion with {request_data[model]!r}',
                     'logfire.msg': "Completion with 'gpt-3.5-turbo-instruct'",
                     'logfire.span_type': 'span',
+                    'logfire.tags': ('LLM',),
                     'response_data': '{"finish_reason":"stop","text":"Nine","usage":null}',
                     'logfire.json_schema': '{"type":"object","properties":{"request_data":{"type":"object"},"async":{},"response_data":{"type":"object"}}}',
                 },
             },
         ]
     )
 
@@ -846,23 +863,25 @@
 
 def test_unknown_method(instrumented_client: openai.Client, exporter: TestExporter) -> None:
     response = instrumented_client.files.create(file=BytesIO(b'file contents'), purpose='fine-tune')
     assert response.filename == 'test.txt'
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
-                'name': 'Unable to instrument OpenAI API call: {error}',
+                'name': 'Unable to instrument {suffix} API call: {error}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 1000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
+                    'suffix': 'OpenAI',
                     'logfire.level_num': 13,
-                    'logfire.msg_template': 'Unable to instrument OpenAI API call: {error}',
+                    'logfire.msg_template': 'Unable to instrument {suffix} API call: {error}',
                     'logfire.msg': 'Unable to instrument OpenAI API call: `model` not found in request data',
                     'code.filepath': 'test_openai.py',
                     'code.function': 'test_unknown_method',
                     'code.lineno': 123,
                     'error': '`model` not found in request data',
                     'kwargs': IsStr(),
                     'logfire.json_schema': IsStr(),
@@ -874,30 +893,32 @@
 
 async def test_async_unknown_method(instrumented_async_client: openai.AsyncClient, exporter: TestExporter) -> None:
     response = await instrumented_async_client.files.create(file=BytesIO(b'file contents'), purpose='fine-tune')
     assert response.filename == 'test.txt'
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
-                'name': 'Unable to instrument OpenAI API call: {error}',
+                'name': 'Unable to instrument {suffix} API call: {error}',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
                 'start_time': 1000000000,
                 'end_time': 1000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
+                    'logfire.tags': ('LLM',),
                     'logfire.level_num': 13,
-                    'logfire.msg_template': 'Unable to instrument OpenAI API call: {error}',
+                    'logfire.msg_template': 'Unable to instrument {suffix} API call: {error}',
                     'logfire.msg': 'Unable to instrument OpenAI API call: `model` not found in request data',
                     'code.filepath': 'test_openai.py',
                     'code.function': 'test_async_unknown_method',
                     'code.lineno': 123,
                     'error': '`model` not found in request data',
                     'kwargs': IsStr(),
                     'logfire.json_schema': IsStr(),
+                    'suffix': 'OpenAI',
                 },
             }
         ]
     )
 
 
 def test_get_endpoint_config_json_not_dict():
```

### Comparing `logfire-0.32.1/tests/otel_integrations/test_psycopg.py` & `logfire-0.33.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_requests.py` & `logfire-0.33.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.33.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_starlette.py` & `logfire-0.33.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/test_wsgi.py` & `logfire-0.33.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.33.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/LICENSE` & `logfire-0.33.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/README.md` & `logfire-0.33.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.32.1/pyproject.toml` & `logfire-0.33.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.32.1"
+version = "0.33.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
@@ -123,14 +123,15 @@
     "mkdocs-glightbox>=0.3.7",
     "mkdocstrings-python>=1.8.0",
     "coverage[toml]>=7.5.0",
     "psycopg[binary]",
     "psycopg2-binary",
     "asyncpg",
     "cloudpickle>=3.0.0",
+    "anthropic",
 ]
 
 [tool.rye.scripts]
 typecheck = "pyright"
 docs = "mkdocs build"
 # no strict so you can build the docs without insiders packages
 docs-serve = "mkdocs serve --no-strict"
```

### Comparing `logfire-0.32.1/PKG-INFO` & `logfire-0.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.32.1
+Version: 0.33.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```


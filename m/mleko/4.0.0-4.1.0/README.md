# Comparing `tmp/mleko-4.0.0.tar.gz` & `tmp/mleko-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-4.0.0.tar", max compression
+gzip compressed data, was "mleko-4.1.0.tar", max compression
```

## Comparing `mleko-4.0.0.tar` & `mleko-4.1.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0    10947 2024-05-09 10:07:38.962391 mleko-4.0.0/LICENSE
--rw-r--r--   0        0        0     5019 2024-05-09 10:07:38.962391 mleko-4.0.0/README.md
--rw-r--r--   0        0        0     1976 2024-05-09 10:08:07.210592 mleko-4.0.0/mleko/__init__.py
--rw-r--r--   0        0        0      585 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    16986 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0     1560 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     1012 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
--rw-r--r--   0        0        0     2989 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1248 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/json_fingerprinter.py
--rw-r--r--   0        0        0     5578 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
--rw-r--r--   0        0        0    14262 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
--rw-r--r--   0        0        0     1219 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0     1832 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/__init__.py
--rw-r--r--   0        0        0      650 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/base_cache_handler.py
--rw-r--r--   0        0        0     1102 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/joblib_cache_handler.py
--rw-r--r--   0        0        0     1251 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/json_cache_handler.py
--rw-r--r--   0        0        0     1196 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/pickle_cache_handler.py
--rw-r--r--   0        0        0     1207 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/string_cache_handler.py
--rw-r--r--   0        0        0     1954 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/handlers/vaex_cache_handler.py
--rw-r--r--   0        0        0     8312 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      805 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      492 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1613 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    15248 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     6592 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/data_schema.py
--rw-r--r--   0        0        0      774 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/__init__.py
--rw-r--r--   0        0        0      900 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/base_exporter.py
--rw-r--r--   0        0        0     8725 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/local_exporter.py
--rw-r--r--   0        0        0     8191 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/export/s3_exporter.py
--rw-r--r--   0        0        0     1614 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0    11612 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     7661 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5156 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5439 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7257 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5803 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      569 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/__init__.py
--rw-r--r--   0        0        0     1615 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/base_filter.py
--rw-r--r--   0        0        0     3927 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/expression_filter.py
--rw-r--r--   0        0        0     7160 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/filter/imblearn_resampling_filter.py
--rw-r--r--   0        0        0      878 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2747 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    20020 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0    11181 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      680 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1501 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     4254 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6732 2024-05-09 10:07:38.966391 mleko-4.0.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1612 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     9362 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     6882 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4743 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0    11533 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3744 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4150 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      388 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/__init__.py
--rw-r--r--   0        0        0    18964 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/base_model.py
--rw-r--r--   0        0        0    10756 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/lgbm_model.py
--rw-r--r--   0        0        0      413 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/tune/__init__.py
--rw-r--r--   0        0        0     3785 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/tune/base_tuner.py
--rw-r--r--   0        0        0    16390 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/model/tune/optuna_tuner.py
--rw-r--r--   0        0        0      645 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1382 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4658 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     9807 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      928 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     3931 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     3312 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/export_step.py
--rw-r--r--   0        0        0     6310 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     3115 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/filter_step.py
--rw-r--r--   0        0        0     2858 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     8139 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/model_step.py
--rw-r--r--   0        0        0     3002 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     5933 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0     3551 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/pipeline/steps/tune_step.py
--rw-r--r--   0        0        0        0 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/py.typed
--rw-r--r--   0        0        0      977 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     9753 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3431 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0     4724 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0    11820 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/s3_helpers.py
--rw-r--r--   0        0        0     1414 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     3641 2024-05-09 10:07:38.970391 mleko-4.0.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2608 2024-05-09 10:08:07.210592 mleko-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     6323 1970-01-01 00:00:00.000000 mleko-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-18 16:27:42.343222 mleko-4.1.0/LICENSE
+-rw-r--r--   0        0        0     5019 2024-05-18 16:27:42.343222 mleko-4.1.0/README.md
+-rw-r--r--   0        0        0     1976 2024-05-18 16:28:13.179034 mleko-4.1.0/mleko/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    16986 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0     1560 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-18 16:27:42.343222 mleko-4.1.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     1012 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
+-rw-r--r--   0        0        0     2989 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1248 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/json_fingerprinter.py
+-rw-r--r--   0        0        0     5578 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
+-rw-r--r--   0        0        0    14262 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
+-rw-r--r--   0        0        0     1219 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0     1832 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/__init__.py
+-rw-r--r--   0        0        0      650 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/base_cache_handler.py
+-rw-r--r--   0        0        0     1102 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/joblib_cache_handler.py
+-rw-r--r--   0        0        0     1251 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/json_cache_handler.py
+-rw-r--r--   0        0        0     1196 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/pickle_cache_handler.py
+-rw-r--r--   0        0        0     1207 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/string_cache_handler.py
+-rw-r--r--   0        0        0     1954 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/handlers/vaex_cache_handler.py
+-rw-r--r--   0        0        0     8312 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      805 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      492 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1613 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    15248 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     6592 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/data_schema.py
+-rw-r--r--   0        0        0      774 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/base_exporter.py
+-rw-r--r--   0        0        0     8725 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/local_exporter.py
+-rw-r--r--   0        0        0     8191 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/export/s3_exporter.py
+-rw-r--r--   0        0        0     1614 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0    11612 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     7661 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5156 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5439 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7257 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5803 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      569 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/__init__.py
+-rw-r--r--   0        0        0     1615 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/base_filter.py
+-rw-r--r--   0        0        0     3927 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/expression_filter.py
+-rw-r--r--   0        0        0     7160 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/filter/imblearn_resampling_filter.py
+-rw-r--r--   0        0        0      878 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2747 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    20020 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0    11181 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      680 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1501 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4254 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     7029 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1797 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     9362 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     6882 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4701 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/expression_transformer.py
+-rw-r--r--   0        0        0     4743 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0    11533 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3744 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4150 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      388 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/__init__.py
+-rw-r--r--   0        0        0    18964 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/base_model.py
+-rw-r--r--   0        0        0    10756 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/lgbm_model.py
+-rw-r--r--   0        0        0      413 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/tune/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/tune/base_tuner.py
+-rw-r--r--   0        0        0    17012 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/model/tune/optuna_tuner.py
+-rw-r--r--   0        0        0      645 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1382 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4658 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     9807 2024-05-18 16:27:42.347222 mleko-4.1.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      928 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     3931 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     3312 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/export_step.py
+-rw-r--r--   0        0        0     6310 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     3115 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/filter_step.py
+-rw-r--r--   0        0        0     2858 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     8139 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/model_step.py
+-rw-r--r--   0        0        0     3002 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     5933 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0     3551 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/pipeline/steps/tune_step.py
+-rw-r--r--   0        0        0        0 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/py.typed
+-rw-r--r--   0        0        0      977 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     9753 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3431 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0     4724 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0    11820 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/s3_helpers.py
+-rw-r--r--   0        0        0     1414 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     3641 2024-05-18 16:27:42.351222 mleko-4.1.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2608 2024-05-18 16:28:13.179034 mleko-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6323 1970-01-01 00:00:00.000000 mleko-4.1.0/PKG-INFO
```

### Comparing `mleko-4.0.0/LICENSE` & `mleko-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/README.md` & `mleko-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/__init__.py` & `mleko-4.1.0/mleko/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning
 practitioners looking to build robust models efficiently.
 """
 
 from __future__ import annotations
 
 
-__version__ = "4.0.0"
+__version__ = "4.1.0"
```

### Comparing `mleko-4.0.0/mleko/cache/__init__.py` & `mleko-4.1.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/cache_mixin.py` & `mleko-4.1.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/__init__.py` & `mleko-4.1.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/json_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/json_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-4.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/__init__.py` & `mleko-4.1.0/mleko/cache/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/base_cache_handler.py` & `mleko-4.1.0/mleko/cache/handlers/base_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/joblib_cache_handler.py` & `mleko-4.1.0/mleko/cache/handlers/joblib_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/json_cache_handler.py` & `mleko-4.1.0/mleko/cache/handlers/json_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/pickle_cache_handler.py` & `mleko-4.1.0/mleko/cache/handlers/pickle_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/string_cache_handler.py` & `mleko-4.1.0/mleko/cache/handlers/string_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/handlers/vaex_cache_handler.py` & `mleko-4.1.0/mleko/cache/handlers/vaex_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/cache/lru_cache_mixin.py` & `mleko-4.1.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/__init__.py` & `mleko-4.1.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/convert/base_converter.py` & `mleko-4.1.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-4.1.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/data_schema.py` & `mleko-4.1.0/mleko/dataset/data_schema.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/export/__init__.py` & `mleko-4.1.0/mleko/dataset/export/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/export/base_exporter.py` & `mleko-4.1.0/mleko/dataset/export/base_exporter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/export/local_exporter.py` & `mleko-4.1.0/mleko/dataset/export/local_exporter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/export/s3_exporter.py` & `mleko-4.1.0/mleko/dataset/export/s3_exporter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/__init__.py` & `mleko-4.1.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-4.1.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-4.1.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-4.1.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-4.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-4.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-4.1.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/filter/__init__.py` & `mleko-4.1.0/mleko/dataset/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/filter/base_filter.py` & `mleko-4.1.0/mleko/dataset/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/filter/expression_filter.py` & `mleko-4.1.0/mleko/dataset/filter/expression_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/filter/imblearn_resampling_filter.py` & `mleko-4.1.0/mleko/dataset/filter/imblearn_resampling_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/ingest/__init__.py` & `mleko-4.1.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/ingest/base_ingester.py` & `mleko-4.1.0/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-4.1.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-4.1.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/split/__init__.py` & `mleko-4.1.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/split/base_splitter.py` & `mleko-4.1.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/split/expression_splitter.py` & `mleko-4.1.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/split/random_splitter.py` & `mleko-4.1.0/mleko/dataset/split/random_splitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 can be stratified by specifying a column name to use for stratification.
 """
 
 from __future__ import annotations
 
 from pathlib import Path
 
+import pandas as pd
 import vaex
 from sklearn.model_selection import train_test_split
 
 from mleko.cache.fingerprinters import VaexFingerprinter
 from mleko.cache.handlers.vaex_cache_handler import VAEX_DATAFRAME_CACHE_HANDLER
+from mleko.utils import auto_repr, get_column, get_columns, get_filtered_df
 from mleko.utils.custom_logger import CustomLogger
-from mleko.utils.decorators import auto_repr
-from mleko.utils.vaex_helpers import get_column, get_filtered_df
 
 from .base_splitter import BaseSplitter
 
 
 logger = CustomLogger()
 """A CustomLogger instance that's used throughout the module for logging."""
 
@@ -32,38 +32,39 @@
     """
 
     @auto_repr
     def __init__(
         self,
         data_split: tuple[float, float] = (0.80, 0.20),
         shuffle: bool = True,
-        stratify: str | None = None,
+        stratify: str | tuple[str, ...] | list[str] | None = None,
         random_state: int | None = 42,
         cache_directory: str | Path = "data/random-splitter",
         cache_size: int = 1,
     ) -> None:
         """Initializes the `RandomSplitter` with the given parameters.
 
         Note:
-            The stratification is performed before the split, meaning that the split will be performed on the stratified
-            data. For example, if the data is split into 80% train and 20% test, and the stratification column contains
-            80% of the rows with value 0 and 20% of the rows with value 1, the resulting split will contain 80% of the
-            rows with value 0 and 20% of the rows with value 1.
-
-        Warning:
-            If `stratify` is not None and the target column is a string/categorical, the target feature must not have
-            any missing values. Please make sure to handle missing values before using this splitter by either dropping
-            the rows with missing values, imputing the missing values, or transforming the target to numeric or boolean.
+            If `stratify` is not None and the type of the data is string/categorical the feature (s) must not have
+            any missing values. Please make sure to handle missing values before using this splitter by either
+            dropping the rows with missing values, imputing the missing values, or transforming the target to
+            numeric or boolean.
+
+            If multiple features are provided for stratification, there must be at least one row for each unique
+            combination of the feature values. Otherwise, the splitter will raise an error.
 
         Args:
             data_split: A tuple containing the desired split percentages or weights for the train and test dataframes.
                 If the sum of the values is not equal to 1, the values will be normalized. Meaning, if the values are
                 (0.90, 0.20), the resulting split will be (0.818, 0.182).
             shuffle: Whether to shuffle the data before splitting.
-            stratify: The name of the column to use for stratification. If None, stratification will not be performed.
+            stratify: Name of the feature(s) to use for stratification. If None, the data will be split without
+                stratification. If a list of features is provided, the data will be stratified based on the unique
+                combinations of the features, i.e., the data will be split such that each unique combination of the
+                features is present in both splits in the same proportion as in the original data.
             random_state: The seed to use for random number generation.
             cache_directory: The target directory where the split dataframes are to be saved.
             cache_size: The maximum number of entries to keep in the cache.
 
         Example:
             >>> import vaex
             >>> from mleko.data.split import RandomSplitter
@@ -78,15 +79,15 @@
                 #    x    y
                 0    2    1
                 1    4    0
         """
         super().__init__(cache_directory, cache_size)
         self._idx2_size = [split / sum(data_split) for split in data_split][1]
         self._shuffle = shuffle
-        self._stratify = stratify
+        self._stratify = tuple(stratify) if isinstance(stratify, (list, tuple)) else (stratify,) if stratify else None
         self._random_state = random_state
 
     def split(
         self,
         dataframe: vaex.DataFrame,
         cache_group: str | None = None,
         force_recompute: bool = False,
@@ -131,29 +132,31 @@
         Returns:
             A tuple containing the split dataframes.
         """
         index_name = "index"
         df = dataframe.copy()
         df[index_name] = vaex.vrange(0, df.shape[0])
         index = get_column(df, index_name)
-        target = get_column(df, self._stratify).to_numpy() if self._stratify else None
+        stratification: pd.DataFrame | None = (
+            get_columns(df, list(self._stratify)).to_pandas_df() if self._stratify else None  # type: ignore
+        )
 
         if self._shuffle:
             logger.info("Shuffling data before splitting.")
-        if target is None:
+        if stratification is None:
             logger.info("Splitting data without stratification.")
         else:
-            logger.info(f"Splitting data with stratification on column {self._stratify!r}.")
+            logger.info(f"Splitting data with stratification on feature(s) {self._stratify!r}.")
 
         idx1, idx2 = train_test_split(
             index.values,
             test_size=self._idx2_size,
             random_state=self._random_state,
             shuffle=self._shuffle,
-            stratify=target,
+            stratify=stratification,
         )
 
         df1 = get_filtered_df(df, index.isin(idx1)).extract()
         df2 = get_filtered_df(df, index.isin(idx2)).extract()
         logger.info(f"Split dataframe into two dataframes with shapes {df1.shape} and {df2.shape}.")
         df1.delete_virtual_column(index_name)
         df2.delete_virtual_column(index_name)
```

### Comparing `mleko-4.0.0/mleko/dataset/transform/__init__.py` & `mleko-4.1.0/mleko/dataset/transform/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 transformation task. By using these feature transformers sequentially, you can create a complete feature
 transformation workflow within the pipeline.
 
 The following feature transformers are provided by the subpackage:
     - `BaseTransformer`: The abstract base class for all feature transformers.
     - `CompositeTransformer`: A feature transformer that combines multiple feature transformers into a single feature
         transformer.
+    - `ExpressionTransformer`: A feature transformer for creating new features using expressions.
     - `FrequencyEncoderTransformer`: A feature transformer for encoding categorical features using frequency encoding.
     - `LabelEncoderTransformer`: A feature transformer for encoding categorical features using label encoding.
     - `MaxAbsScalerTransformer`: A feature transformer for scaling features using maximum absolute scaling.
     - `MinMaxScalerTransformer`: A feature transformer for scaling features using min-max scaling.
 """
 
 from .base_transformer import BaseTransformer
 from .composite_transformer import CompositeTransformer
+from .expression_transformer import ExpressionTransformer
 from .frequency_encoder_transformer import FrequencyEncoderTransformer
 from .label_encoder_transformer import LabelEncoderTransformer
 from .max_abs_scaler_transformer import MaxAbsScalerTransformer
 from .min_max_scaler_transformer import MinMaxScalerTransformer
 
 
 __all__ = [
     "BaseTransformer",
     "CompositeTransformer",
+    "ExpressionTransformer",
     "FrequencyEncoderTransformer",
     "LabelEncoderTransformer",
     "MaxAbsScalerTransformer",
     "MinMaxScalerTransformer",
 ]
```

### Comparing `mleko-4.0.0/mleko/dataset/transform/base_transformer.py` & `mleko-4.1.0/mleko/dataset/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/transform/composite_transformer.py` & `mleko-4.1.0/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-4.1.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-4.1.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-4.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-4.1.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/model/base_model.py` & `mleko-4.1.0/mleko/model/base_model.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/model/lgbm_model.py` & `mleko-4.1.0/mleko/model/lgbm_model.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/model/tune/base_tuner.py` & `mleko-4.1.0/mleko/model/tune/base_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/model/tune/optuna_tuner.py` & `mleko-4.1.0/mleko/model/tune/optuna_tuner.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import getpass
 import inspect
 import logging
 import platform
 import random
 from datetime import datetime
 from pathlib import Path
-from typing import Callable, Hashable, Literal
+from typing import Any, Callable, Hashable, Literal
 
 import optuna
 import vaex
 from optuna.samplers import (
     BaseSampler,
     BruteForceSampler,
     CmaEsSampler,
@@ -65,14 +65,15 @@
                 [optuna.Trial, DataSchema, list[tuple[vaex.DataFrame, vaex.DataFrame]]],
                 float | list[float] | tuple[float, ...],
             ]
         ),
         direction: OptimizeDirection | list[OptimizeDirection],
         num_trials: int,
         cv_folds: Callable[[DataSchema, vaex.DataFrame], list[tuple[vaex.DataFrame, vaex.DataFrame]]] | None = None,
+        enqueue_trials: list[dict[str, Any]] | None = None,
         sampler: BaseSampler | None = None,
         pruner: optuna.pruners.BasePruner | None = None,
         study_name: str | None = None,
         storage: str | RDBStorage | None = None,
         load_if_exists: bool = False,
         random_state: int | None = 42,
         cache_directory: str | Path = "data/optuna-tuner",
@@ -125,14 +126,18 @@
                 If a list of directions is given, the tuner will perform multi-objective
                 optimization. The length of the list must match the length of the list
                 returned by the objective function.
             cv_folds: The cross-validation function to use. The function must accept
                 the data schema and the DataFrame to be tuned on and return a list of
                 tuples containing the training and validation DataFrames. The length
                 of the list must match the number of folds to perform.
+            enqueue_trials: A list of dictionaries containing the parameters configurations
+                to enqueue trials. The keys of the dictionary must match the parameter
+                names of the objective function. The tuner will enqueue the trials
+                with the specified configurations before starting the optimization.
             num_trials: The number of trials to perform.
             sampler: The Optuna sampler to use, if None `TPESampler` is
                 used for single-objective optimization and `NSGAIISampler`
                 is used for multi-objective optimization.
             pruner: The Optuna pruner to use, if None `optuna.pruners.MedianPruner` is
                 used.
             study_name: The name of the study. If None, the current date and time will
@@ -187,14 +192,15 @@
             >>> best_trial, best_score, study = optuna_tuner.tune(data_schema, dataframe)
         """
         super().__init__(cache_directory, cache_size)
         self._objective_function = objective_function
         self._direction = direction
         self._num_trials = num_trials
         self._cv_folds = cv_folds
+        self._enqueue_trials = enqueue_trials
         self._sampler = sampler or (TPESampler() if isinstance(direction, list) else NSGAIISampler())
         self._pruner = pruner or optuna.pruners.MedianPruner()
         self._study_name = study_name if study_name is not None else datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self._storage = storage
         self._load_if_exists = load_if_exists
         self._using_optuna_dashboard = True if self._storage is not None else False
         self._random_state = random_state
@@ -225,14 +231,19 @@
             sampler=self._sampler,
             pruner=self._pruner,
             study_name=self._study_name,
             direction=self._direction if isinstance(self._direction, str) else None,
             directions=self._direction if isinstance(self._direction, list) else None,
             load_if_exists=self._load_if_exists,
         )
+
+        if self._enqueue_trials is not None:
+            for trial in self._enqueue_trials:
+                study.enqueue_trial(params=trial, skip_if_exists=True)
+
         if self._using_optuna_dashboard:
             direction_str = (
                 self._direction if isinstance(self._direction, str) else ", ".join(self._direction)
             ).upper()
             save_note(
                 study,
                 f"""# Experiment Documentation
```

### Comparing `mleko-4.0.0/mleko/pipeline/__init__.py` & `mleko-4.1.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/data_container.py` & `mleko-4.1.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/pipeline.py` & `mleko-4.1.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/pipeline_step.py` & `mleko-4.1.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/__init__.py` & `mleko-4.1.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/convert_step.py` & `mleko-4.1.0/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/export_step.py` & `mleko-4.1.0/mleko/pipeline/steps/export_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-4.1.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/filter_step.py` & `mleko-4.1.0/mleko/pipeline/steps/filter_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/ingest_step.py` & `mleko-4.1.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/model_step.py` & `mleko-4.1.0/mleko/pipeline/steps/model_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/split_step.py` & `mleko-4.1.0/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/transform_step.py` & `mleko-4.1.0/mleko/pipeline/steps/transform_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/pipeline/steps/tune_step.py` & `mleko-4.1.0/mleko/pipeline/steps/tune_step.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/__init__.py` & `mleko-4.1.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/custom_logger.py` & `mleko-4.1.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/decorators.py` & `mleko-4.1.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/file_helpers.py` & `mleko-4.1.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/s3_helpers.py` & `mleko-4.1.0/mleko/utils/s3_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/tqdm_helpers.py` & `mleko-4.1.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/mleko/utils/vaex_helpers.py` & `mleko-4.1.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-4.0.0/pyproject.toml` & `mleko-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "4.0.0"
+version = "4.1.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/klarna-incubator/mleko"
 repository = "https://github.com/klarna-incubator/mleko"
 documentation = "https://mleko.readthedocs.io"
@@ -46,15 +46,15 @@
 isort = ">=5.10.1"
 moto = "^4.1.4"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pytest-mock = "^3.10.0"
-python-semantic-release = "^8.7.0"
+python-semantic-release = "^9.0.0"
 ipykernel = "^6.21.3"
 safety = ">=1.10.3"
 pyright = "^1.1.316"
 sphinx = "7.1.2"
 furo = "^2023.9.10"
 myst-parser = "^2.0.0"
 sphinx-autodoc-typehints = "^1.25.2"
```

### Comparing `mleko-4.0.0/PKG-INFO` & `mleko-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 4.0.0
+Version: 4.1.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/klarna-incubator/mleko
 License: Apache-2.0
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.1,<3.11.dev0
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/autogluon.core-1.1.1b20240516.tar.gz` & `tmp/autogluon.core-1.1.1b20240517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-1.1.1b20240516.tar", last modified: Thu May 16 09:04:32 2024, max compression
+gzip compressed data, was "autogluon.core-1.1.1b20240517.tar", last modified: Fri May 17 09:04:58 2024, max compression
```

## Comparing `autogluon.core-1.1.1b20240516.tar` & `autogluon.core-1.1.1b20240517.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.455421 autogluon.core-1.1.1b20240516/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.455421 autogluon.core-1.1.1b20240516/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.459421 autogluon.core-1.1.1b20240516/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.459421 autogluon.core-1.1.1b20240516/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.459421 autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.459421 autogluon.core-1.1.1b20240516/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.463420 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29424 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.463420 autogluon.core-1.1.1b20240516/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.463420 autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.463420 autogluon.core-1.1.1b20240516/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.463420 autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)   100159 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.463420 autogluon.core-1.1.1b20240516/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66746 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.467420 autogluon.core-1.1.1b20240516/src/autogluon/core/stacked_overfitting/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/stacked_overfitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   198919 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36236 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.471420 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    50695 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 09:04:09.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:04:32.459421 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:04:32.000000 autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.001549 autogluon.core-1.1.1b20240517/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.001549 autogluon.core-1.1.1b20240517/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.005549 autogluon.core-1.1.1b20240517/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.005549 autogluon.core-1.1.1b20240517/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.005549 autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.005549 autogluon.core-1.1.1b20240517/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.009549 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29424 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.009549 autogluon.core-1.1.1b20240517/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.009549 autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    26505 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.009549 autogluon.core-1.1.1b20240517/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.009549 autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102328 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.009549 autogluon.core-1.1.1b20240517/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67049 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45241 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.013549 autogluon.core-1.1.1b20240517/src/autogluon/core/stacked_overfitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/stacked_overfitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   199164 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36236 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.017549 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50705 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-17 09:04:33.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:04:58.005549 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:04:57.000000 autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-1.1.1b20240516/PKG-INFO` & `autogluon.core-1.1.1b20240517/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.1.1b20240516
+Version: 1.1.1b20240517
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-1.1.1b20240516/setup.py` & `autogluon.core-1.1.1b20240517/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/_setup_utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/constants.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/data/cleaner.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/dataset.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/executors.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/__init__.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/_utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         self.feature_metadata = None  # External feature metadata, do not use internally
         self._features_internal = None  # Internal features, safe to use internally via the `_features` property
         self._feature_metadata = None  # Internal feature metadata, safe to use internally
         self._is_features_in_same_as_ex = None  # Whether self.features == self._features_internal
 
         self.fit_time = None  # Time taken to fit in seconds (Training data)
         self.predict_time = None  # Time taken to predict in seconds (Validation data)
+        self._predict_n_size = None  # Batch size used to calculate predict_time
         self.predict_1_time = None  # Time taken to predict 1 row of data in seconds (with batch size `predict_1_batch_size` in params_aux)
         self.compile_time = None  # Time taken to compile the model in seconds
         self.val_score = None  # Score with eval_metric (Validation data)
 
         self._user_params, self._user_params_aux = self._init_user_params(params=hyperparameters)
 
         self.params = {}
@@ -927,39 +928,65 @@
         """
         y_pred += self.conformalize
         return y_pred
 
     def predict(self, X, **kwargs) -> np.ndarray:
         """
         Returns class predictions of X.
-        For binary and multiclass problems, this returns the predicted class labels as a Series.
-        For regression problems, this returns the predicted values as a Series.
+        For binary and multiclass problems, this returns the predicted class labels as a 1d numpy array.
+        For regression problems, this returns the predicted values as a 1d numpy array.
         """
         y_pred_proba = self.predict_proba(X, **kwargs)
         y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=self.problem_type)
         return y_pred
 
-    def predict_proba(self, X, normalize=None, **kwargs) -> np.ndarray:
+    def predict_proba(self, X, *, normalize: bool | None = None, record_time: bool = False, **kwargs) -> np.ndarray:
         """
         Returns class prediction probabilities of X.
-        For binary problems, this returns the positive class label probability as a Series.
-        For multiclass problems, this returns the class label probabilities of each class as a DataFrame.
-        For regression problems, this returns the predicted values as a Series.
+        For binary problems, this returns the positive class label probability as a 1d numpy array.
+        For multiclass problems, this returns the class label probabilities of each class as a 2d numpy array.
+        For regression problems, this returns the predicted values as a 1d numpy array.
+
+        Parameters
+        ----------
+        X
+            The data used for prediction.
+        normalize: bool | None, default = None
+            Whether to normalize the predictions prior to returning.
+            If None, will default to `self.normalize_pred_probas`.
+        record_time: bool, default = False
+            If True, will record the time taken for prediction in `self.predict_time` and the number of rows of X in `self.predict_n_size`.
+        kwargs
+            Keyword arguments to pass into `self._predict_proba`.
+
+        Returns
+        -------
+        y_pred_proba : np.ndarray
+            The prediction probabilities
         """
+        time_start = time.time() if record_time else None
+
+        y_pred_proba = self._predict_proba_internal(X=X, normalize=normalize, **kwargs)
+
+        if self.params_aux.get("temperature_scalar", None) is not None:
+            y_pred_proba = self._apply_temperature_scaling(y_pred_proba)
+        elif self.conformalize is not None:
+            y_pred_proba = self._apply_conformalization(y_pred_proba)
+        if record_time:
+            self.predict_time = time.time() - time_start
+            self.record_predict_info(X=X)
+        return y_pred_proba
+
+    def _predict_proba_internal(self, X, *, normalize: bool | None = None, **kwargs):
         if normalize is None:
             normalize = self.normalize_pred_probas
         y_pred_proba = self._predict_proba(X=X, **kwargs)
         if normalize:
             y_pred_proba = normalize_pred_probas(y_pred_proba, self.problem_type)
         y_pred_proba = y_pred_proba.astype(np.float32)
-
-        if self.params_aux.get("temperature_scalar", None) is not None:
-            y_pred_proba = self._apply_temperature_scaling(y_pred_proba)
-        elif self.conformalize is not None:
-            y_pred_proba = self._apply_conformalization(y_pred_proba)
         return y_pred_proba
 
     def predict_from_proba(self, y_pred_proba: np.ndarray) -> np.ndarray:
         """
         Convert prediction probabilities to predictions.
 
         Parameters
@@ -1874,14 +1901,42 @@
         info = self.get_info()
 
         save_pkl.save(path=os.path.join(self.path, self.model_info_name), object=info)
         json_path = os.path.join(self.path, self.model_info_json_name)
         save_json.save(path=json_path, obj=info)
         return info
 
+    @property
+    def predict_n_size(self) -> int | None:
+        """
+        The number of rows in the data used when calculating `self.predict_time`.
+        """
+        return self._predict_n_size
+
+    @property
+    def predict_n_time_per_row(self) -> float | None:
+        """
+        The time in seconds required to predict 1 row of data given a batch size of `self.predict_n_size`.
+        Returns None if either `self.predict_time` or `self.predict_n_size` are None.
+        """
+        if self.predict_time is None or self.predict_n_size is None:
+            return None
+        return self.predict_time / self.predict_n_size
+
+    def record_predict_info(self, X: pd.DataFrame):
+        """
+        Records the necessary information to compute `self.predict_n_time_per_row`.
+
+        Parameters
+        ----------
+        X: pd.DataFrame
+            The data used to predict on when calculating `self.predict_time`.
+        """
+        self._predict_n_size = len(X)
+
     def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
         """
         Get the maximum resources allowed to use for this model.
         This can be useful when model not scale well with resources, i.e. cpu cores.
         Return empty dict if no maximum resources needed
 
         Return
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/abstract/model_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,21 +99,22 @@
     if model._get_tags().get("valid_oof", False):
         oof_pred_proba = model.predict_proba_oof(X=fit_args["X"], y=fit_args["y"])
         time_pred_end = time.time()
         # TODO: use sample_weight?
         # sample_weight = fit_args.get('sample_weight', None)
         model.val_score = model.score_with_y_pred_proba(y=fit_args["y"], y_pred_proba=oof_pred_proba)
     else:
-        y_pred_proba = model.predict_proba(**predict_proba_args)
+        y_pred_proba = model.predict_proba(record_time=True, **predict_proba_args)
         time_pred_end = time.time()
         sample_weight_val = fit_args.get("sample_weight_val", None)
         model.val_score = model.score_with_y_pred_proba(y=y_val, y_pred_proba=y_pred_proba, sample_weight=sample_weight_val)
 
     model.fit_time = time_fit_end - time_fit_start
-    model.predict_time = time_pred_end - time_fit_end
+    if model.predict_time is None:
+        model.predict_time = time_pred_end - time_fit_end
     model.save()
     return model
 
 
 def skip_hpo(model, X, y, X_val, y_val, time_limit=None, **kwargs):
     """Skips HPO and simply trains the model once with the provided HPO time budget. Returns model artifacts as if from HPO."""
     fit_model_args = dict(X=X, y=y, **kwargs)
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,16 @@
         # _child_oof currently is only set to True for KNN models, that are capable of LOO prediction generation to avoid needing bagging.
         # TODO: Consider moving `_child_oof` logic to a separate class / refactor OOF logic.
         # FIXME: Avoid unnecessary refit during refit_full on `_child_oof=True` models, just reuse the original model.
         self._child_oof = False  # Whether the OOF preds were taken from a single child model (Assumes child can produce OOF preds without bagging).
         self._cv_splitters = []  # Keeps track of the CV splitter used for each bagged repeat.
         self._params_aux_child = None  # aux params of child model
 
+        self._predict_n_size_lst = None  # A list of the predict row count for each child, useful to calculate the expected inference throughput of the bag.
+
         super().__init__(problem_type=self.model_base.problem_type, eval_metric=self.model_base.eval_metric, **kwargs)
 
     def _set_default_params(self):
         default_params = {
             # 'use_child_oof': False,  # [Advanced] Whether to defer to child model for OOF preds and only train a single child.
             "save_bag_folds": True,
             # 'refit_folds': False,  # [Advanced, Experimental] Whether to refit bags immediately to a refit_full model in a single .fit call.
@@ -444,31 +446,25 @@
         pred_children = []
         pred_children.append(model.predict(X=X, preprocess_nonadaptive=False, normalize=normalize))
         for model in children[1:]:
             model = self.load_child(model)
             pred_children.append(model.predict(X=X, preprocess_nonadaptive=False, normalize=normalize))
         return pred_children
 
-    def predict_proba(self, X, normalize=None, **kwargs):
+    def _predict_proba_internal(self, X, *, normalize: bool | None = None, **kwargs):
         model = self.load_child(self.models[0])
         X = self.preprocess(X, model=model, **kwargs)
-        pred_proba = model.predict_proba(X=X, preprocess_nonadaptive=False, normalize=normalize)
+        y_pred_proba = model.predict_proba(X=X, preprocess_nonadaptive=False, normalize=normalize)
         for model in self.models[1:]:
             model = self.load_child(model)
-            pred_proba += model.predict_proba(X=X, preprocess_nonadaptive=False, normalize=normalize)
-        pred_proba = pred_proba / self.n_children
-
-        if self.params_aux.get("temperature_scalar", None) is not None:
-            pred_proba = self._apply_temperature_scaling(pred_proba)
-        elif self.conformalize is not None:
-            pred_proba = self._apply_conformalization(pred_proba)
+            y_pred_proba += model.predict_proba(X=X, preprocess_nonadaptive=False, normalize=normalize)
+        y_pred_proba = y_pred_proba / self.n_children
+        return y_pred_proba
 
-        return pred_proba
-
-    def _predict_proba(self, X, normalize=False, **kwargs):
+    def _predict_proba(self, X, normalize=False, **kwargs) -> np.ndarray:
         return self.predict_proba(X=X, normalize=normalize, **kwargs)
 
     def score_with_oof(self, y, sample_weight=None):
         self._load_oof()
         valid_indices = self._oof_pred_model_repeats > 0
         y = y[valid_indices]
         y_pred_proba = self.predict_proba_oof()[valid_indices]
@@ -553,14 +549,15 @@
                         f"\tWARNING: Setting `self._oof_pred_proba` by predicting on train directly! "
                         f"This is probably a bug and should be investigated...\n"
                         f'\tIf this is intended, set the model tag "can_get_oof_from_train" to True '
                         f"in `{self.__class__.__name__}._more_tags` to avoid this warning.",
                     )
                 self._oof_pred_proba = model_base.predict_proba(X=X)  # TODO: Cheater value, will be overfit to valid set
             self._oof_pred_model_repeats = np.ones(shape=len(X), dtype=np.uint8)
+        model_base.record_predict_info(X=X)
         model_base.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
         if not self.params.get("save_bag_folds", True):
             model_base.model = None
         if self.low_memory:
             self.save_child(model_base)
         self.add_child(model=model_base, add_child_times=True)
         self._set_n_repeat_single()
@@ -1071,30 +1068,19 @@
     def _get_model_base(self):
         if self.model_base is None:
             return self.load_model_base()
         else:
             return self.model_base
 
     def _add_child_times_to_bag(self, model):
-        if self.fit_time is None:
-            self.fit_time = model.fit_time
-        else:
-            self.fit_time += model.fit_time
-
-        if self.predict_time is None:
-            self.predict_time = model.predict_time
-        else:
-            self.predict_time += model.predict_time
-
-        if self.predict_1_time is None:
-            self.predict_1_time = model.predict_1_time
-        else:
-            self.predict_1_time += model.predict_1_time
+        self._add_parallel_child_times(fit_time=model.fit_time, predict_time=model.predict_time, predict_1_time=model.predict_1_time)
+        assert model.predict_n_size is not None
+        self._add_predict_n_size(predict_n_size_lst=[model.predict_n_size])
 
-    def _add_parallel_child_times(self, fit_time, predict_time, predict_1_time):
+    def _add_parallel_child_times(self, fit_time: float, predict_time: float, predict_1_time: float):
         if self.fit_time is None:
             self.fit_time = fit_time
         else:
             self.fit_time += fit_time
 
         if self.predict_time is None:
             self.predict_time = predict_time
@@ -1102,14 +1088,27 @@
             self.predict_time += predict_time
 
         if self.predict_1_time is None:
             self.predict_1_time = predict_1_time
         else:
             self.predict_1_time += predict_1_time
 
+    def _add_predict_n_size(self, predict_n_size_lst: List[float]):
+        if self._predict_n_size_lst is None:
+            self._predict_n_size_lst = []
+        self._predict_n_size_lst += predict_n_size_lst
+
+    @property
+    def predict_n_size(self) -> float | None:
+        if self._predict_n_size is not None:
+            return self._predict_n_size
+        if not self._predict_n_size_lst:
+            return None
+        return np.ceil(np.mean(self._predict_n_size_lst))
+
     @classmethod
     def load(cls, path: str, reset_paths=True, low_memory=True, load_oof=False, verbose=True):
         model = super().load(path=path, reset_paths=reset_paths, verbose=verbose)
         if not low_memory:
             model.persist_child_models(reset_paths=reset_paths)
         if load_oof:
             model._load_oof()
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,37 +247,35 @@
             self.bagged_ensemble_model.save_child(fold_model, verbose=False)
             model_to_append = fold_model.name
         self.models.append(model_to_append)
         self.oof_pred_proba[val_index] += pred_proba
         self.oof_pred_model_repeats[val_index] += 1
         self.bagged_ensemble_model._add_child_times_to_bag(model=fold_model)
 
-    def _predict_oof(self, fold_model, fold_ctx):
-        time_train_end_fold = time.time()
+    def _predict_oof(self, fold_model: AbstractModel, fold_ctx) -> Tuple[AbstractModel, ndarray]:
         fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = self._get_fold_properties(fold_ctx)
         _, val_index = fold
         X_val_fold = self.X.iloc[val_index, :]
         y_val_fold = self.y.iloc[val_index]
         # Check to avoid unnecessarily predicting and saving a model
         # when an Exception is going to be raised later
         if self.time_limit is not None:
             if not is_last_fold:
                 time_elapsed = time.time() - self.time_start
                 time_left = self.time_limit - time_elapsed
                 expected_time_required = time_elapsed * folds_to_fit / (folds_finished + 1)
                 expected_remaining_time_required = expected_time_required * (folds_left - 1) / folds_to_fit
                 if expected_remaining_time_required > time_left:
                     raise TimeLimitExceeded
-        pred_proba = fold_model.predict_proba(X_val_fold)
-        fold_model.predict_time = time.time() - time_train_end_fold
-        fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold, y_pred_proba=pred_proba)
+        y_pred_proba = fold_model.predict_proba(X_val_fold, record_time=True)
+        fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold, y_pred_proba=y_pred_proba)
         fold_model.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
         if not self.bagged_ensemble_model.params.get("save_bag_folds", True):
             fold_model.model = None
-        return fold_model, pred_proba
+        return fold_model, y_pred_proba
 
     @staticmethod
     def _get_fold_properties(fold_ctx):
         fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = [
             fold_ctx[f] for f in ["fold", "folds_finished", "folds_left", "folds_to_fit", "is_last_fold", "model_name_suffix"]
         ]
         return fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix
@@ -400,32 +398,36 @@
     if is_pseudo:
         logger.log(15, f"{len(X_pseudo)} extra rows of pseudolabeled data added to training set for {fold_model.name}")
         X_fold = pd.concat([X_fold, X_pseudo], axis=0, ignore_index=True)
         y_fold = pd.concat([y_fold, y_pseudo], axis=0, ignore_index=True)
     fold_model.fit(X=X_fold, y=y_fold, X_val=X_val_fold, y_val=y_val_fold, time_limit=time_limit_fold, **resources, **kwargs_fold)
     time_train_end_fold = time.time()
     fold_model.fit_time = time_train_end_fold - time_start_fold
-    fold_model, pred_proba = _ray_predict_oof(fold_model, X_val_fold, y_val_fold, time_train_end_fold, resources["num_cpus"], save_bag_folds)
+    fold_model, pred_proba = _ray_predict_oof(
+        fold_model=fold_model,
+        X_val_fold=X_val_fold,
+        y_val_fold=y_val_fold,
+        num_cpus=resources["num_cpus"],
+        save_bag_folds=save_bag_folds,
+    )
     save_path = fold_model.save()
     if model_sync_path is not None and not is_head_node:
         model_sync_path = model_sync_path + f"{fold_model.name}/"  # s3 path hence need "/" as the saperator
         bucket, prefix = s3_path_to_bucket_prefix(model_sync_path)
         upload_s3_folder(bucket=bucket, prefix=prefix, folder_to_upload=save_path, verbose=False)
-    return fold_model.name, pred_proba, time_start_fold, time_train_end_fold, fold_model.predict_time, fold_model.predict_1_time
+    return fold_model.name, pred_proba, time_start_fold, time_train_end_fold, fold_model.predict_time, fold_model.predict_1_time, fold_model.predict_n_size
 
 
-def _ray_predict_oof(fold_model, X_val_fold, y_val_fold, time_train_end_fold, num_cpus=-1, save_bag_folds=True):
-    pred_proba = fold_model.predict_proba(X_val_fold, num_cpus=num_cpus)
-    time_pred_end_fold = time.time()
-    fold_model.predict_time = time_pred_end_fold - time_train_end_fold
-    fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold, y_pred_proba=pred_proba)
+def _ray_predict_oof(fold_model: AbstractModel, X_val_fold: pd.DataFrame, y_val_fold: pd.Series, num_cpus: int = -1, save_bag_folds: bool = True):
+    y_pred_proba = fold_model.predict_proba(X_val_fold, record_time=True, num_cpus=num_cpus)
+    fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold, y_pred_proba=y_pred_proba)
     fold_model.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
     if not save_bag_folds:
         fold_model.model = None
-    return fold_model, pred_proba
+    return fold_model, y_pred_proba
 
 
 class ParallelFoldFittingStrategy(FoldFittingStrategy):
     """
     An implementation of FoldFittingStrategy to train multiple folds in parallel.
     Folds are spread to cpu/gpu cores by ray tasks.
     Large data are stored in ray object store, which minimizes memory usage and unessary serializations.
@@ -469,14 +471,15 @@
         self.max_memory_usage_ratio = max_memory_usage_ratio
         self.model_sync_path = model_sync_path
         self.time_start_fit = None
         self.time_end_fit = None
         self.fit_time = 0
         self.predict_time = 0
         self.predict_1_time = None
+        self.predict_n_size_lst = None
         # max_calls to guarantee release of gpu resource
         self._ray_fit = self.ray.remote(max_calls=1)(_ray_fit)
         self.mem_est_model = self._initialized_model_base.estimate_memory_usage(X=self.X)
         self.mem_est_data = self._estimate_data_memory_usage()
         self.mem_available = ResourceManager.get_available_virtual_mem()
         num_folds_parallel = self.folds_to_fit_in_parallel_with_mem(user_specified_num_folds_parallel=num_folds_parallel)
         self._pseudo_sequential: bool = num_folds_parallel == 1
@@ -527,23 +530,24 @@
         Get the arguments needed to init ray runtime.
         This could differ in different context, i.e. distributed vs local
         """
         return dict(address="auto", logging_level=logging.ERROR, log_to_driver=False)
 
     def _process_fold_results(self, finished, unfinished, fold_ctx):
         try:
-            fold_model, pred_proba, time_start_fit, time_end_fit, predict_time, predict_1_time = self.ray.get(finished)
+            fold_model, pred_proba, time_start_fit, time_end_fit, predict_time, predict_1_time, predict_n_size = self.ray.get(finished)
             assert fold_ctx is not None
             self._update_bagged_ensemble(
                 fold_model=fold_model,
                 pred_proba=pred_proba,
                 time_start_fit=time_start_fit,
                 time_end_fit=time_end_fit,
                 predict_time=predict_time,
                 predict_1_time=predict_1_time,
+                predict_n_size=predict_n_size,
                 fold_ctx=fold_ctx,
             )
             model_sync_path = None
             if self.model_sync_path is not None:
                 model_sync_path: str = self.model_sync_path + fold_model
                 if not model_sync_path.endswith("/"):
                     model_sync_path += "/"
@@ -568,14 +572,15 @@
             raise processed_exception
 
     def _update_bagged_ensemble_times(self):
         self.fit_time = 0
         if self.time_start_fit and self.time_end_fit:
             self.fit_time = self.time_end_fit - self.time_start_fit
         self.bagged_ensemble_model._add_parallel_child_times(fit_time=self.fit_time, predict_time=self.predict_time, predict_1_time=self.predict_1_time)
+        self.bagged_ensemble_model._add_predict_n_size(predict_n_size_lst=self.predict_n_size_lst)
 
     def _run_parallel(self, X, y, X_pseudo, y_pseudo, model_base_ref, time_limit_fold, head_node_id):
         job_refs = []
         job_fold_map = {}
 
         # spread the task
         for job in self.jobs:
@@ -712,15 +717,15 @@
             save_bag_folds=save_bag_folds,
             resources=resources_model,
             kwargs_fold=kwargs_fold,
             head_node_id=head_node_id,
             model_sync_path=self.model_sync_path,
         )
 
-    def _update_bagged_ensemble(self, fold_model, pred_proba, time_start_fit, time_end_fit, predict_time, predict_1_time, fold_ctx):
+    def _update_bagged_ensemble(self, fold_model, pred_proba, time_start_fit, time_end_fit, predict_time, predict_1_time, predict_n_size, fold_ctx):
         _, val_index = fold_ctx["fold"]
         self.models.append(fold_model)
         self.oof_pred_proba[val_index] += pred_proba
         self.oof_pred_model_repeats[val_index] += 1
         if self.time_start_fit:
             self.time_start_fit = min(time_start_fit, self.time_start_fit)
         else:
@@ -730,14 +735,17 @@
         else:
             self.time_end_fit = time_end_fit
         self.predict_time += predict_time
         if predict_1_time is not None:
             if self.predict_1_time is None:
                 self.predict_1_time = 0
             self.predict_1_time += predict_1_time
+        if self.predict_n_size_lst is None:
+            self.predict_n_size_lst = []
+        self.predict_n_size_lst.append(predict_n_size)
 
     def _get_fold_time_limit(self):
         time_elapsed = time.time() - self.time_start
         if self.time_limit is not None:
             time_left = self.time_limit - time_elapsed
             required_time_per_fold = time_left / self.batches
             time_limit_fold = required_time_per_fold * self.time_limit_fold_ratio
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/problem_type.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/stacked_overfitting/utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/stacked_overfitting/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1909,36 +1909,29 @@
                 w_val = model_fit_kwargs.get("sample_weight_val", None)
             else:
                 w = None
                 w_val = None
             if not compute_score:
                 score = None
                 model.predict_time = None
+            elif X_val is not None and y_val is not None:
+                y_pred_proba_val = model.predict_proba(X_val, record_time=True)
+                score = model.score_with_y_pred_proba(y=y_val, y_pred_proba=y_pred_proba_val, sample_weight=w_val)
             elif isinstance(model, BaggedEnsembleModel):
-                if X_val is not None and y_val is not None:
-                    y_pred_proba_val = model.predict_proba(X_val)
-                    score = model.score_with_y_pred_proba(y=y_val, y_pred_proba=y_pred_proba_val, sample_weight=w_val)
-                elif model.is_valid_oof() or isinstance(model, WeightedEnsembleModel):
+                if model.is_valid_oof() or isinstance(model, WeightedEnsembleModel):
                     score = model.score_with_oof(y=y, sample_weight=w)
                 else:
                     score = None
             else:
-                if X_val is not None and y_val is not None:
-                    y_pred_proba_val = model.predict_proba(X_val)
-                    score = model.score_with_y_pred_proba(y=y_val, y_pred_proba=y_pred_proba_val, sample_weight=w_val)
-                else:
-                    score = None
+                score = None
             pred_end_time = time.time()
             if model.fit_time is None:
                 model.fit_time = fit_end_time - fit_start_time
-            if model.predict_time is None:
-                if score is None:
-                    model.predict_time = None
-                else:
-                    model.predict_time = pred_end_time - fit_end_time
+            if model.predict_time is None and score is not None:
+                model.predict_time = pred_end_time - fit_end_time
             model.val_score = score
             # TODO: Add recursive=True to avoid repeatedly loading models each time this is called for bagged ensembles (especially during repeated bagging)
             self.save_model(model=model)
         except Exception as err:
             del_model = True
             if isinstance(err, TimeLimitExceeded):
                 logger.log(20, f"\tTime limit exceeded... Skipping {model.name}.")
@@ -1999,14 +1992,16 @@
         model_metadata = dict(
             fit_time=model.fit_time,
             compile_time=model.compile_time,
             predict_time=model.predict_time,
             predict_1_time=model.predict_1_time,
             predict_child_time=predict_child_time,
             predict_1_child_time=predict_1_child_time,
+            predict_n_time_per_row=model.predict_n_time_per_row,
+            predict_n_size=model.predict_n_size,
             val_score=model.val_score,
             eval_metric=model.eval_metric.name,
             stopping_metric=model.stopping_metric.name,
             path=os.path.relpath(model.path, self.path).split(os.sep),  # model's relative path to trainer
             type=type(model),  # Outer type, can be BaggedEnsemble, StackEnsemble (Type that is able to load the model)
             type_inner=type_inner,  # Inner type, if Ensemble then it is the type of the inner model (May not be able to load with this type)
             can_infer=model.can_infer(),
@@ -2125,14 +2120,18 @@
             else:
                 sign_str = ""
             logger.log(20, f"\t{round(model.val_score, 4)}\t = Validation score   ({sign_str}{model.eval_metric.name})")
         if model.fit_time is not None:
             logger.log(20, f"\t{round(model.fit_time, 2)}s\t = Training   runtime")
         if model.predict_time is not None:
             logger.log(20, f"\t{round(model.predict_time, 2)}s\t = Validation runtime")
+        predict_n_time_per_row = self.get_model_attribute_full(model=model.name, attribute="predict_n_time_per_row")
+        predict_n_size = self.get_model_attribute_full(model=model.name, attribute="predict_n_size", func=min)
+        if predict_n_time_per_row is not None and predict_n_time_per_row != 0 and predict_n_size is not None:
+            logger.log(30, f"\t{round(1 / predict_n_time_per_row, 1)}\t = Inference  throughput (rows/s | {int(predict_n_size)} batch size)")
         if model.predict_1_time is not None:
             fit_metadata = model.get_fit_metadata()
             predict_1_batch_size = fit_metadata.get("predict_1_batch_size", None)
             assert predict_1_batch_size is not None, "predict_1_batch_size cannot be None if predict_1_time is not None"
 
             if _is_refit:
                 predict_1_time = self.get_model_attribute(model=model.name, attribute="predict_1_child_time")
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/trainer/utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/decorators.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/files.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/plots.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/time.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,16 +628,16 @@
             y_min = y.min()
             y_mean = y.mean()
             y_stddev = y.std()
             logger.log(20, f"\tLabel info (max, min, mean, stddev): ({y_max}, {y_min}, {round(y_mean, 5)}, {round(y_stddev, 5)})")
 
         logger.log(
             25,
-            f"\tIf '{problem_type}' is not the correct problem_type, please manually specify the problem_type parameter during predictor init "
-            f"(You may specify problem_type as one of: {[BINARY, MULTICLASS, REGRESSION]})",
+            f"\tIf '{problem_type}' is not the correct problem_type, please manually specify the problem_type parameter during Predictor init "
+            f"(You may specify problem_type as one of: {[BINARY, MULTICLASS, REGRESSION, QUANTILE]})",
         )
     return problem_type
 
 
 def infer_eval_metric(problem_type: str) -> Scorer:
     """Infers appropriate default eval metric based on problem_type. Useful when no eval_metric was provided."""
     if problem_type == BINARY:
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon/core/utils/version_utils.py` & `autogluon.core-1.1.1b20240517/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.1.1b20240516
+Version: 1.1.1b20240517
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-1.1.1b20240516/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-1.1.1b20240517/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*


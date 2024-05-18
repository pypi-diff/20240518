# Comparing `tmp/remodels-0.2.0.tar.gz` & `tmp/remodels-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remodels-0.2.0.tar", max compression
+gzip compressed data, was "remodels-1.0.0.tar", max compression
```

## Comparing `remodels-0.2.0.tar` & `remodels-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1096 2023-12-19 22:06:42.622027 remodels-0.2.0/LICENSE
--rw-r--r--   0        0        0     2076 2023-12-19 22:06:42.622027 remodels-0.2.0/README.md
--rw-r--r--   0        0        0     1993 2023-12-19 22:06:52.926046 remodels-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       16 2023-12-19 22:06:42.626026 remodels-0.2.0/src/remodels/__init__.py
--rw-r--r--   0        0        0      206 2023-12-19 22:06:42.626026 remodels-0.2.0/src/remodels/__main__.py
--rw-r--r--   0        0        0     9917 2023-12-19 22:06:42.626026 remodels-0.2.0/src/remodels/data/EntsoeApi.py
--rw-r--r--   0        0        0       55 2023-12-19 22:06:42.626026 remodels-0.2.0/src/remodels/data/__init__.py
--rw-r--r--   0        0        0     5372 2023-12-19 22:06:42.626026 remodels-0.2.0/src/remodels/pipelines/RePipeline.py
--rw-r--r--   0        0        0       62 2023-12-19 22:06:42.626026 remodels-0.2.0/src/remodels/pipelines/__init__.py
--rw-r--r--   0        0        0    10250 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/pointsModels/PointModel.py
--rw-r--r--   0        0        0       65 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/pointsModels/__init__.py
--rw-r--r--   0        0        0        0 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/py.typed
--rw-r--r--   0        0        0      383 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/__init__.py
--rw-r--r--   0        0        0     2654 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/_functions.py
--rw-r--r--   0        0        0     1253 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/_linear_model.py
--rw-r--r--   0        0        0      948 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/_lstsq.py
--rw-r--r--   0        0        0     3081 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/fqra.py
--rw-r--r--   0        0        0     2253 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/fqrm.py
--rw-r--r--   0        0        0     1502 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/lqra.py
--rw-r--r--   0        0        0     1415 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/qra.py
--rw-r--r--   0        0        0     1310 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/qrm.py
--rw-r--r--   0        0        0     1854 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/sfqra.py
--rw-r--r--   0        0        0     1584 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/sfqrm.py
--rw-r--r--   0        0        0     1676 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/sqra.py
--rw-r--r--   0        0        0     1422 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/sqrm.py
--rw-r--r--   0        0        0      207 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/tester/__init__.py
--rw-r--r--   0        0        0     6303 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/tester/qr_results_summary.py
--rw-r--r--   0        0        0    12970 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/qra/tester/qr_tester.py
--rw-r--r--   0        0        0     3137 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/BaseScaler.py
--rw-r--r--   0        0        0     2493 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/DSTAdjuster.py
--rw-r--r--   0        0        0     5791 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/StandardizingScaler.py
--rw-r--r--   0        0        0     2108 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/ArcsinhScaler.py
--rw-r--r--   0        0        0     3515 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/BoxCoxScaler.py
--rw-r--r--   0        0        0     3707 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/ClippingScaler.py
--rw-r--r--   0        0        0     3349 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/LogClippingScaler.py
--rw-r--r--   0        0        0     2464 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/LogisticScaler.py
--rw-r--r--   0        0        0     2880 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/MLogScaler.py
--rw-r--r--   0        0        0     5626 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/PITScaler.py
--rw-r--r--   0        0        0     3287 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/PolyScaler.py
--rw-r--r--   0        0        0      363 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/VSTransformers/__init__.py
--rw-r--r--   0        0        0       83 2023-12-19 22:06:42.630026 remodels-0.2.0/src/remodels/transformers/__init__.py
--rw-r--r--   0        0        0     3211 2023-12-19 22:06:54.932697 remodels-0.2.0/setup.py
--rw-r--r--   0        0        0     3020 2023-12-19 22:06:54.933025 remodels-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-18 17:11:03.947711 remodels-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3157 2024-05-18 17:11:03.947711 remodels-1.0.0/README.md
+-rw-r--r--   0        0        0     1990 2024-05-18 17:11:14.547842 remodels-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/__main__.py
+-rw-r--r--   0        0        0     9983 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/data/EntsoeApi.py
+-rw-r--r--   0        0        0       55 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/data/__init__.py
+-rw-r--r--   0        0        0     5372 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/pipelines/RePipeline.py
+-rw-r--r--   0        0        0       62 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/pipelines/__init__.py
+-rw-r--r--   0        0        0    10501 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/pointsModels/PointModel.py
+-rw-r--r--   0        0        0       65 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/pointsModels/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/py.typed
+-rw-r--r--   0        0        0      383 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/qra/__init__.py
+-rw-r--r--   0        0        0     2654 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/qra/_functions.py
+-rw-r--r--   0        0        0     1253 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/qra/_linear_model.py
+-rw-r--r--   0        0        0      948 2024-05-18 17:11:03.951712 remodels-1.0.0/src/remodels/qra/_lstsq.py
+-rw-r--r--   0        0        0     3081 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/fqra.py
+-rw-r--r--   0        0        0     2253 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/fqrm.py
+-rw-r--r--   0        0        0     1502 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/lqra.py
+-rw-r--r--   0        0        0     1415 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/qra.py
+-rw-r--r--   0        0        0     1310 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/qrm.py
+-rw-r--r--   0        0        0     1854 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/sfqra.py
+-rw-r--r--   0        0        0     1584 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/sfqrm.py
+-rw-r--r--   0        0        0     1676 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/sqra.py
+-rw-r--r--   0        0        0     1422 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/sqrm.py
+-rw-r--r--   0        0        0      207 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/tester/__init__.py
+-rw-r--r--   0        0        0     6303 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/tester/qr_results_summary.py
+-rw-r--r--   0        0        0    12975 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/qra/tester/qr_tester.py
+-rw-r--r--   0        0        0     3137 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/BaseScaler.py
+-rw-r--r--   0        0        0     2493 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/DSTAdjuster.py
+-rw-r--r--   0        0        0     5791 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/StandardizingScaler.py
+-rw-r--r--   0        0        0     2108 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/ArcsinhScaler.py
+-rw-r--r--   0        0        0     3515 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/BoxCoxScaler.py
+-rw-r--r--   0        0        0     3707 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/ClippingScaler.py
+-rw-r--r--   0        0        0     3349 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/LogClippingScaler.py
+-rw-r--r--   0        0        0     2464 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/LogisticScaler.py
+-rw-r--r--   0        0        0     2880 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/MLogScaler.py
+-rw-r--r--   0        0        0     5626 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/PITScaler.py
+-rw-r--r--   0        0        0     3287 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/PolyScaler.py
+-rw-r--r--   0        0        0      363 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/VSTransformers/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-18 17:11:03.955711 remodels-1.0.0/src/remodels/transformers/__init__.py
+-rw-r--r--   0        0        0     4318 2024-05-18 17:11:16.532596 remodels-1.0.0/setup.py
+-rw-r--r--   0        0        0     4098 2024-05-18 17:11:16.532991 remodels-1.0.0/PKG-INFO
```

### Comparing `remodels-0.2.0/LICENSE` & `remodels-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/pyproject.toml` & `remodels-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "remodels"
-version = "0.2.0"
+version = "1.0.0"
 description = "remodels"
 authors = ["Grzegorz Zakrzewski <zakrzew12@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zakrzewow/remodels"
 repository = "https://github.com/zakrzewow/remodels"
 documentation = "https://remodels.readthedocs.io"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/zakrzewow/remodels/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `remodels-0.2.0/src/remodels/data/EntsoeApi.py` & `remodels-1.0.0/src/remodels/data/EntsoeApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,19 @@
             except requests.HTTPError as e:
                 self.logger.error(f"Failed to retrieve data: {e}")
                 break
             except Exception as e:
                 self.logger.error(f"An unexpected error occurred: {e}")
                 break
 
-        return pd.DataFrame(data).set_index("datetime") if data else pd.DataFrame()
+        return (
+            pd.DataFrame(data).set_index("datetime").tz_localize(None)
+            if data
+            else pd.DataFrame()
+        )
 
     def _parse_production_and_load_data(self, content: str) -> list:
         """Parses the production and load data from the API's XML response.
 
         :param content: XML content to parse.
         :type content: str
         :return: List of dictionaries containing production and load data.
```

### Comparing `remodels-0.2.0/src/remodels/pipelines/RePipeline.py` & `remodels-1.0.0/src/remodels/pipelines/RePipeline.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/pointsModels/PointModel.py` & `remodels-1.0.0/src/remodels/pointsModels/PointModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """PointModel."""
+
 import datetime as dt
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_squared_error
 from sklearn.metrics import r2_score
@@ -15,15 +16,15 @@
 
     This model is equipped with a flexible data processing pipeline and the ability to handle different sets
     of predictor variables for different hours of the day. It offers functionality for model training,
     prediction with a rolling window approach, and calculation of various evaluation metrics.
     """
 
     def __init__(
-        self, pipeline: RePipeline, variables_per_hour: dict, y_column="price_da"
+        self, pipeline: RePipeline, variables_per_hour: dict = {}, y_column="price_da"
     ):
         """Initialize the PointModel with a data processing pipeline, variables mapped to each hour, and the target column name.
 
         :param pipeline: Sequence of data transformation steps and a predictive model.
         :type pipeline: RePipeline
         :param variables_per_hour: Mapping from hour ranges to the variables to be used in those hours.
         :type variables_per_hour: dict
@@ -141,14 +142,16 @@
         :param predictions_list: List to store the predictions.
         :type predictions_list: list
         :param inverse_predictions: Flag to determine whether to apply inverse transformation to predictions.
         :type inverse_predictions: bool
         """
         for hour in self.unique_hours:
             hour_variables = self.get_hour_variables(hour)
+            if hour_variables is None:
+                hour_variables = self.all_used_columns
             Xy_train_hour = Xy_train.loc[Xy_train.index.hour == hour]
             X_test_hour = Xy_test.loc[Xy_test.index.hour == hour][hour_variables]
             Xy_train_hour, y_train_hour = self.fit_transform_data(
                 Xy_train_hour[hour_variables + self.y_column]
             )
             X_test_hour = self.fit_transform_data(
                 X_test_hour[hour_variables], is_train=False
@@ -163,54 +166,56 @@
                     _, prediction_df = self.transformation_pipeline.inverse_transform(
                         yt=prediction[0]
                     )
                     predictions_list.append((date_, prediction_df[0]))
                 elif len(prediction) > 0:
                     predictions_list.append((date_, prediction[0, 0]))
 
-    def predict(self, rolling_window: int = 728, inverse_predictions: bool = True):
+    def predict(self, calibration_window: int = 728, inverse_predictions: bool = True):
         """Predict values over a given range, from start to end, using a rolling window, and store/update predictions in the model.
 
         :param df: DataFrame containing the data to be used for prediction.
         :type df: pd.DataFrame
-        :param rolling_window: Number of days to look back for training data.
-        :type rolling_window: int
+        :param calibration_window: Number of days to look back for training data.
+        :type calibration_window: int
         :param inverse_predictions: Flag to determine whether to apply inverse transformation to predictions.
         :type inverse_predictions: bool
         :return: DataFrame of predicted values.
         :rtype: pd.DataFrame
         """
         df = self.training_data
+        if not len(self.all_used_columns):
+            self.all_used_columns = df.drop(columns=self.y_column).columns.tolist()
         predictions_list = []
         for day in pd.date_range(self.start, self.end, freq="D"):
             Xy_train = df.loc[
-                (df.index.date >= day.date() - dt.timedelta(days=rolling_window))
+                (df.index.date >= day.date() - dt.timedelta(days=calibration_window))
                 & (df.index.date < day.date())
             ][self.all_used_columns + self.y_column].dropna()
             Xy_test = df.loc[df.index.date == day.date()][
                 self.all_used_columns + self.y_column
             ].dropna()
             self.train_and_predict_hours(
                 day, Xy_train, Xy_test, predictions_list, inverse_predictions
             )
 
         new_predictions_df = pd.DataFrame(
-            predictions_list, columns=["DateTime", f"prediction_{rolling_window}rw"]
+            predictions_list, columns=["DateTime", f"prediction_{calibration_window}rw"]
         )
         new_predictions_df.set_index("DateTime", inplace=True)
 
         if (
             self.predictions is not None
             and new_predictions_df.columns[0] not in self.predictions.columns
         ):
             self.predictions = self.predictions.join(new_predictions_df, how="outer")
         else:
             self.predictions = new_predictions_df
 
-        return self.predictions[[f"prediction_{rolling_window}rw"]]
+        return self.predictions[[f"prediction_{calibration_window}rw"]]
 
     def calculate_metrics(self, y_true: pd.DataFrame, y_pred: pd.DataFrame):
         """Calculate regression metrics.
 
         :param y_true: DataFrame containing the actual data
         :type y_pred: pd.DataFrame
         :param y_pred: DataFrame containing the predicted data
```

### Comparing `remodels-0.2.0/src/remodels/qra/_functions.py` & `remodels-1.0.0/src/remodels/qra/_functions.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/_linear_model.py` & `remodels-1.0.0/src/remodels/qra/_linear_model.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/_lstsq.py` & `remodels-1.0.0/src/remodels/qra/_lstsq.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/fqra.py` & `remodels-1.0.0/src/remodels/qra/fqra.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/fqrm.py` & `remodels-1.0.0/src/remodels/qra/fqrm.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/lqra.py` & `remodels-1.0.0/src/remodels/qra/lqra.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/qra.py` & `remodels-1.0.0/src/remodels/qra/qra.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/qrm.py` & `remodels-1.0.0/src/remodels/qra/qrm.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/sfqra.py` & `remodels-1.0.0/src/remodels/qra/sfqra.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/sfqrm.py` & `remodels-1.0.0/src/remodels/qra/sfqrm.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/sqra.py` & `remodels-1.0.0/src/remodels/qra/sqra.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/sqrm.py` & `remodels-1.0.0/src/remodels/qra/sqrm.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/tester/qr_results_summary.py` & `remodels-1.0.0/src/remodels/qra/tester/qr_results_summary.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/qra/tester/qr_tester.py` & `remodels-1.0.0/src/remodels/qra/tester/qr_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         multivariate: bool = True,
         qr_model=_default_qr_model,
         max_workers: int = None,
         progress: bool = True,
     ) -> None:
         """Initialize the QR Tester.
 
-        :param calibration_window: length of calibration window, defaults to 14
+        :param calibration_window: length of calibration window, defaults to 7 * 24
         :type calibration_window: int, optional
-        :param prediction_window: length of prediction window, defaults to 1
+        :param prediction_window: length of prediction window, defaults to 24
         :type prediction_window: int, optional
         :param qr_model: *QR* model, defaults to QRA(fit_intercept=True)
         :type qr_model: QRA, optional
         :param max_workers: process pool executor max workers, defaults to None
         :type max_workers: int, optional
         """
         self.calibration_window = calibration_window
```

### Comparing `remodels-0.2.0/src/remodels/transformers/BaseScaler.py` & `remodels-1.0.0/src/remodels/transformers/BaseScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/DSTAdjuster.py` & `remodels-1.0.0/src/remodels/transformers/DSTAdjuster.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/StandardizingScaler.py` & `remodels-1.0.0/src/remodels/transformers/StandardizingScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/ArcsinhScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/ArcsinhScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/BoxCoxScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/BoxCoxScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/ClippingScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/ClippingScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/LogClippingScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/LogClippingScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/LogisticScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/LogisticScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/MLogScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/MLogScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/PITScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/PITScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/src/remodels/transformers/VSTransformers/PolyScaler.py` & `remodels-1.0.0/src/remodels/transformers/VSTransformers/PolyScaler.py`

 * *Files identical despite different names*

### Comparing `remodels-0.2.0/PKG-INFO` & `remodels-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: remodels
-Version: 0.2.0
-Summary: remodels
-Home-page: https://github.com/zakrzewow/remodels
-License: MIT
-Author: Grzegorz Zakrzewski
-Author-email: zakrzew12@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=8.0.1)
-Requires-Dist: matplotlib (>=3.7.0,<3.8.0)
-Requires-Dist: pandas (<=1.5.3)
-Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
-Requires-Dist: tqdm (>=4.66.1,<5.0.0)
-Project-URL: Changelog, https://github.com/zakrzewow/remodels/releases
-Project-URL: Documentation, https://remodels.readthedocs.io
-Project-URL: Repository, https://github.com/zakrzewow/remodels
-Description-Content-Type: text/markdown
-
 # remodels
 
 [![PyPI](https://img.shields.io/pypi/v/remodels.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/remodels.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/remodels)][python version]
 [![License](https://img.shields.io/pypi/l/remodels)][license]
 
@@ -42,14 +17,39 @@
 [python version]: https://pypi.org/project/remodels
 [read the docs]: https://remodels.readthedocs.io/en/latest/
 [tests]: https://github.com/zakrzewow/remodels/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/zakrzewow/remodels
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
+ReModels is a Python package for probabilistic energy price forecasting using eight Quantile Regression Averaging (QRA) methods.
+
+### Features
+
+- **Dataset Download**: access commonly used public datasets for transparent data acquisition.
+- **Data Preprocessing**: apply variance stabilizing transformation for improved data quality.
+- **Forecast Generation**: produce point and probabilistic forecasts with reference implementations of QRA variants.
+- **Result Evaluation**: compare predictions using dedicated metrics for fair and consistent evaluation.
+
+ReModels provides a robust framework for researchers to compare different QRA methods and other forecasting techniques. It supports the development of new forecasting methods, extending beyond energy price forecasting.
+
+ReModels simplifies and enhances energy price forecasting research with comprehensive tools and transparent methodologies.
+
+Implemented QRA variants:
+
+- QRA
+- QRM
+- FQRA
+- FQRM
+- sFQRA
+- sFQRM
+- LQRA
+- SQRA
+- SQRM
+
 ## Installation
 
 You can install _remodels_ via [pip] from [PyPI]:
 
 ```console
 $ pip install remodels
 ```
@@ -60,15 +60,15 @@
 $ git clone https://github.com/zakrzewow/remodels.git
 $ cd remodels
 $ pip install .
 ```
 
 ## Usage
 
-Please see the [Usage] for details.
+Please see the [Usage] or the [Reference] for details.
 
 ## License
 
 Distributed under the terms of the [MIT license][license],
 _remodels_ is free and open source software.
 
 ## Credits
@@ -80,8 +80,8 @@
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
 [license]: https://github.com/zakrzewow/remodels/blob/main/LICENSE
 [usage]: https://remodels.readthedocs.io/en/latest/usage.html
-
+[reference]: https://remodels.readthedocs.io/en/latest/reference.html
```


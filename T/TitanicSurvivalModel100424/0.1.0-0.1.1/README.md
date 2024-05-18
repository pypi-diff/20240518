# Comparing `tmp/TitanicSurvivalModel100424-0.1.0.tar.gz` & `tmp/titanicsurvivalmodel100424-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TitanicSurvivalModel100424-0.1.0.tar", last modified: Fri May 10 07:40:27 2024, max compression
+gzip compressed data, was "titanicsurvivalmodel100424-0.1.1.tar", last modified: Sat May 18 07:36:23 2024, max compression
```

## Comparing `TitanicSurvivalModel100424-0.1.0.tar` & `titanicsurvivalmodel100424-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.124481 TitanicSurvivalModel100424-0.1.0/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      482 2024-05-09 06:18:45.000000 TitanicSurvivalModel100424-0.1.0/MANIFEST.in
--rw-r--r--   0 ongzhicong   (501) staff       (20)      830 2024-05-10 07:40:27.124231 TitanicSurvivalModel100424-0.1.0/PKG-INFO
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.118791 TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      830 2024-05-10 07:40:26.000000 TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/PKG-INFO
--rw-r--r--   0 ongzhicong   (501) staff       (20)      899 2024-05-10 07:40:27.000000 TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/SOURCES.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-10 07:40:26.000000 TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/dependency_links.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)      195 2024-05-10 07:40:26.000000 TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/requires.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-10 07:40:26.000000 TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/top_level.txt
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.121351 TitanicSurvivalModel100424-0.1.0/classification_model/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-10 01:46:12.000000 TitanicSurvivalModel100424-0.1.0/classification_model/VERSION
--rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 TitanicSurvivalModel100424-0.1.0/classification_model/__init__.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.121951 TitanicSurvivalModel100424-0.1.0/classification_model/config/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 TitanicSurvivalModel100424-0.1.0/classification_model/config/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2078 2024-05-08 07:20:27.000000 TitanicSurvivalModel100424-0.1.0/classification_model/config/core.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      702 2024-05-10 06:30:56.000000 TitanicSurvivalModel100424-0.1.0/classification_model/config.yml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.122306 TitanicSurvivalModel100424-0.1.0/classification_model/datasets/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 TitanicSurvivalModel100424-0.1.0/classification_model/datasets/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1958 2024-05-04 09:20:40.000000 TitanicSurvivalModel100424-0.1.0/classification_model/pipeline.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1072 2024-05-10 06:10:01.000000 TitanicSurvivalModel100424-0.1.0/classification_model/predict.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.123577 TitanicSurvivalModel100424-0.1.0/classification_model/processing/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 TitanicSurvivalModel100424-0.1.0/classification_model/processing/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     2671 2024-05-10 06:02:13.000000 TitanicSurvivalModel100424-0.1.0/classification_model/processing/data_manager.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      630 2024-05-10 06:30:35.000000 TitanicSurvivalModel100424-0.1.0/classification_model/processing/features.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1898 2024-05-07 08:31:39.000000 TitanicSurvivalModel100424-0.1.0/classification_model/processing/validation.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)      818 2024-05-07 08:32:04.000000 TitanicSurvivalModel100424-0.1.0/classification_model/train_pipeline.py
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.123929 TitanicSurvivalModel100424-0.1.0/classification_model/trained_models/
--rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 TitanicSurvivalModel100424-0.1.0/classification_model/trained_models/__init__.py
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 TitanicSurvivalModel100424-0.1.0/pyproject.toml
-drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-10 07:40:27.117548 TitanicSurvivalModel100424-0.1.0/requirements/
--rw-r--r--   0 ongzhicong   (501) staff       (20)      585 2024-05-05 03:30:20.000000 TitanicSurvivalModel100424-0.1.0/requirements/requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 TitanicSurvivalModel100424-0.1.0/requirements/test_requirements.txt
--rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-10 07:40:27.124557 TitanicSurvivalModel100424-0.1.0/setup.cfg
--rw-r--r--   0 ongzhicong   (501) staff       (20)     1996 2024-05-10 07:40:06.000000 TitanicSurvivalModel100424-0.1.0/setup.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.901917 titanicsurvivalmodel100424-0.1.1/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      482 2024-05-09 06:18:45.000000 titanicsurvivalmodel100424-0.1.1/MANIFEST.in
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-18 07:36:23.901518 titanicsurvivalmodel100424-0.1.1/PKG-INFO
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.901010 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1138 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/PKG-INFO
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1022 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/SOURCES.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        1 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/dependency_links.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      188 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/requires.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       21 2024-05-18 07:36:23.000000 titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/top_level.txt
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.897710 titanicsurvivalmodel100424-0.1.1/classification_model/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        6 2024-05-18 07:34:56.000000 titanicsurvivalmodel100424-0.1.1/classification_model/VERSION
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      862 2024-05-04 09:04:59.000000 titanicsurvivalmodel100424-0.1.1/classification_model/__init__.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.898157 titanicsurvivalmodel100424-0.1.1/classification_model/config/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:23.000000 titanicsurvivalmodel100424-0.1.1/classification_model/config/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2128 2024-05-17 09:35:46.000000 titanicsurvivalmodel100424-0.1.1/classification_model/config/core.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      899 2024-05-17 08:13:51.000000 titanicsurvivalmodel100424-0.1.1/classification_model/config.yml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.898398 titanicsurvivalmodel100424-0.1.1/classification_model/datasets/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:51.000000 titanicsurvivalmodel100424-0.1.1/classification_model/datasets/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     2434 2024-05-17 06:12:30.000000 titanicsurvivalmodel100424-0.1.1/classification_model/pipeline.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1058 2024-05-18 07:00:50.000000 titanicsurvivalmodel100424-0.1.1/classification_model/predict.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.899236 titanicsurvivalmodel100424-0.1.1/classification_model/processing/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:08:58.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1750 2024-05-18 06:45:19.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/data_manager.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     3575 2024-05-17 06:26:00.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1763 2024-05-18 07:29:10.000000 titanicsurvivalmodel100424-0.1.1/classification_model/processing/validation.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      831 2024-05-17 06:24:46.000000 titanicsurvivalmodel100424-0.1.1/classification_model/train_pipeline.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.899966 titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)        0 2024-05-04 09:09:07.000000 titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/__init__.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     4110 2024-05-18 06:53:30.000000 titanicsurvivalmodel100424-0.1.1/classification_model/trained_models/classification_model_output_v0.1.0.pkl
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1914 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.1/pyproject.toml
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.894538 titanicsurvivalmodel100424-0.1.1/requirements/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      225 2024-05-17 09:24:00.000000 titanicsurvivalmodel100424-0.1.1/requirements/requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       65 2023-04-19 02:15:38.000000 titanicsurvivalmodel100424-0.1.1/requirements/test_requirements.txt
+-rw-r--r--   0 ongzhicong   (501) staff       (20)       38 2024-05-18 07:36:23.901998 titanicsurvivalmodel100424-0.1.1/setup.cfg
+-rw-r--r--   0 ongzhicong   (501) staff       (20)     1996 2024-05-10 07:40:06.000000 titanicsurvivalmodel100424-0.1.1/setup.py
+drwxr-xr-x   0 ongzhicong   (501) staff       (20)        0 2024-05-18 07:36:23.900703 titanicsurvivalmodel100424-0.1.1/tests/
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      680 2024-05-14 08:58:22.000000 titanicsurvivalmodel100424-0.1.1/tests/test_features.py
+-rw-r--r--   0 ongzhicong   (501) staff       (20)      855 2024-05-14 08:58:29.000000 titanicsurvivalmodel100424-0.1.1/tests/test_prediction.py
```

### Comparing `TitanicSurvivalModel100424-0.1.0/TitanicSurvivalModel100424.egg-info/SOURCES.txt` & `titanicsurvivalmodel100424-0.1.1/TitanicSurvivalModel100424.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 classification_model/config/__init__.py
 classification_model/config/core.py
 classification_model/datasets/__init__.py
 classification_model/processing/__init__.py
 classification_model/processing/data_manager.py
 classification_model/processing/features.py
 classification_model/processing/validation.py
-classification_model/trained_models/__init__.py
+classification_model/trained_models/__init__.py
+classification_model/trained_models/classification_model_output_v0.1.0.pkl
+tests/test_features.py
+tests/test_prediction.py
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/__init__.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/__init__.py`

 * *Files identical despite different names*

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/config/core.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/config/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from pathlib import Path
 from typing import List, Optional
 
 from pydantic import BaseModel
 from strictyaml import YAML, load
 
-import classification_model
+script_path = Path(__file__).resolve().parent
 
-# Project Directories
-PACKAGE_ROOT = Path(classification_model.__file__).resolve().parent
+PACKAGE_ROOT = script_path.parent
 ROOT = PACKAGE_ROOT.parent
 CONFIG_FILE_PATH = PACKAGE_ROOT / "config.yml"
 DATASET_DIR = PACKAGE_ROOT / "datasets"
 TRAINED_MODEL_DIR = PACKAGE_ROOT / "trained_models"
 
-
 class AppConfig(BaseModel):
     """
     Application-level config.
     """
-
     package_name: str
     training_data_file: str
     pipeline_save_file: str
 
 
 class ModelConfig(BaseModel):
     """
     All configuration relevant to model
     training and feature engineering.
     """
-
     target: str
     features: List[str]
     test_size: float
     random_state: int
     C: float
     categorical_vars: List[str]
     numerical_vars: List[str]
     cabin: List[str]
-    to_drop: List[str]
+    cols_to_drop: List[str]
+    name_title: List[str]
+    convert_to_float: List[str]
+    input_features: List[str]
 
 class Config(BaseModel):
     """Master config object."""
 
     app_config: AppConfig
     model_config: ModelConfig
 
@@ -73,12 +72,10 @@
         parsed_config = fetch_config_from_yaml()
 
     # specify the data attribute from the strictyaml YAML type.
     _config = Config(
         app_config=AppConfig(**parsed_config.data),
         model_config=ModelConfig(**parsed_config.data),
     )
-
     return _config
 
-
 config = create_and_validate_config()
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/config.yml` & `titanicsurvivalmodel100424-0.1.1/classification_model/config.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 # Package Overview
 package_name: classification_model
 
 # Data Files
 training_data_file: titanic_train.csv
-test_data_file: test.csv
 
 pipeline_name: classification_model
 pipeline_save_file: classification_model_output_v
 
 # Variables
 target: Survived
 
+input_features:
+  - PassengerId
+  - Pclass
+  - Name
+  - Sex
+  - Age
+  - SibSp
+  - Parch
+  - Ticket
+  - Fare
+  - Cabin
+  - Embarked
+
 features:
   - Age
   - Fare
   - Sex
   - Cabin
   - Embarked
   - Title
@@ -44,10 +56,19 @@
   - Pclass
   - Parch
   - Fare
 
 cabin:
   - Cabin
 
-to_drop:
+cols_to_drop:
+  - Name
+  - Ticket
+  - PassengerId
+
+name_title:
   - Name
-  - Ticket
+
+convert_to_float:
+  - Fare
+  - Age
+  - Pclass
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/pipeline.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 from sklearn.preprocessing import StandardScaler
 from sklearn.linear_model import LogisticRegression
 
 from classification_model.config.core import config
 from classification_model.processing import features as pp
 
 titanic_pipe = Pipeline(
-    [
+    [   
+        # ==== INITIAL PREPROCESSING ====  
+        ('replace_?_w_nan', pp.ReplaceWithNan()),
+        
+        ('get_first_cabin', pp.GetFirstCabin(variables=config.model_config.cabin)),
+
+        ('get_title', pp.GetTitle(variables=config.model_config.name_title)),
+        
+        ('convert_to_float', pp.DTypeTransformer_Float(variables=config.model_config.convert_to_float)),
+        
+        ('drop_cols', pp.DropColumns(variables=config.model_config.cols_to_drop)),
+
         # ===== IMPUTATION =====
         # impute categorical variables with string missing
         (
         'categorical_imputation', CategoricalImputer(
         imputation_method='missing', variables=config.model_config.categorical_vars)
         ),
         # add missing indicator to numerical variables
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/predict.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import typing as t
-
-import numpy as np
 import pandas as pd
 
 from classification_model import __version__ as _version
 from classification_model.config.core import config
 from classification_model.processing.data_manager import load_pipeline
 from classification_model.processing.validation import validate_inputs
 
@@ -18,15 +16,15 @@
     """
     data = pd.DataFrame(input_data)
     validated_data, errors = validate_inputs(input_data=data)
     results = {"predictions": None, "version": _version, "errors": errors}
     
     if not errors:
         predictions = _titanic_pipe.predict(
-            X=validated_data[config.model_config.features]
+            X=validated_data[config.model_config.input_features]
         )
         results = {
             "predictions": predictions,  # type: ignore
             "version": _version,
             "errors": errors,
         }
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/processing/data_manager.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/processing/data_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,24 @@
 import typing as t
-import re
 from pathlib import Path
-from typing import Union
 
 import joblib
 import pandas as pd
-import numpy as np
 from sklearn.pipeline import Pipeline
 
 from classification_model import __version__ as _version
 from classification_model.config.core import DATASET_DIR, TRAINED_MODEL_DIR, config
 
 
-def get_first_cabin(row) -> Union[str, float]:
-    try:
-        return row.split()[0]
-    except:
-        return np.nan
-    
-
-def get_title(passenger: str) -> str:
-    line = passenger
-    if re.search('Mrs', line):
-        return 'Mrs'
-    elif re.search('Mr', line):
-        return 'Mr'
-    elif re.search('Miss', line):
-        return 'Miss'
-    elif re.search('Master', line):
-        return 'Master'
-    else:
-        return 'Other'
-
-
 def load_dataset(*, file_name: str) -> pd.DataFrame:
     try:
         dataframe = pd.read_csv(Path(f"{DATASET_DIR}/{file_name}"))
     except:
         dataframe = pd.read_csv(file_name)
-    dataframe = dataframe.replace('?', np.nan)
-
-    dataframe['Cabin'] = dataframe['Cabin'].apply(get_first_cabin)
-    dataframe['Title'] = dataframe['Name'].apply(get_title)
-
-    dataframe["Fare"] = dataframe["Fare"].astype("float")
-    dataframe["Age"] = dataframe["Age"].astype("float")
-    dataframe["Pclass"] = dataframe["Pclass"].astype("float")
-
-    dataframe.drop(labels=config.model_config.to_drop, axis=1, inplace=True)
-
-
+    
     return dataframe
 
 
 def save_pipeline(*, pipeline_to_persist: Pipeline) -> None:
     """Persist the pipeline.
     Saves the versioned model, and overwrites any previous
     saved models. This ensures that when the package is
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/processing/validation.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/processing/validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def drop_na_inputs(*, input_data: pd.DataFrame) -> pd.DataFrame:
     """Check model inputs for na values and filter."""
     validated_data = input_data.copy()
     new_vars_with_na = [
         var
-        for var in config.model_config.features
+        for var in config.model_config.input_features
         if var
         not in config.model_config.categorical_vars
         + config.model_config.cabin
         + config.model_config.numerical_vars
         and validated_data[var].isnull().sum() > 0
     ]
     
@@ -24,19 +24,16 @@
 
     return validated_data
 
 
 def validate_inputs(*, input_data: pd.DataFrame) -> Tuple[pd.DataFrame, Optional[dict]]:
     """Check model inputs for unprocessable values."""
 
-    input_data["Fare"] = input_data["Fare"].astype("float")
-    input_data["Age"] = input_data["Age"].astype("float")
-    input_data["Pclass"] = input_data["Pclass"].astype("float")
-
-    relevant_data = input_data[config.model_config.features].copy()
+    relevant_data = input_data[config.model_config.input_features].copy()
+    
     validated_data = drop_na_inputs(input_data=relevant_data)
     errors = None
 
     try:
         # replace numpy nans so that pydantic can validate
         MultiplePassengerDataInputs(
             inputs=validated_data.replace({np.nan: None}).to_dict(orient="records")
@@ -44,14 +41,15 @@
     except ValidationError as error:
         errors = error.json()
 
     return validated_data, errors
 
 
 class PassengerDataInputSchema(BaseModel):
+    PassengerId: Optional[int]
     Age: Optional[float]
     Fare: Optional[float]
     Pclass: Optional[int]
     Sex: Optional[str]
     Name: Optional[str]
     SibSp: Optional[int]
     Parch: Optional[int]
```

### Comparing `TitanicSurvivalModel100424-0.1.0/classification_model/train_pipeline.py` & `titanicsurvivalmodel100424-0.1.1/classification_model/train_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Train the model."""
 
     # read training data
     data = load_dataset(file_name=config.app_config.training_data_file)
 
     # divide train and test
     X_train, X_test, y_train, y_test = train_test_split(
-        data[config.model_config.features],  # predictors
+        data.drop([config.model_config.target], axis=1),  # predictors
         data[config.model_config.target],
         test_size=config.model_config.test_size,
         random_state=config.model_config.random_state,
     )
 
     # fit model
     titanic_pipe.fit(X_train, y_train)
```

### Comparing `TitanicSurvivalModel100424-0.1.0/pyproject.toml` & `titanicsurvivalmodel100424-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TitanicSurvivalModel100424-0.1.0/setup.py` & `titanicsurvivalmodel100424-0.1.1/setup.py`

 * *Files identical despite different names*


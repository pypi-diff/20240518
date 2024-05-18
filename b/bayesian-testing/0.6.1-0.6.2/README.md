# Comparing `tmp/bayesian_testing-0.6.1.tar.gz` & `tmp/bayesian_testing-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian_testing-0.6.1.tar", max compression
+gzip compressed data, was "bayesian_testing-0.6.2.tar", max compression
```

## Comparing `bayesian_testing-0.6.1.tar` & `bayesian_testing-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/LICENSE
--rw-r--r--   0        0        0    17237 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/README.md
--rw-r--r--   0        0        0      326 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/__init__.py
--rw-r--r--   0        0        0      479 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/__init__.py
--rw-r--r--   0        0        0     2372 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/base.py
--rw-r--r--   0        0        0     7783 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/binary.py
--rw-r--r--   0        0        0    11852 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/delta_lognormal.py
--rw-r--r--   0        0        0    11090 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/delta_normal.py
--rw-r--r--   0        0        0     7616 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/discrete.py
--rw-r--r--   0        0        0     7722 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/exponential.py
--rw-r--r--   0        0        0     8932 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/normal.py
--rw-r--r--   0        0        0     7674 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/experiments/poisson.py
--rw-r--r--   0        0        0      425 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/metrics/__init__.py
--rw-r--r--   0        0        0    19837 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/metrics/evaluation.py
--rw-r--r--   0        0        0     8844 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/metrics/posteriors.py
--rw-r--r--   0        0        0       58 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/utilities/__init__.py
--rw-r--r--   0        0        0      383 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/utilities/common.py
--rw-r--r--   0        0        0      445 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/utilities/logging.conf
--rw-r--r--   0        0        0      285 2023-12-23 14:38:13.742757 bayesian_testing-0.6.1/bayesian_testing/utilities/logging.py
--rw-r--r--   0        0        0      800 2023-12-23 14:38:13.750757 bayesian_testing-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    18022 1970-01-01 00:00:00.000000 bayesian_testing-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/LICENSE
+-rw-r--r--   0        0        0    17237 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/README.md
+-rw-r--r--   0        0        0      326 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/__init__.py
+-rw-r--r--   0        0        0     2372 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/base.py
+-rw-r--r--   0        0        0     7783 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/binary.py
+-rw-r--r--   0        0        0    11852 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/delta_lognormal.py
+-rw-r--r--   0        0        0    11090 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/delta_normal.py
+-rw-r--r--   0        0        0     7616 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/discrete.py
+-rw-r--r--   0        0        0     7722 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/exponential.py
+-rw-r--r--   0        0        0     8932 2024-05-18 14:36:36.401985 bayesian_testing-0.6.2/bayesian_testing/experiments/normal.py
+-rw-r--r--   0        0        0     7674 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/experiments/poisson.py
+-rw-r--r--   0        0        0      425 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/metrics/__init__.py
+-rw-r--r--   0        0        0    19837 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/metrics/evaluation.py
+-rw-r--r--   0        0        0     8844 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/metrics/posteriors.py
+-rw-r--r--   0        0        0       58 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/utilities/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/utilities/common.py
+-rw-r--r--   0        0        0      445 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/utilities/logging.conf
+-rw-r--r--   0        0        0      285 2024-05-18 14:36:36.405985 bayesian_testing-0.6.2/bayesian_testing/utilities/logging.py
+-rw-r--r--   0        0        0      800 2024-05-18 14:36:36.413985 bayesian_testing-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    18022 1970-01-01 00:00:00.000000 bayesian_testing-0.6.2/PKG-INFO
```

### Comparing `bayesian_testing-0.6.1/LICENSE` & `bayesian_testing-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/README.md` & `bayesian_testing-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/base.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/base.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/binary.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/binary.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/delta_lognormal.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/delta_lognormal.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/delta_normal.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/delta_normal.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/discrete.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/discrete.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/exponential.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/exponential.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/normal.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/normal.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/experiments/poisson.py` & `bayesian_testing-0.6.2/bayesian_testing/experiments/poisson.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/metrics/evaluation.py` & `bayesian_testing-0.6.2/bayesian_testing/metrics/evaluation.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/bayesian_testing/metrics/posteriors.py` & `bayesian_testing-0.6.2/bayesian_testing/metrics/posteriors.py`

 * *Files identical despite different names*

### Comparing `bayesian_testing-0.6.1/pyproject.toml` & `bayesian_testing-0.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesian-testing"
-version = "0.6.1"
+version = "0.6.2"
 description = "Bayesian A/B testing with simple probabilities."
 authors = ["Matus Baniar"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Matt52/bayesian-testing"
 repository = "https://github.com/Matt52/bayesian-testing"
 keywords = ["ab testing", "bayes", "bayesian statistics"]
```

### Comparing `bayesian_testing-0.6.1/PKG-INFO` & `bayesian_testing-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesian-testing
-Version: 0.6.1
+Version: 0.6.2
 Summary: Bayesian A/B testing with simple probabilities.
 Home-page: https://github.com/Matt52/bayesian-testing
 License: MIT
 Keywords: ab testing,bayes,bayesian statistics
 Author: Matus Baniar
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


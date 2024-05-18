# Comparing `tmp/synapse_prometheus_exporter-0.0.1.tar.gz` & `tmp/synapse_prometheus_exporter-0.0.2.tar.gz`

## Comparing `synapse_prometheus_exporter-0.0.1.tar` & `synapse_prometheus_exporter-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/contrib/synapse-prometheus-exporter.service
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/src/synapse_prometheus_exporter/__init__.py
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/src/synapse_prometheus_exporter/__main__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/src/synapse_prometheus_exporter/config.dist.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/LICENSE
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/contrib/synapse-prometheus-exporter.service
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/src/synapse_prometheus_exporter/__init__.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/src/synapse_prometheus_exporter/__main__.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/src/synapse_prometheus_exporter/config.dist.yaml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 synapse_prometheus_exporter-0.0.2/PKG-INFO
```

### Comparing `synapse_prometheus_exporter-0.0.1/src/synapse_prometheus_exporter/__main__.py` & `synapse_prometheus_exporter-0.0.2/src/synapse_prometheus_exporter/__main__.py`

 * *Files identical despite different names*

### Comparing `synapse_prometheus_exporter-0.0.1/src/synapse_prometheus_exporter/config.dist.yaml` & `synapse_prometheus_exporter-0.0.2/src/synapse_prometheus_exporter/config.dist.yaml`

 * *Files identical despite different names*

### Comparing `synapse_prometheus_exporter-0.0.1/LICENSE` & `synapse_prometheus_exporter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_prometheus_exporter-0.0.1/README.md` & `synapse_prometheus_exporter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `synapse_prometheus_exporter-0.0.1/pyproject.toml` & `synapse_prometheus_exporter-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synapse-prometheus-exporter"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kumi Mitterer", email="synapse-prometheus-exporter@kumi.email" },
 ]
 description = "A Prometheus exporter for Synapse metrics"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `synapse_prometheus_exporter-0.0.1/PKG-INFO` & `synapse_prometheus_exporter-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: synapse-prometheus-exporter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Prometheus exporter for Synapse metrics
 Project-URL: Homepage, https://git.private.coffee/kumi/synapse-prometheus-exporter
 Project-URL: Bug Tracker, https://git.private.coffee/kumi/synapse-prometheus-exporter/issues
 Project-URL: Source Code, https://git.private.coffee/kumi/synapse-prometheus-exporter
 Author-email: Kumi Mitterer <synapse-prometheus-exporter@kumi.email>
 License: Copyright (c) 2024 Kumi Mitterer <synapse-prometheus-exporter@kumi.email>
```


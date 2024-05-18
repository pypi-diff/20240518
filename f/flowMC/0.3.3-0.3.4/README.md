# Comparing `tmp/flowmc-0.3.3.tar.gz` & `tmp/flowmc-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowmc-0.3.3.tar", last modified: Tue May  7 18:40:45 2024, max compression
+gzip compressed data, was "flowmc-0.3.4.tar", last modified: Sat May 18 02:04:09 2024, max compression
```

## Comparing `flowmc-0.3.3.tar` & `flowmc-0.3.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.848202 flowmc-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 18:40:36.000000 flowmc-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 18:40:45.848202 flowmc-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-07 18:40:36.000000 flowmc-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 18:40:36.000000 flowmc-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 18:40:45.848202 flowmc-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.840202 flowmc-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/nfmodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/realNVP.py
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/nfmodel/rqSpline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/Gaussian_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/HMC.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/MALA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/NF_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/proposal/flowHMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.844202 flowmc-0.3.3/src/flowMC/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/global_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/importance_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/strategy/optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.848202 flowmc-0.3.3/src/flowMC/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/EvolutionaryOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/PythonFunctionWrap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-07 18:40:36.000000 flowmc-0.3.3/src/flowMC/utils/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:40:45.848202 flowmc-0.3.3/src/flowMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 18:40:45.000000 flowmc-0.3.3/src/flowMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.160416 flowmc-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-18 02:04:05.000000 flowmc-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-18 02:04:09.160416 flowmc-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-18 02:04:05.000000 flowmc-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-18 02:04:05.000000 flowmc-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-18 02:04:09.160416 flowmc-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.152416 flowmc-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.152416 flowmc-0.3.4/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.156416 flowmc-0.3.4/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/nfmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/nfmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/nfmodel/rqSpline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.156416 flowmc-0.3.4/src/flowMC/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/proposal/flowHMC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.156416 flowmc-0.3.4/src/flowMC/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/strategy/global_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/strategy/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/strategy/optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.160416 flowmc-0.3.4/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/utils/EvolutionaryOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-18 02:04:05.000000 flowmc-0.3.4/src/flowMC/utils/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 02:04:09.160416 flowmc-0.3.4/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-18 02:04:09.000000 flowmc-0.3.4/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-18 02:04:09.000000 flowmc-0.3.4/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 02:04:09.000000 flowmc-0.3.4/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-18 02:04:09.000000 flowmc-0.3.4/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 02:04:09.000000 flowmc-0.3.4/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowmc-0.3.3/LICENSE` & `flowmc-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/PKG-INFO` & `flowmc-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.3
+Version: 0.3.4
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.3 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.4 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowmc-0.3.3/README.md` & `flowmc-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/setup.cfg` & `flowmc-0.3.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flowMC
-version = 0.3.3
+version = 0.3.4
 author = Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 author_email = kazewong.physics@gmail.com
 url = https://github.com/kazewong/flowMC
 description = Normalizing flow exhanced sampler in jax
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sampling, inference, machine learning, normalizing, autodiff, jax
```

### Comparing `flowmc-0.3.3/src/flowMC/Sampler.py` & `flowmc-0.3.4/src/flowMC/Sampler.py`

 * *Files 15% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     def load_flow(self, path: str):
         """
         Save the normalizing flow to a file.
 
         Args:
             path (str): Path to save the normalizing flow.
         """
-        self.nf_model.load_model(path)
+        self.nf_model = self.nf_model.load_model(path)
 
     def reset(self):
         """
         Reset the sampler state.
 
         """
         self.summary = {}
@@ -384,7 +384,50 @@
         Save the summary to a file.
 
         Args:
             path (str): Path to save the summary.
         """
         with open(path, "wb") as f:
             pickle.dump(self.summary, f)
+
+    def print_summary(self) -> None:
+        """
+        Print summary to the screen about log probabilities and local/global acceptance rates.
+        """
+        train_summary = self.get_sampler_state(training=True)
+        production_summary = self.get_sampler_state(training=False)
+
+        training_log_prob = train_summary["log_prob"]
+        training_local_acceptance = train_summary["local_accs"]
+        training_global_acceptance = train_summary["global_accs"]
+        training_loss = train_summary["loss_vals"]
+
+        production_log_prob = production_summary["log_prob"]
+        production_local_acceptance = production_summary["local_accs"]
+        production_global_acceptance = production_summary["global_accs"]
+
+        print("Training summary")
+        print("=" * 10)
+        print(
+            f"Log probability: {training_log_prob.mean():.3f} +/- {training_log_prob.std():.3f}"
+        )
+        print(
+            f"Local acceptance: {training_local_acceptance.mean():.3f} +/- {training_local_acceptance.std():.3f}"
+        )
+        print(
+            f"Global acceptance: {training_global_acceptance.mean():.3f} +/- {training_global_acceptance.std():.3f}"
+        )
+        print(
+            f"Max loss: {training_loss.max():.3f}, Min loss: {training_loss.min():.3f}"
+        )
+
+        print("Production summary")
+        print("=" * 10)
+        print(
+            f"Log probability: {production_log_prob.mean():.3f} +/- {production_log_prob.std():.3f}"
+        )
+        print(
+            f"Local acceptance: {production_local_acceptance.mean():.3f} +/- {production_local_acceptance.std():.3f}"
+        )
+        print(
+            f"Global acceptance: {production_global_acceptance.mean():.3f} +/- {production_global_acceptance.std():.3f}"
+        )
```

### Comparing `flowmc-0.3.3/src/flowMC/nfmodel/base.py` & `flowmc-0.3.4/src/flowMC/nfmodel/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def n_features(self) -> int:
         return NotImplemented
 
     def save_model(self, path: str):
         eqx.tree_serialise_leaves(path + ".eqx", self)
 
     def load_model(self, path: str):
-        self = eqx.tree_deserialise_leaves(path + ".eqx", self)
+        return eqx.tree_deserialise_leaves(path + ".eqx", self)
 
     @eqx.filter_value_and_grad
     def loss_fn(self, x):
         return -jnp.mean(self.log_prob(x))
 
     @eqx.filter_jit
     def train_step(
```

### Comparing `flowmc-0.3.3/src/flowMC/nfmodel/common.py` & `flowmc-0.3.4/src/flowMC/nfmodel/common.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/nfmodel/realNVP.py` & `flowmc-0.3.4/src/flowMC/nfmodel/realNVP.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/nfmodel/rqSpline.py` & `flowmc-0.3.4/src/flowMC/nfmodel/rqSpline.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/proposal/Gaussian_random_walk.py` & `flowmc-0.3.4/src/flowMC/proposal/Gaussian_random_walk.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/proposal/HMC.py` & `flowmc-0.3.4/src/flowMC/proposal/HMC.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/proposal/MALA.py` & `flowmc-0.3.4/src/flowMC/proposal/MALA.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/proposal/NF_proposal.py` & `flowmc-0.3.4/src/flowMC/proposal/NF_proposal.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/proposal/base.py` & `flowmc-0.3.4/src/flowMC/proposal/base.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/proposal/flowHMC.py` & `flowmc-0.3.4/src/flowMC/proposal/flowHMC.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/strategy/base.py` & `flowmc-0.3.4/src/flowMC/strategy/base.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/strategy/global_tuning.py` & `flowmc-0.3.4/src/flowMC/strategy/global_tuning.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/strategy/optimization.py` & `flowmc-0.3.4/src/flowMC/strategy/optimization.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/utils/EvolutionaryOptimizer.py` & `flowmc-0.3.4/src/flowMC/utils/EvolutionaryOptimizer.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/utils/PythonFunctionWrap.py` & `flowmc-0.3.4/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC/utils/postprocessing.py` & `flowmc-0.3.4/src/flowMC/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `flowmc-0.3.3/src/flowMC.egg-info/PKG-INFO` & `flowmc-0.3.4/src/flowMC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.3
+Version: 0.3.4
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.3 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.4 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowmc-0.3.3/src/flowMC.egg-info/SOURCES.txt` & `flowmc-0.3.4/src/flowMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*


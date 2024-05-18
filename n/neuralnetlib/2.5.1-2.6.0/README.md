# Comparing `tmp/neuralnetlib-2.5.1.tar.gz` & `tmp/neuralnetlib-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.5.1.tar", last modified: Fri May 17 20:38:08 2024, max compression
+gzip compressed data, was "neuralnetlib-2.6.0.tar", last modified: Sat May 18 14:05:58 2024, max compression
```

## Comparing `neuralnetlib-2.5.1.tar` & `neuralnetlib-2.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    45924 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 20:38:08.000000 neuralnetlib-2.5.1/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 20:38:08.093984 neuralnetlib-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-17 20:38:00.000000 neuralnetlib-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:05:58.799204 neuralnetlib-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-18 14:05:58.799204 neuralnetlib-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:05:58.799204 neuralnetlib-2.6.0/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45924 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:05:58.799204 neuralnetlib-2.6.0/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-18 14:05:58.000000 neuralnetlib-2.6.0/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-18 14:05:58.000000 neuralnetlib-2.6.0/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:05:58.000000 neuralnetlib-2.6.0/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 14:05:58.000000 neuralnetlib-2.6.0/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 14:05:58.000000 neuralnetlib-2.6.0/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 14:05:58.799204 neuralnetlib-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-18 14:05:51.000000 neuralnetlib-2.6.0/setup.py
```

### Comparing `neuralnetlib-2.5.1/LICENSE` & `neuralnetlib-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/PKG-INFO` & `neuralnetlib-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.5.1
+Version: 2.6.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.5.1/README.md` & `neuralnetlib-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/activations.py` & `neuralnetlib-2.6.0/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/callbacks.py` & `neuralnetlib-2.6.0/neuralnetlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/layers.py` & `neuralnetlib-2.6.0/neuralnetlib/layers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/losses.py` & `neuralnetlib-2.6.0/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/metrics.py` & `neuralnetlib-2.6.0/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/model.py` & `neuralnetlib-2.6.0/neuralnetlib/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import json
 import time
+import matplotlib
 
 import numpy as np
 
 from neuralnetlib.activations import ActivationFunction
 from neuralnetlib.layers import Layer, Input, Activation, Dropout, compatibility_dict
 from neuralnetlib.losses import LossFunction, CategoricalCrossentropy
-from neuralnetlib.metrics import accuracy_score
+from neuralnetlib.preprocessing import PCA
 from neuralnetlib.optimizers import Optimizer
 from neuralnetlib.utils import shuffle, progress_bar
+import matplotlib.pyplot as plt
+
+
+matplotlib.use("TkAgg")
 
 
 class Model:
     def __init__(self):
         self.layers = []
         self.loss_function = None
         self.optimizer = None
@@ -102,39 +107,80 @@
             error = error[:, None]
 
         self.backward_pass(error)
         return loss
 
     def fit(self, x_train: np.ndarray, y_train: np.ndarray, epochs: int, batch_size: int = None,
             verbose: bool = True, metrics: list = None, random_state: int = None, validation_data: tuple = None,
-            callbacks: list = None):
+            callbacks: list = None, plot_decision_boundary: bool = False):
         """
         Fit the model to the training data.
 
         Args:
             x_train: Training data
             y_train: Training labels
             epochs: Number of epochs to train the model
             batch_size: Number of samples per gradient update
             verbose: Whether to print training progress
             metrics: List of metric functions to evaluate the model
             random_state: Random seed for shuffling the data
             validation_data: Tuple of validation data and labels
             callbacks: List of callback objects (e.g., EarlyStopping)
+            plot_decision_boundary: Whether to plot the decision boundary
         """
+        global update_plot
         x_train = np.array(x_train) if not isinstance(
             x_train, np.ndarray) else x_train
         y_train = np.array(y_train) if not isinstance(
             y_train, np.ndarray) else y_train
 
         if validation_data is not None:
             x_test, y_test = validation_data
             x_test = np.array(x_test)
             y_test = np.array(y_test)
 
+        if plot_decision_boundary:
+            pca = PCA(n_components=2, random_state=random_state)
+            x_train_2d = pca.fit_transform(x_train)
+
+            fig, ax = plt.subplots(figsize=(8, 6))
+
+            x_min, x_max = x_train_2d[:, 0].min() - 1, x_train_2d[:, 0].max() + 1
+            y_min, y_max = x_train_2d[:, 1].min() - 1, x_train_2d[:, 1].max() + 1
+            xx, yy = np.meshgrid(np.arange(x_min, x_max, 0.1),
+                                 np.arange(y_min, y_max, 0.1))
+
+            y_train_encoded = np.argmax(y_train, axis=1) if y_train.ndim > 1 else y_train
+
+            def update_plot(epoch):
+                ax.clear()
+
+                scatter = ax.scatter(x_train_2d[:, 0], x_train_2d[:, 1], c=y_train_encoded, cmap='viridis', alpha=0.7)
+
+                labels = np.unique(y_train_encoded)
+                handles = [
+                    plt.Line2D([0], [0], marker='o', color='w', markerfacecolor=scatter.cmap(scatter.norm(label)),
+                               label=f'Class {label}', markersize=8) for label in labels]
+                ax.legend(handles=handles, title='Classes')
+
+                grid_points = np.c_[xx.ravel(), yy.ravel()]
+                Z = self.predict(pca.inverse_transform(grid_points))
+                if Z.shape[1] > 1:  # Multiclass classification
+                    Z = np.argmax(Z, axis=1).reshape(xx.shape)
+                    ax.contourf(xx, yy, Z, alpha=0.2, cmap=plt.cm.RdYlBu, levels=np.arange(Z.max() + 1))
+                else:  # Binary classification
+                    Z = (Z > 0.5).astype(int).reshape(xx.shape)
+                    ax.contourf(xx, yy, Z, alpha=0.2, cmap=plt.cm.RdYlBu, levels=1)
+
+                ax.set_xlabel("PCA Component 1")
+                ax.set_ylabel("PCA Component 2")
+                ax.set_title(f"Decision Boundary (Epoch {epoch + 1})")
+
+                fig.canvas.draw()
+
         for i in range(epochs):
             start_time = time.time()
 
             # Shuffling the data to avoid overfitting
             x_train_shuffled, y_train_shuffled = shuffle(
                 x_train, y_train, random_state=random_state)
 
@@ -186,18 +232,18 @@
                 x_test, y_test = validation_data
                 val_predictions = self.predict(x_test)
                 val_metrics = []
                 if metrics is not None:
                     for metric in metrics:
                         # Change extend to append
                         val_metrics.append(metric(val_predictions, y_test))
-                if verbose:
-                    val_metrics_str = ' - '.join(
-                        f'{metric.__name__}: {val_metric:.4f}' for metric, val_metric in zip(metrics, val_metrics))
-                    print(f' - {val_metrics_str}', end='')
+                    if verbose:
+                        val_metrics_str = ' - '.join(
+                            f'{metric.__name__}: {val_metric:.4f}' for metric, val_metric in zip(metrics, val_metrics))
+                        print(f' - {val_metrics_str}', end='')
 
             if callbacks:
                 metrics_values = {}
                 if metrics is not None:
                     for metric in metrics:
                         metrics_values[metric.__name__] = metric(
                             np.vstack(predictions_list), np.vstack(y_true_list))
@@ -214,14 +260,21 @@
                         break
 
                 if any(callback.stop_training for callback in callbacks):
                     break
 
             if verbose:
                 print()
+                
+            if plot_decision_boundary:
+                update_plot(i)
+                plt.pause(0.1)  # Pause pour laisser le temps de mettre à jour le graphique
+
+        if plot_decision_boundary and 'IPython' in globals():
+            plt.show(block=False)
 
         if verbose:
             print()
 
     def evaluate(self, x_test: np.ndarray, y_test: np.ndarray) -> float:
         x_test = np.array(x_test)
         y_test = np.array(y_test)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neuralnetlib-2.5.1/neuralnetlib/optimizers.py` & `neuralnetlib-2.6.0/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib/preprocessing.py` & `neuralnetlib-2.6.0/neuralnetlib/preprocessing.py`

 * *Files 11% similar despite different names*

```diff
@@ -248,7 +248,41 @@
         self.fit(X)
         return self.transform(X)
 
     def inverse_transform(self, X):
         if self.min_ is None or self.scale_ is None:
             raise ValueError("MinMaxScaler has not been fitted yet.")
         return (X - self.feature_range[0]) / (self.feature_range[1] - self.feature_range[0]) * self.scale_ + self.min_
+
+
+class PCA:
+    def __init__(self, n_components: int, random_state: int = None):
+        self.n_components = n_components
+        self.random_state = random_state
+        self.components = None
+        self.mean = None
+
+    def fit(self, X: np.ndarray):
+        self.mean = np.mean(X, axis=0)
+        X_centered = X - self.mean
+
+        covariance_matrix = np.cov(X_centered, rowvar=False)
+
+        eigenvalues, eigenvectors = np.linalg.eigh(covariance_matrix)
+
+        sorted_indices = np.argsort(eigenvalues)[::-1]
+        eigenvalues = eigenvalues[sorted_indices]
+        eigenvectors = eigenvectors[:, sorted_indices]
+
+        self.components = eigenvectors[:, :self.n_components]
+
+    def transform(self, X: np.ndarray) -> np.ndarray:
+        X_centered = X - self.mean
+
+        return np.dot(X_centered, self.components)
+
+    def fit_transform(self, X: np.ndarray) -> np.ndarray:
+        self.fit(X)
+        return self.transform(X)
+
+    def inverse_transform(self, X: np.ndarray) -> np.ndarray:
+        return np.dot(X, self.components.T) + self.mean
```

### Comparing `neuralnetlib-2.5.1/neuralnetlib/utils.py` & `neuralnetlib-2.6.0/neuralnetlib/utils.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.5.1/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.6.0/neuralnetlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.5.1
+Version: 2.6.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.5.1/setup.py` & `neuralnetlib-2.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.5.1',
+    version='2.6.0',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```


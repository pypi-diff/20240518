# Comparing `tmp/autonav-1.0.2.tar.gz` & `tmp/autonav-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonav-1.0.2.tar", last modified: Tue Mar 12 18:23:11 2024, max compression
+gzip compressed data, was "autonav-1.0.3.tar", last modified: Sat May 18 15:02:54 2024, max compression
```

## Comparing `autonav-1.0.2.tar` & `autonav-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:23:11.782726 autonav-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-12 18:23:05.000000 autonav-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-03-12 18:23:11.782726 autonav-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-03-12 18:23:05.000000 autonav-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:23:11.778726 autonav-1.0.2/autonav/
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/GTRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/WLS.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/random_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-12 18:23:05.000000 autonav-1.0.2/autonav/velocity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:23:11.782726 autonav-1.0.2/autonav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-03-12 18:23:11.000000 autonav-1.0.2/autonav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-12 18:23:11.000000 autonav-1.0.2/autonav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 18:23:11.000000 autonav-1.0.2/autonav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-12 18:23:11.000000 autonav-1.0.2/autonav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-12 18:23:11.000000 autonav-1.0.2/autonav.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-12 18:23:05.000000 autonav-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 18:23:11.782726 autonav-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:23:11.782726 autonav-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_GTRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_WLS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_random_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-12 18:23:05.000000 autonav-1.0.2/tests/test_velocity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:02:54.339155 autonav-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-18 15:02:47.000000 autonav-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-18 15:02:54.339155 autonav-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-18 15:02:47.000000 autonav-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:02:54.335155 autonav-1.0.3/autonav/
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/GTRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/WLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/random_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-18 15:02:47.000000 autonav-1.0.3/autonav/velocity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:02:54.335155 autonav-1.0.3/autonav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-18 15:02:54.000000 autonav-1.0.3/autonav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-18 15:02:54.000000 autonav-1.0.3/autonav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:02:54.000000 autonav-1.0.3/autonav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-18 15:02:54.000000 autonav-1.0.3/autonav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 15:02:54.000000 autonav-1.0.3/autonav.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-18 15:02:48.000000 autonav-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:02:54.339155 autonav-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:02:54.335155 autonav-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_GTRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_WLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_random_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-18 15:02:48.000000 autonav-1.0.3/tests/test_velocity.py
```

### Comparing `autonav-1.0.2/LICENSE.txt` & `autonav-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autonav-1.0.2/PKG-INFO` & `autonav-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonav
-Version: 1.0.2
+Version: 1.0.3
 Summary: Research software for navigating a UAV in indoor environments
 Author-email: "Ricardo S. Santos" <p6221@ulusofona.pt>
 License: MIT
 Project-URL: Bug Reports, https://github.com/ricardo-s-santos/AutoNAV/issues
 Project-URL: Documentation, https://ricardo-s-santos.github.io/AutoNAV/
 Project-URL: Source, https://github.com/ricardo-s-santos/AutoNAV
 Keywords: UAV,Navigation,Indoor
@@ -88,35 +88,53 @@
     [0, 0, b / 8],
     [0, b, b / 8],
     [b / 2, 0, b / 8],
     [b / 2, b, b / 8],]
     ).T
 # Number of measurement samples
 k = 50
-# Noise standard deviation
-sigma = 1
 # Maximum velocity allowed to the UAV
 v_max = b / 100
 # Distance threshold
 tau = b / 50
 # Smoothing factor
 gamma = b / 100
 # Initial position of the UAV
 initial_uav_position = [10, 10, 5]
 # File containing the waypoints
 destinations = readpathfile("docs/docs/examples/Path.csv")
+# Noise seed
+noise_seed = 1
+# Noise Distribution
+noise_distribution = "normal"
+# Noise distribution parameters
+mean = 0
+std = 1
+noise_distribution_parameters = [mean, std]
 ```
 
 Finally, run the GTRS or WLS algorithm and plot the trajectories:
 
 ```python
-# Estimate the trajectory using the GTRS algorithm
-[estimated_trajectory, true_trajectory] = gtrs(a_i, n, k, sigma, destinations, initial_uav_position, v_max, tau, gamma)
-# Plot the estimated trajectory
-plot_trajectories(destinations, [estimated_trajectory], a_i, ['GTRS'])
+# Estimate the positions and trajectory using the GTRS algorithm
+[estimated_positions, true_trajectory] = gtrs(
+    a_i,
+    n,
+    k,
+    destinations,
+    initial_uav_position,
+    v_max,
+    tau,
+    gamma,
+    noise_seed,
+    noise_distribution,
+    noise_distribution_parameters,
+)
+# Plot the trajectory that the UAV followed
+plot_trajectories(destinations, [true_trajectory], a_i, ['GTRS'])
 plt.show()
 ```
 
 <p align="center">
   <img src="https://github.com/ricardo-s-santos/AutoNAV/blob/main/docs/docs/figures/trajectories_plot.png?raw=true" alt="image" width="auto" height="auto">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autonav Version: 1.0.2 Summary: Research software
+Metadata-Version: 2.1 Name: autonav Version: 1.0.3 Summary: Research software
 for navigating a UAV in indoor environments Author-email: "Ricardo S. Santos"
 ulusofona.pt> License: MIT Project-URL: Bug Reports, https://github.com/
 ricardo-s-santos/AutoNAV/issues Project-URL: Documentation, https://ricardo-s-
 santos.github.io/AutoNAV/ Project-URL: Source, https://github.com/ricardo-s-
 santos/AutoNAV Keywords: UAV,Navigation,Indoor Classifier: Development Status
 :: 5 - Production/Stable Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
@@ -34,25 +34,28 @@
 the package one can import the algorithms and necessary dependencies as
 follows: ```python import matplotlib.pyplot as plt from autonav import gtrs,
 wls from autonav.file_handlers import readpathfile from autonav.plots import
 plot_trajectories from numpy import array ``` Afterwards, one can create the
 necessary values to run the algorithms: ```python # Area border b = 200 #
 Number of anchors n = 8 # Position of the anchors a_i = array( [ [0, 0, 0], [0,
 b, 0], [b / 2, 0, 0], [b / 2, b, 0], [0, 0, b / 8], [0, b, b / 8], [b / 2, 0, b
-/ 8], [b / 2, b, b / 8],] ).T # Number of measurement samples k = 50 # Noise
-standard deviation sigma = 1 # Maximum velocity allowed to the UAV v_max = b /
-100 # Distance threshold tau = b / 50 # Smoothing factor gamma = b / 100 #
-Initial position of the UAV initial_uav_position = [10, 10, 5] # File
-containing the waypoints destinations = readpathfile("docs/docs/examples/
-Path.csv") ``` Finally, run the GTRS or WLS algorithm and plot the
-trajectories: ```python # Estimate the trajectory using the GTRS algorithm
-[estimated_trajectory, true_trajectory] = gtrs(a_i, n, k, sigma, destinations,
-initial_uav_position, v_max, tau, gamma) # Plot the estimated trajectory
-plot_trajectories(destinations, [estimated_trajectory], a_i, ['GTRS']) plt.show
-() ```
+/ 8], [b / 2, b, b / 8],] ).T # Number of measurement samples k = 50 # Maximum
+velocity allowed to the UAV v_max = b / 100 # Distance threshold tau = b / 50 #
+Smoothing factor gamma = b / 100 # Initial position of the UAV
+initial_uav_position = [10, 10, 5] # File containing the waypoints destinations
+= readpathfile("docs/docs/examples/Path.csv") # Noise seed noise_seed = 1 #
+Noise Distribution noise_distribution = "normal" # Noise distribution
+parameters mean = 0 std = 1 noise_distribution_parameters = [mean, std] ```
+Finally, run the GTRS or WLS algorithm and plot the trajectories: ```python #
+Estimate the positions and trajectory using the GTRS algorithm
+[estimated_positions, true_trajectory] = gtrs( a_i, n, k, destinations,
+initial_uav_position, v_max, tau, gamma, noise_seed, noise_distribution,
+noise_distribution_parameters, ) # Plot the trajectory that the UAV followed
+plot_trajectories(destinations, [true_trajectory], a_i, ['GTRS']) plt.show()
+```
                                     [image]
 ## References [1] J. P. Matos-Carvalho, R. Santos, S. Tomic and M. Beko, "GTRS-
 Based Algorithm for UAV Navigation in Indoor Environments Employing Range
 Measurements and Odometry," in IEEE Access, vol. 9, pp. 89120-89132, 2021, doi:
 10.1109/ACCESS.2021.3089900. https://ieeexplore.ieee.org/document/9456863 [2]
 R. Santos, J. P. Matos-Carvalho, S. Tomic and M. Beko, "WLS algorithm for UAV
 navigation in satelliteâless environments," in IET Wireless Sensor Systems,
```

### Comparing `autonav-1.0.2/README.md` & `autonav-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -48,35 +48,53 @@
     [0, 0, b / 8],
     [0, b, b / 8],
     [b / 2, 0, b / 8],
     [b / 2, b, b / 8],]
     ).T
 # Number of measurement samples
 k = 50
-# Noise standard deviation
-sigma = 1
 # Maximum velocity allowed to the UAV
 v_max = b / 100
 # Distance threshold
 tau = b / 50
 # Smoothing factor
 gamma = b / 100
 # Initial position of the UAV
 initial_uav_position = [10, 10, 5]
 # File containing the waypoints
 destinations = readpathfile("docs/docs/examples/Path.csv")
+# Noise seed
+noise_seed = 1
+# Noise Distribution
+noise_distribution = "normal"
+# Noise distribution parameters
+mean = 0
+std = 1
+noise_distribution_parameters = [mean, std]
 ```
 
 Finally, run the GTRS or WLS algorithm and plot the trajectories:
 
 ```python
-# Estimate the trajectory using the GTRS algorithm
-[estimated_trajectory, true_trajectory] = gtrs(a_i, n, k, sigma, destinations, initial_uav_position, v_max, tau, gamma)
-# Plot the estimated trajectory
-plot_trajectories(destinations, [estimated_trajectory], a_i, ['GTRS'])
+# Estimate the positions and trajectory using the GTRS algorithm
+[estimated_positions, true_trajectory] = gtrs(
+    a_i,
+    n,
+    k,
+    destinations,
+    initial_uav_position,
+    v_max,
+    tau,
+    gamma,
+    noise_seed,
+    noise_distribution,
+    noise_distribution_parameters,
+)
+# Plot the trajectory that the UAV followed
+plot_trajectories(destinations, [true_trajectory], a_i, ['GTRS'])
 plt.show()
 ```
 
 <p align="center">
   <img src="https://github.com/ricardo-s-santos/AutoNAV/blob/main/docs/docs/figures/trajectories_plot.png?raw=true" alt="image" width="auto" height="auto">
 </p>
```

#### html2text {}

```diff
@@ -12,25 +12,28 @@
 the package one can import the algorithms and necessary dependencies as
 follows: ```python import matplotlib.pyplot as plt from autonav import gtrs,
 wls from autonav.file_handlers import readpathfile from autonav.plots import
 plot_trajectories from numpy import array ``` Afterwards, one can create the
 necessary values to run the algorithms: ```python # Area border b = 200 #
 Number of anchors n = 8 # Position of the anchors a_i = array( [ [0, 0, 0], [0,
 b, 0], [b / 2, 0, 0], [b / 2, b, 0], [0, 0, b / 8], [0, b, b / 8], [b / 2, 0, b
-/ 8], [b / 2, b, b / 8],] ).T # Number of measurement samples k = 50 # Noise
-standard deviation sigma = 1 # Maximum velocity allowed to the UAV v_max = b /
-100 # Distance threshold tau = b / 50 # Smoothing factor gamma = b / 100 #
-Initial position of the UAV initial_uav_position = [10, 10, 5] # File
-containing the waypoints destinations = readpathfile("docs/docs/examples/
-Path.csv") ``` Finally, run the GTRS or WLS algorithm and plot the
-trajectories: ```python # Estimate the trajectory using the GTRS algorithm
-[estimated_trajectory, true_trajectory] = gtrs(a_i, n, k, sigma, destinations,
-initial_uav_position, v_max, tau, gamma) # Plot the estimated trajectory
-plot_trajectories(destinations, [estimated_trajectory], a_i, ['GTRS']) plt.show
-() ```
+/ 8], [b / 2, b, b / 8],] ).T # Number of measurement samples k = 50 # Maximum
+velocity allowed to the UAV v_max = b / 100 # Distance threshold tau = b / 50 #
+Smoothing factor gamma = b / 100 # Initial position of the UAV
+initial_uav_position = [10, 10, 5] # File containing the waypoints destinations
+= readpathfile("docs/docs/examples/Path.csv") # Noise seed noise_seed = 1 #
+Noise Distribution noise_distribution = "normal" # Noise distribution
+parameters mean = 0 std = 1 noise_distribution_parameters = [mean, std] ```
+Finally, run the GTRS or WLS algorithm and plot the trajectories: ```python #
+Estimate the positions and trajectory using the GTRS algorithm
+[estimated_positions, true_trajectory] = gtrs( a_i, n, k, destinations,
+initial_uav_position, v_max, tau, gamma, noise_seed, noise_distribution,
+noise_distribution_parameters, ) # Plot the trajectory that the UAV followed
+plot_trajectories(destinations, [true_trajectory], a_i, ['GTRS']) plt.show()
+```
                                     [image]
 ## References [1] J. P. Matos-Carvalho, R. Santos, S. Tomic and M. Beko, "GTRS-
 Based Algorithm for UAV Navigation in Indoor Environments Employing Range
 Measurements and Odometry," in IEEE Access, vol. 9, pp. 89120-89132, 2021, doi:
 10.1109/ACCESS.2021.3089900. https://ieeexplore.ieee.org/document/9456863 [2]
 R. Santos, J. P. Matos-Carvalho, S. Tomic and M. Beko, "WLS algorithm for UAV
 navigation in satelliteâless environments," in IET Wireless Sensor Systems,
```

### Comparing `autonav-1.0.2/autonav/GTRS.py` & `autonav-1.0.3/autonav/GTRS.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module contains the GTRS algorithm functions."""
 
 import math
+from typing import Optional
 
 from numpy import (
     append,
     arange,
     array,
     asarray,
     concatenate,
@@ -29,66 +30,73 @@
 from autonav.velocity import _velocity
 
 
 def gtrs(
     a_i: ArrayLike,
     n: int,
     k: int,
-    sigma: float,
     destinations: ArrayLike,
     initial_uav_position: ArrayLike,
     v_max: float,
     tau: float,
     gamma: float,
     noise_seed: int = 1,
+    noise_distribution: str = "standard_normal",
+    distribution_parameters: Optional[ArrayLike] = None,
     tol: float = 0.001,
     n_iter: int = 30,
     max_lim: float = 1000000.0,
 ) -> NDArray:
     """Executes the GTRS algorithm.
 
     [See here more details about the GTRS algorithm.](https://ieeexplore.ieee.org/document/9456863)
 
     Args:
         a_i: The true position of the anchors in 3D.
         n: The number of anchors.
         k: The number of measurements.
-        sigma: The noise level in meters.
         destinations: The intermediate points need for navigation in 3D.
         initial_uav_position: The initial UAV position in 3D.
         v_max: The maximum velocity that the UAV can fly.
         tau: The threshold to reach the destination.
         gamma: The smoothing factor.
         noise_seed: The seed to generate the noise.
+        noise_distribution: The distribution used to model the noise.
+        distribution_parameters: Optional parameters to customize the noise distribution.
         tol: The tolerance for the bisection function.
         n_iter: The max number of iterations for the bisection function.
         max_lim: The maximum value for the interval in the bisection function.
 
     Returns:
-        The estimated trajectory computed using the GTRS algorithm for the given input scenario
-          and the true trajectory that the UAV followed.
+        The estimated positions for the UAV computed using the GTRS algorithm for the given input scenario
+        and the true trajectory that the UAV followed.
     """
     # Transform inputs in NDArray
     arr_a_i: NDArray = asarray(a_i, dtype=float)
     arr_destinations: NDArray = asarray(destinations, dtype=float)
     arr_initial_uav_position: NDArray = asarray(initial_uav_position, dtype=float)
+    if distribution_parameters is None:
+        arr_distribution_parameters: NDArray = asarray([])
+    else:
+        arr_distribution_parameters = asarray(distribution_parameters, dtype=float)
     # Validate inputs
     if size(arr_a_i, axis=1) != n:
         raise ValueError("The length of a_i must be equal to N.")
     if k <= 0:
         raise ValueError("K must be positive.")
-    if sigma < 0 or sigma > 5:
-        raise ValueError("Sigma must be between 0 and 5.")
     if size(arr_destinations) == 0:
         raise ValueError("Waypoints cannot be empty.")
     if size(arr_destinations, axis=1) != 3:
         raise ValueError("Waypoints must contain the 3 coordinates (x, y, z).")
     if size(arr_initial_uav_position) != 3:
         raise ValueError("Initial UAV position must contain the 3 coordinates (x, y, z).")
     # Test optional inputs
+    available_noise_distributions = ["normal", "standard_normal", "exponential"]
+    if noise_distribution not in available_noise_distributions:
+        raise ValueError("Noise distribution must be " + ", ".join(available_noise_distributions) + ".")
     if tol < 0:
         raise ValueError("Tolerance must be positive.")
     if n_iter < 0:
         raise ValueError("Number of Bisection iterations must be positive.")
     if max_lim < 0:
         raise ValueError("The maximum value for the interval in the bisection function must be positive.")
     # Time sample in seconds
@@ -115,15 +123,15 @@
         ),
     )
     x_state = zeros(shape=(6, 1))
     x_loc = zeros(shape=(3, 1))
     p = eye(6)
     qq = 0
     x_true = arr_initial_uav_position[:]
-    estimated_trajectory = []
+    estimated_positions = []
     true_trajectory = []
     ww = 0
     n_dest = len(arr_destinations) - 1
     # Generator to create random numbers
     gen = random_generator(noise_seed)
     while ww <= n_dest:
         distance = math.sqrt(
@@ -134,15 +142,35 @@
         while distance > 1:
             x = x_true[:]
             # ---------------------------------------------------------------------
             # Simulation part
             # ---------------------------------------------------------------------
             di_k = sqrt(((x[0] - arr_a_i[0, :]) ** 2) + ((x[1] - arr_a_i[1, :]) ** 2) + ((x[2] - arr_a_i[2, :]) ** 2))
             di_k = array([di_k]).T
-            di_k = di_k + (sigma * gen.standard_normal(size=(n, k)))
+            if noise_distribution == "normal":
+                # See if user passed the mean and std
+                if size(arr_distribution_parameters) == 2:
+                    mean = arr_distribution_parameters[0]
+                    std = arr_distribution_parameters[1]
+                    noise_model = gen.normal(loc=mean, scale=std, size=(n, k))
+                else:
+                    noise_model = gen.normal(size=(n, k))
+                di_k = di_k + noise_model
+            elif noise_distribution == "exponential":
+                # See if user passed the rate
+                if size(arr_distribution_parameters) == 1:
+                    rate = arr_distribution_parameters[0]
+                    noise_model = gen.exponential(scale=rate, size=(n, k))
+                else:
+                    rate = 10**-6
+                    noise_model = gen.exponential(scale=rate, size=(n, k))
+                di_k = di_k + noise_model
+            elif noise_distribution == "standard_normal":  # Default distribution
+                noise_model = gen.standard_normal(size=(n, k))
+                di_k = di_k + noise_model
             d_i = median(di_k, axis=1)
             d_i = array([d_i]).T
             # ---------------------------------------------------------------------
             # Estimation part
             # ---------------------------------------------------------------------
             a1_loc = zeros(shape=(n, 4))
             b1_loc = zeros(shape=(n, 1))
@@ -194,15 +222,15 @@
                 (dot(a_loc.T, a_loc) + dot(lambda_loc, d_loc) + dot(1e-06, eye(size(a_loc, 1)))),
                 (dot(a_loc.T, b_loc) - dot(lambda_loc, f_loc)),
             )
             if qq == 0:
                 x_loc[0:3, qq] = real(y_hat_loc[0:3, 0])
                 x_state[0:6, qq] = concatenate((x_loc[0:3, qq], zeros(3)), axis=0)
                 p = eye(6)
-                estimated_trajectory.append(x_loc[0:3, qq])
+                estimated_positions.append(x_loc[0:3, qq])
             else:
                 x_loc = insert(x_loc, qq, real(y_hat_loc[0:3, 0]), axis=1)
                 eigen_values = _calc_eigen(a_track, d_track)
                 eig_1 = max(eigen_values)
                 min_lim = -1.0 / eig_1
                 lambda_track = _bisection_fun(min_lim, max_lim, tol, n_iter, a_track, d_track, b_track, f_track)
                 y_hat_track = solve(
@@ -210,28 +238,28 @@
                     (dot(a_track.T, b_track) - dot(lambda_track, f_track)),
                 )
                 x_state = concatenate((x_state, zeros((size(x_state, 0), 1))), axis=1)
                 x_state[0:6, qq] = concatenate((real(y_hat_track[arange(0, size(x_state, 0))])), axis=0)
                 lk1 = subtract(x_state[0:6, qq], x_state[0:6, qq - 1]).reshape((6, 1))
                 lk2 = subtract(x_state[0:6, qq], x_state[0:6, qq - 1]).reshape((6, 1)).T
                 p = matmul(lk1, lk2)
-                estimated_trajectory.append(x_loc[0:3, qq])
+                estimated_positions.append(x_loc[0:3, qq])
             true_trajectory.append(x_true.copy())
             uav_velocity = _velocity(x_loc[0:3, qq], arr_destinations[ww, :], v_max, tau, gamma)
             x_true[0] = x_true[0] + uav_velocity[0]
             x_true[1] = x_true[1] + uav_velocity[1]
             x_true[2] = x_true[2] + uav_velocity[2]
             distance = math.sqrt(
                 (x_true[0] - arr_destinations[ww][0]) ** 2
                 + (x_true[1] - arr_destinations[ww][1]) ** 2
                 + (x_true[2] - arr_destinations[ww][2]) ** 2
             )
             qq += 1
         ww += 1
-    return array([array(estimated_trajectory), array(true_trajectory)])
+    return array([array(estimated_positions), array(true_trajectory)])
 
 
 def _bisection_fun(
     min_lim: float,
     max_lim: float,
     tol: float,
     n_iter: int,
```

### Comparing `autonav-1.0.2/autonav/WLS.py` & `autonav-1.0.3/autonav/WLS.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,85 @@
 """This module contains the WLS algorithm."""
 
 import cmath
 import itertools
 import math
+from typing import Optional
 
 from numpy import array, asarray, cos, dot, eye, median, sin, size, sqrt, zeros
 from numpy.lib import scimath
 from numpy.linalg import norm, solve
 from numpy.typing import ArrayLike, NDArray
 
 from autonav.random_generator import random_generator
 from autonav.velocity import _velocity
 
 
 def wls(
     a_i: ArrayLike,
     n: int,
     k: int,
-    sigma: float,
     destinations: ArrayLike,
     initial_uav_position: ArrayLike,
-    v_max: int,
-    tau: int,
-    gamma: int,
+    v_max: float,
+    tau: float,
+    gamma: float,
     noise_seed: int = 1,
+    noise_distribution: str = "standard_normal",
+    distribution_parameters: Optional[ArrayLike] = None,
 ) -> NDArray:
     """Executes the WLS algorithm.
 
     [See here more details about the WLS algorithm.]
     (https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/wss2.12041)
 
     Args:
         a_i: The true position of the anchors in 3D.
         n: The number of anchors.
         k: The number of measurements.
-        sigma: The noise level in meters.
         destinations: The intermediate points need for navigation in 3D.
         initial_uav_position: The initial UAV position in 3D.
         v_max: The maximum velocity that the UAV can fly.
         tau: The threshold to reach the destination.
         gamma: The smoothing factor.
         noise_seed: The seed to generate the noise.
+        noise_distribution: The distribution used to model the noise.
+        distribution_parameters: Optional parameters to customize the noise distribution.
 
     Returns:
-        The estimated trajectory computed using the WLS algorithm for the given input scenario
-          and the true trajectory that the UAV followed.
+        The estimated positions for the UAV computed using the WLS algorithm for the given input scenario
+        and the true trajectory that the UAV followed.
     """
     # Transform inputs in NDArray
     arr_a_i: NDArray = asarray(a_i, dtype=float)
     arr_destinations: NDArray = asarray(destinations, dtype=float)
     arr_initial_uav_position: NDArray = asarray(initial_uav_position, dtype=float)
+    if distribution_parameters is None:
+        arr_distribution_parameters: NDArray = asarray([])
+    else:
+        arr_distribution_parameters = asarray(distribution_parameters, dtype=float)
     # Validate inputs
     if size(arr_a_i, axis=1) != n:
         raise ValueError("The length of a_i must be equal to N.")
     if k <= 0:
         raise ValueError("K must be positive.")
-    if sigma < 0 or sigma > 5:
-        raise ValueError("Sigma must be between 0 and 5.")
     if size(arr_destinations) == 0:
         raise ValueError("Waypoints cannot be empty.")
     if size(arr_destinations, axis=1) != 3:
         raise ValueError("Waypoints must contain the 3 coordinates (x, y, z).")
     if size(initial_uav_position) != 3:
         raise ValueError("Initial UAV position must contain the 3 coordinates (x, y, z).")
+    # Test optional inputs
+    available_noise_distributions = ["normal", "standard_normal", "exponential"]
+    if noise_distribution not in available_noise_distributions:
+        raise ValueError("Noise distribution must be " + ", ".join(available_noise_distributions) + ".")
     x_true = arr_initial_uav_position[:]
     ww = 0
     n_dest = len(arr_destinations) - 1
-    estimated_trajectory = []
+    estimated_positions = []
     true_trajectory = []
     # Generator to create random numbers (see line 65)
     gen = random_generator(noise_seed)
     while ww <= n_dest:
         distance = math.sqrt(
             (x_true[0] - arr_destinations[ww][0]) ** 2
             + (x_true[1] - arr_destinations[ww][1]) ** 2
@@ -79,15 +88,35 @@
         while distance > 1:
             x = x_true[0:3]
             # ---------------------------------------------------------------------
             # Simulation part
             # ---------------------------------------------------------------------
             di_k = sqrt(((x[0] - arr_a_i[0, :]) ** 2) + ((x[1] - arr_a_i[1, :]) ** 2) + ((x[2] - arr_a_i[2, :]) ** 2))
             di_k = array([di_k]).T
-            di_k = di_k + (sigma * gen.standard_normal(size=(n, k)))
+            if noise_distribution == "normal":
+                # See if user passed the mean and std
+                if size(arr_distribution_parameters) == 2:
+                    mean = arr_distribution_parameters[0]
+                    std = arr_distribution_parameters[1]
+                    noise_model = gen.normal(loc=mean, scale=std, size=(n, k))
+                else:
+                    noise_model = gen.normal(size=(n, k))
+                di_k = di_k + noise_model
+            elif noise_distribution == "exponential":
+                # See if user passed the rate
+                if size(arr_distribution_parameters) == 1:
+                    rate = arr_distribution_parameters[0]
+                    noise_model = gen.exponential(scale=rate, size=(n, k))
+                else:
+                    rate = 10**-6
+                    noise_model = gen.exponential(scale=rate, size=(n, k))
+                di_k = di_k + noise_model
+            elif noise_distribution == "standard_normal":  # Default distribution
+                noise_model = gen.standard_normal(size=(n, k))
+                di_k = di_k + noise_model
             d_i = median(di_k, axis=1)
             d_i = array([d_i]).T
             # ---------------------------------------------------------------------
             # Estimation part
             # ---------------------------------------------------------------------
             xi_est = zeros(shape=(3, n))
             phi_i = zeros(shape=(n, 1))
@@ -137,20 +166,20 @@
             a_1 = u_i.T
             b_1 = d_i + (sum(u_i * arr_a_i).T.reshape(n, 1))
             w_i = asarray((1 / d_i) / (sum(1 / d_i)))
             w = asarray(eye(n) * scimath.sqrt(w_i))
             a_loc = dot(w, a_1)
             b_loc = dot(w, b_1)
             x_est = asarray(solve(dot(a_loc.T, a_loc) + (1 * 10 ** (-6)) * eye(3), dot(a_loc.T, b_loc)))
-            estimated_trajectory.append(x_est[:, 0])
+            estimated_positions.append(x_est[:, 0])
             true_trajectory.append(x_true.copy())
             uav_velocity = _velocity(x_est[:, 0], arr_destinations[ww, :], v_max, tau, gamma)
             x_true[0] = x_true[0] + uav_velocity[0]
             x_true[1] = x_true[1] + uav_velocity[1]
             x_true[2] = x_true[2] + uav_velocity[2]
             distance = math.sqrt(
                 (x_true[0] - arr_destinations[ww][0]) ** 2
                 + (x_true[1] - arr_destinations[ww][1]) ** 2
                 + (x_true[2] - arr_destinations[ww][2]) ** 2
             )
         ww += 1
-    return array([array(estimated_trajectory), array(true_trajectory)])
+    return array([array(estimated_positions), array(true_trajectory)])
```

### Comparing `autonav-1.0.2/autonav/file_handlers.py` & `autonav-1.0.3/autonav/file_handlers.py`

 * *Files identical despite different names*

### Comparing `autonav-1.0.2/autonav/metrics.py` & `autonav-1.0.3/autonav/metrics.py`

 * *Files identical despite different names*

### Comparing `autonav-1.0.2/autonav/plots.py` & `autonav-1.0.3/autonav/plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 """This module contains the plotting functions."""
 
 from typing import List, Optional
 
+import matplotlib.pylab as pylab
 import matplotlib.pyplot as plt
 from numpy import asarray
 from numpy.typing import ArrayLike, NDArray
 
 from .metrics import compute_rmse
 
+# Parameters for plots
+params = {
+    "legend.fontsize": "xx-large",
+    "figure.figsize": (15, 5),
+    "axes.labelsize": "xx-large",
+    "axes.titlesize": "xx-large",
+    "xtick.labelsize": "medium",
+    "ytick.labelsize": "medium",
+}
+pylab.rcParams.update(params)
+
 
 def plot_trajectories(
     ideal_trajectory: ArrayLike,
     estimated_trajectories: List[ArrayLike],
     a_i: ArrayLike,
     names_of_the_algorithms: Optional[List[str]] = None,
 ) -> list:
     """Plots the ideal and estimated trajectory for one or more algorithms.
 
     Args:
         ideal_trajectory: The ideal trajectory that the UAV is supposed to follow.
-        estimated_trajectories: The estimated trajectory that the UAV followed using the GTRS algorithm.
+        estimated_trajectories: The estimated trajectory that the UAV followed using an algorithm.
         names_of_the_algorithms: The names of the algorithms in the same order as in estimated_trajectories.
         a_i: The position of the anchors.
 
     Returns:
         A list of Matplotlib Axes object containing the ideal and estimated trajectory comparison.
     """
     # Transform inputs in NDArray
@@ -41,15 +53,15 @@
             ax = plt.axes(projection="3d")
             a_i_label = "a_i"
             for i in range(0, arr_a_i.shape[1]):
                 ax.plot(
                     arr_a_i[0][i],
                     arr_a_i[1][i],
                     arr_a_i[2][i],
-                    marker="s",
+                    "s",
                     markersize=10,
                     markeredgecolor="black",
                     markerfacecolor="black",
                     label=a_i_label,
                 )
                 a_i_label = "_nolegend_"  # Legend only in the first iteration
             ax.plot(
@@ -61,19 +73,18 @@
                 linewidth=3.0,
                 alpha=0.7,
             )
             ax.plot(
                 arr_estimated_trajectories[:, 0],
                 arr_estimated_trajectories[:, 1],
                 arr_estimated_trajectories[:, 2],
-                label="Estimated Trajectory " + names_of_the_algorithms[j],
+                label="Trajectory followed by the UAV using " + names_of_the_algorithms[j],
                 color="red",
                 alpha=1.0,
             )
-            ax.set_title("Estimated Trajectory " + names_of_the_algorithms[j])
             ax.set_xlabel("Width (m)")
             ax.set_ylabel("Length (m)")
             ax.set(zlabel="Heigth (m)")
             ax.legend()
             axes.append(ax)
         return axes
     else:
```

### Comparing `autonav-1.0.2/autonav/velocity.py` & `autonav-1.0.3/autonav/velocity.py`

 * *Files identical despite different names*

### Comparing `autonav-1.0.2/autonav.egg-info/PKG-INFO` & `autonav-1.0.3/autonav.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonav
-Version: 1.0.2
+Version: 1.0.3
 Summary: Research software for navigating a UAV in indoor environments
 Author-email: "Ricardo S. Santos" <p6221@ulusofona.pt>
 License: MIT
 Project-URL: Bug Reports, https://github.com/ricardo-s-santos/AutoNAV/issues
 Project-URL: Documentation, https://ricardo-s-santos.github.io/AutoNAV/
 Project-URL: Source, https://github.com/ricardo-s-santos/AutoNAV
 Keywords: UAV,Navigation,Indoor
@@ -88,35 +88,53 @@
     [0, 0, b / 8],
     [0, b, b / 8],
     [b / 2, 0, b / 8],
     [b / 2, b, b / 8],]
     ).T
 # Number of measurement samples
 k = 50
-# Noise standard deviation
-sigma = 1
 # Maximum velocity allowed to the UAV
 v_max = b / 100
 # Distance threshold
 tau = b / 50
 # Smoothing factor
 gamma = b / 100
 # Initial position of the UAV
 initial_uav_position = [10, 10, 5]
 # File containing the waypoints
 destinations = readpathfile("docs/docs/examples/Path.csv")
+# Noise seed
+noise_seed = 1
+# Noise Distribution
+noise_distribution = "normal"
+# Noise distribution parameters
+mean = 0
+std = 1
+noise_distribution_parameters = [mean, std]
 ```
 
 Finally, run the GTRS or WLS algorithm and plot the trajectories:
 
 ```python
-# Estimate the trajectory using the GTRS algorithm
-[estimated_trajectory, true_trajectory] = gtrs(a_i, n, k, sigma, destinations, initial_uav_position, v_max, tau, gamma)
-# Plot the estimated trajectory
-plot_trajectories(destinations, [estimated_trajectory], a_i, ['GTRS'])
+# Estimate the positions and trajectory using the GTRS algorithm
+[estimated_positions, true_trajectory] = gtrs(
+    a_i,
+    n,
+    k,
+    destinations,
+    initial_uav_position,
+    v_max,
+    tau,
+    gamma,
+    noise_seed,
+    noise_distribution,
+    noise_distribution_parameters,
+)
+# Plot the trajectory that the UAV followed
+plot_trajectories(destinations, [true_trajectory], a_i, ['GTRS'])
 plt.show()
 ```
 
 <p align="center">
   <img src="https://github.com/ricardo-s-santos/AutoNAV/blob/main/docs/docs/figures/trajectories_plot.png?raw=true" alt="image" width="auto" height="auto">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autonav Version: 1.0.2 Summary: Research software
+Metadata-Version: 2.1 Name: autonav Version: 1.0.3 Summary: Research software
 for navigating a UAV in indoor environments Author-email: "Ricardo S. Santos"
 ulusofona.pt> License: MIT Project-URL: Bug Reports, https://github.com/
 ricardo-s-santos/AutoNAV/issues Project-URL: Documentation, https://ricardo-s-
 santos.github.io/AutoNAV/ Project-URL: Source, https://github.com/ricardo-s-
 santos/AutoNAV Keywords: UAV,Navigation,Indoor Classifier: Development Status
 :: 5 - Production/Stable Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
@@ -34,25 +34,28 @@
 the package one can import the algorithms and necessary dependencies as
 follows: ```python import matplotlib.pyplot as plt from autonav import gtrs,
 wls from autonav.file_handlers import readpathfile from autonav.plots import
 plot_trajectories from numpy import array ``` Afterwards, one can create the
 necessary values to run the algorithms: ```python # Area border b = 200 #
 Number of anchors n = 8 # Position of the anchors a_i = array( [ [0, 0, 0], [0,
 b, 0], [b / 2, 0, 0], [b / 2, b, 0], [0, 0, b / 8], [0, b, b / 8], [b / 2, 0, b
-/ 8], [b / 2, b, b / 8],] ).T # Number of measurement samples k = 50 # Noise
-standard deviation sigma = 1 # Maximum velocity allowed to the UAV v_max = b /
-100 # Distance threshold tau = b / 50 # Smoothing factor gamma = b / 100 #
-Initial position of the UAV initial_uav_position = [10, 10, 5] # File
-containing the waypoints destinations = readpathfile("docs/docs/examples/
-Path.csv") ``` Finally, run the GTRS or WLS algorithm and plot the
-trajectories: ```python # Estimate the trajectory using the GTRS algorithm
-[estimated_trajectory, true_trajectory] = gtrs(a_i, n, k, sigma, destinations,
-initial_uav_position, v_max, tau, gamma) # Plot the estimated trajectory
-plot_trajectories(destinations, [estimated_trajectory], a_i, ['GTRS']) plt.show
-() ```
+/ 8], [b / 2, b, b / 8],] ).T # Number of measurement samples k = 50 # Maximum
+velocity allowed to the UAV v_max = b / 100 # Distance threshold tau = b / 50 #
+Smoothing factor gamma = b / 100 # Initial position of the UAV
+initial_uav_position = [10, 10, 5] # File containing the waypoints destinations
+= readpathfile("docs/docs/examples/Path.csv") # Noise seed noise_seed = 1 #
+Noise Distribution noise_distribution = "normal" # Noise distribution
+parameters mean = 0 std = 1 noise_distribution_parameters = [mean, std] ```
+Finally, run the GTRS or WLS algorithm and plot the trajectories: ```python #
+Estimate the positions and trajectory using the GTRS algorithm
+[estimated_positions, true_trajectory] = gtrs( a_i, n, k, destinations,
+initial_uav_position, v_max, tau, gamma, noise_seed, noise_distribution,
+noise_distribution_parameters, ) # Plot the trajectory that the UAV followed
+plot_trajectories(destinations, [true_trajectory], a_i, ['GTRS']) plt.show()
+```
                                     [image]
 ## References [1] J. P. Matos-Carvalho, R. Santos, S. Tomic and M. Beko, "GTRS-
 Based Algorithm for UAV Navigation in Indoor Environments Employing Range
 Measurements and Odometry," in IEEE Access, vol. 9, pp. 89120-89132, 2021, doi:
 10.1109/ACCESS.2021.3089900. https://ieeexplore.ieee.org/document/9456863 [2]
 R. Santos, J. P. Matos-Carvalho, S. Tomic and M. Beko, "WLS algorithm for UAV
 navigation in satelliteâless environments," in IET Wireless Sensor Systems,
```

### Comparing `autonav-1.0.2/pyproject.toml` & `autonav-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autonav"
-version = "1.0.2"
+version = "1.0.3"
 description = "Research software for navigating a UAV in indoor environments"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["UAV", "Navigation", "Indoor"]
 license = { text = "MIT" }
 authors = [{ name = "Ricardo S. Santos", email = "p6221@ulusofona.pt" }]
 classifiers = [
```

### Comparing `autonav-1.0.2/tests/test_GTRS.py` & `autonav-1.0.3/tests/test_GTRS.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,243 +5,239 @@
 import pytest
 from numpy import array
 from numpy.testing import assert_allclose, assert_array_equal
 
 from autonav.GTRS import _calc_eigen, gtrs
 
 
-@pytest.mark.critical()
-def test_gtrs_no_noise(default_values, expected_trajectories_gtrs_sigma_0):
+@pytest.mark.critical
+def test_gtrs_no_noise(default_values, expected_trajectories_gtrs_standard_normal):
     """Tests if the algorithm is correctly implemented by setting the noise to zero."""
     # This test does not use seeds because the noise is set to zero.
     # Values used in test
-    sigma = 0  # Noise STD in meters
     trajectories = gtrs(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
     )
     gtrs_estimated_trajectory = trajectories[0]
     gtrs_true_trajectory = trajectories[1]
-    # With sigma zero the trajectories should be the following ones if one performs the math
-    assert_allclose(expected_trajectories_gtrs_sigma_0[0], gtrs_estimated_trajectory)
-    assert_allclose(expected_trajectories_gtrs_sigma_0[1], gtrs_true_trajectory)
+    assert_allclose(expected_trajectories_gtrs_standard_normal[0], gtrs_estimated_trajectory)
+    assert_allclose(expected_trajectories_gtrs_standard_normal[1], gtrs_true_trajectory)
 
 
-@pytest.mark.critical()
+@pytest.mark.critical
 def test_gtrs_reproducibility(default_values, seeds):
     """Tests if the algorithm is reproducible."""
     # Values used in test
-    sigma = 1  # Noise STD in meters
     trajectories = gtrs(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
         seeds,
     )
     gtrs_estimated_trajectory_1 = trajectories[0]
     gtrs_true_trajectory_1 = trajectories[1]
     # Call GTRS again
     trajectories = gtrs(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
         seeds,
     )
     gtrs_estimated_trajectory_2 = trajectories[0]
     gtrs_true_trajectory_2 = trajectories[1]
     # Check to see if both results are equal
     assert_allclose(gtrs_estimated_trajectory_1, gtrs_estimated_trajectory_2)
     assert_allclose(gtrs_true_trajectory_1, gtrs_true_trajectory_2)
 
 
-@pytest.mark.critical()
+@pytest.mark.critical
 def test_gtrs_exceptions(default_values):
     """Tests if the expected exceptions are raised with wrong arguments."""
-    sigma = 0
     # Case n != size(a_i, axis=1)
     with pytest.raises(ValueError, match=re.escape("The length of a_i must be equal to N.")):
         gtrs(
             default_values.a_i,
             10,
             default_values.k,
-            sigma,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case k < 0
     with pytest.raises(ValueError, match=re.escape("K must be positive.")):
         gtrs(
             default_values.a_i,
             default_values.n,
             -1,
-            sigma,
-            default_values.destinations,
-            default_values.initial_uav_position,
-            default_values.v_max,
-            default_values.tau,
-            default_values.gamma,
-        )
-    # Case sigma < 0
-    with pytest.raises(ValueError, match=re.escape("Sigma must be between 0 and 5.")):
-        gtrs(
-            default_values.a_i,
-            default_values.n,
-            default_values.k,
-            -1,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case destinations with wrong coordinates
     with pytest.raises(ValueError, match=re.escape("Waypoints must contain the 3 coordinates (x, y, z).")):
         gtrs(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             array([[1, 2]]),
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case empty destinations
     with pytest.raises(ValueError, match=re.escape("Waypoints cannot be empty.")):
         gtrs(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             array([]),
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case initial_uav_position with wrong coordinates
     with pytest.raises(ValueError, match=re.escape("Initial UAV position must contain the 3 coordinates (x, y, z).")):
         gtrs(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             default_values.destinations,
             [1, 2],
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Validate optional parameters
     # Case tol < 0
     with pytest.raises(ValueError, match=re.escape("Tolerance must be positive.")):
         gtrs(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
             0,
+            "standard_normal",
+            [],
             -1,
         )
     # Case n_iter < 0
     with pytest.raises(ValueError, match=re.escape("Number of Bisection iterations must be positive.")):
         gtrs(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
             0,
+            "standard_normal",
+            [],
             0.001,
             -1,
         )
     # Case max_lim < 0
     with pytest.raises(
         ValueError, match=re.escape("The maximum value for the interval in the bisection function must be positive.")
     ):
         gtrs(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
             0,
+            "standard_normal",
+            [],
             0.001,
             30,
             -1,
         )
+    # Case wrong distribution
+    with pytest.raises(ValueError, match=re.escape("Noise distribution must be normal, standard_normal, exponential.")):
+        gtrs(
+            default_values.a_i,
+            default_values.n,
+            default_values.k,
+            default_values.destinations,
+            default_values.initial_uav_position,
+            default_values.v_max,
+            default_values.tau,
+            default_values.gamma,
+            0,
+            "exp",
+        )
 
 
-def test_gtrs_optional_parameters(default_values, expected_trajectories_gtrs_sigma_0, seeds):
+def test_gtrs_optional_parameters(
+    default_values, expected_trajectories_gtrs_standard_normal, seeds, noise_distributions, distribution_parameters
+):
     """Tests if the algorithm correctly accepts optional parameters."""
     # Values used in test
-    sigma = 1  # Noise STD in meters
     tol = 0.0015
     n_iter = 35
     max_lim = 1000005.0
+    if noise_distributions == "normal" and distribution_parameters == [10**-3]:
+        distribution_parameters = [0, 1]
     trajectories = gtrs(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
         seeds,
+        noise_distributions,
+        distribution_parameters,
         tol,
         n_iter,
         max_lim,
     )
     gtrs_estimated_trajectory = trajectories[0]
     gtrs_true_trajectory = trajectories[1]
     # Check if the algorithm reach the final position with a tolerance 1 (m) due to noise
-    assert_allclose(expected_trajectories_gtrs_sigma_0[0][-1], gtrs_estimated_trajectory[-1], rtol=1)
-    assert_allclose(expected_trajectories_gtrs_sigma_0[1][-1], gtrs_true_trajectory[-1], rtol=1)
+    assert_allclose(expected_trajectories_gtrs_standard_normal[0][-1], gtrs_estimated_trajectory[-1], rtol=1)
+    assert_allclose(expected_trajectories_gtrs_standard_normal[1][-1], gtrs_true_trajectory[-1], rtol=1)
     # Check to see if the algorithm solved the problem in the expected number of steps
     # Tolerance of ten steps due to noise
-    expected_steps_necessary_estimated_trajectory = len(expected_trajectories_gtrs_sigma_0[0])
-    expected_steps_necessary_true_trajectory = len(expected_trajectories_gtrs_sigma_0[1])
+    expected_steps_necessary_estimated_trajectory = len(expected_trajectories_gtrs_standard_normal[0])
+    expected_steps_necessary_true_trajectory = len(expected_trajectories_gtrs_standard_normal[1])
     steps_necessary_estimated_trajectory = len(trajectories[0])
     steps_necessary_true_trajectory = len(trajectories[1])
     assert expected_steps_necessary_estimated_trajectory <= steps_necessary_estimated_trajectory + 10
     assert expected_steps_necessary_true_trajectory <= steps_necessary_true_trajectory + 10
 
 
 def test_calc_eigen_incorrect_parameters():
```

### Comparing `autonav-1.0.2/tests/test_WLS.py` & `autonav-1.0.3/tests/test_WLS.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,183 +5,177 @@
 import pytest
 from numpy import array
 from numpy.testing import assert_allclose
 
 from autonav.WLS import wls
 
 
-@pytest.mark.critical()
-def test_wls_no_noise(default_values, expected_trajectories_wls_sigma_0):
+@pytest.mark.critical
+def test_wls_no_noise(default_values, expected_trajectories_wls_standard_normal):
     """Tests if the algorithm is correctly implemented by setting the noise to zero."""
     # This test does not use seeds because the noise is set to zero.
     # Values used in test
-    sigma = 0  # Noise STD in meters
     trajectories = wls(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
     )
     wls_estimated_trajectory = trajectories[0]
     wls_true_trajectory = trajectories[1]
     # With sigma zero the trajectories should be the following ones if one performs the math
-    assert_allclose(expected_trajectories_wls_sigma_0[0], wls_estimated_trajectory, rtol=1e-03)
-    assert_allclose(expected_trajectories_wls_sigma_0[1], wls_true_trajectory, rtol=1e-03)
+    assert_allclose(expected_trajectories_wls_standard_normal[0], wls_estimated_trajectory, rtol=1e-03)
+    assert_allclose(expected_trajectories_wls_standard_normal[1], wls_true_trajectory, rtol=1e-03)
 
 
-@pytest.mark.critical()
+@pytest.mark.critical
 def test_wls_reproducibility(default_values, seeds):
     """Tests if the algorithm is reproducible."""
     # Values used in test
-    sigma = 1  # Noise STD in meters
     trajectories = wls(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
         seeds,
     )
     wls_estimated_trajectory_1 = trajectories[0]
     wls_true_trajectory_1 = trajectories[1]
     # Call WLS again
     trajectories = wls(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
         seeds,
     )
     wls_estimated_trajectory_2 = trajectories[0]
     wls_true_trajectory_2 = trajectories[1]
     # Check to see if both results are equal
     assert_allclose(wls_estimated_trajectory_1, wls_estimated_trajectory_2)
     assert_allclose(wls_true_trajectory_1, wls_true_trajectory_2)
 
 
-@pytest.mark.critical()
+@pytest.mark.critical
 def test_wls_exceptions(default_values):
     """Tests if the expected exceptions are raised with wrong arguments."""
-    sigma = 0
     # Case n != size(a_i, axis=1)
     with pytest.raises(ValueError, match=re.escape("The length of a_i must be equal to N.")):
         wls(
             default_values.a_i,
             10,
             default_values.k,
-            sigma,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case k < 0
     with pytest.raises(ValueError, match=re.escape("K must be positive.")):
         wls(
             default_values.a_i,
             default_values.n,
             -1,
-            sigma,
-            default_values.destinations,
-            default_values.initial_uav_position,
-            default_values.v_max,
-            default_values.tau,
-            default_values.gamma,
-        )
-    # Case sigma < 0
-    with pytest.raises(ValueError, match=re.escape("Sigma must be between 0 and 5.")):
-        wls(
-            default_values.a_i,
-            default_values.n,
-            default_values.k,
-            -1,
             default_values.destinations,
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case destinations with wrong coordinates
     with pytest.raises(ValueError, match=re.escape("Waypoints must contain the 3 coordinates (x, y, z).")):
         wls(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             array([[1, 2]]),
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case empty destinations
     with pytest.raises(ValueError, match=re.escape("Waypoints cannot be empty.")):
         wls(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             array([]),
             default_values.initial_uav_position,
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
     # Case initial_uav_position with wrong coordinates
     with pytest.raises(ValueError, match=re.escape("Initial UAV position must contain the 3 coordinates (x, y, z).")):
         wls(
             default_values.a_i,
             default_values.n,
             default_values.k,
-            sigma,
             default_values.destinations,
             [1, 2],
             default_values.v_max,
             default_values.tau,
             default_values.gamma,
         )
+    # Case wrong distribution
+    with pytest.raises(ValueError, match=re.escape("Noise distribution must be normal, standard_normal, exponential.")):
+        wls(
+            default_values.a_i,
+            default_values.n,
+            default_values.k,
+            default_values.destinations,
+            default_values.initial_uav_position,
+            default_values.v_max,
+            default_values.tau,
+            default_values.gamma,
+            0,
+            "exp",
+        )
 
 
-def test_wls_optional_parameters(default_values, expected_trajectories_wls_sigma_0, seeds):
+def test_wls_optional_parameters(
+    default_values, expected_trajectories_wls_standard_normal, seeds, noise_distributions, distribution_parameters
+):
     """Tests if the algorithm correctly accepts optional parameters."""
     # Values used in test
-    sigma = 1  # Noise STD in meters
+    if noise_distributions == "normal" and distribution_parameters == [10**-3]:
+        distribution_parameters = [0, 1]
     trajectories = wls(
         default_values.a_i,
         default_values.n,
         default_values.k,
-        sigma,
         default_values.destinations,
         default_values.initial_uav_position,
         default_values.v_max,
         default_values.tau,
         default_values.gamma,
         seeds,
+        noise_distributions,
+        distribution_parameters,
     )
     wls_estimated_trajectory = trajectories[0]
     wls_true_trajectory = trajectories[1]
     # Check if the algorithm reach the final position with a tolerance 1 (m) due to noise
-    assert_allclose(expected_trajectories_wls_sigma_0[0][-1], wls_estimated_trajectory[-1], rtol=1)
-    assert_allclose(expected_trajectories_wls_sigma_0[1][-1], wls_true_trajectory[-1], rtol=1)
+    assert_allclose(expected_trajectories_wls_standard_normal[0][-1], wls_estimated_trajectory[-1], rtol=1)
+    assert_allclose(expected_trajectories_wls_standard_normal[1][-1], wls_true_trajectory[-1], rtol=1)
     # Check to see if the algorithm solved the problem in the expected number of steps
     # Tolerance of ten steps due to noise
-    expected_steps_necessary_estimated_trajectory = len(expected_trajectories_wls_sigma_0[0])
-    expected_steps_necessary_true_trajectory = len(expected_trajectories_wls_sigma_0[1])
+    expected_steps_necessary_estimated_trajectory = len(expected_trajectories_wls_standard_normal[0])
+    expected_steps_necessary_true_trajectory = len(expected_trajectories_wls_standard_normal[1])
     steps_necessary_estimated_trajectory = len(trajectories[0])
     steps_necessary_true_trajectory = len(trajectories[1])
     assert expected_steps_necessary_estimated_trajectory <= steps_necessary_estimated_trajectory + 10
     assert expected_steps_necessary_true_trajectory <= steps_necessary_true_trajectory + 10
```

### Comparing `autonav-1.0.2/tests/test_file_handlers.py` & `autonav-1.0.3/tests/test_file_handlers.py`

 * *Files identical despite different names*

### Comparing `autonav-1.0.2/tests/test_metrics.py` & `autonav-1.0.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `autonav-1.0.2/tests/test_plots.py` & `autonav-1.0.3/tests/test_plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,57 +5,63 @@
 import pytest
 from numpy import ndarray
 
 from autonav.plots import plot_rmse, plot_trajectories
 
 
 def test_plot_trajectories(
-    default_values, expected_trajectories_gtrs_sigma_0, expected_trajectories_wls_sigma_0, ideal_trajectory
+    default_values,
+    expected_trajectories_gtrs_standard_normal,
+    expected_trajectories_wls_standard_normal,
+    ideal_trajectory,
 ):
     """Tests if the plot_trajectories function returns the correct type."""
     ax = plot_trajectories(
         ideal_trajectory,
-        [expected_trajectories_gtrs_sigma_0[0], expected_trajectories_wls_sigma_0[0]],
+        [expected_trajectories_gtrs_standard_normal[0], expected_trajectories_wls_standard_normal[0]],
         default_values[0],
     )
     assert type(ax) is list
 
 
-def test_plot_rmse(expected_trajectories_gtrs_sigma_0, expected_trajectories_wls_sigma_0):
+def test_plot_rmse(expected_trajectories_gtrs_standard_normal, expected_trajectories_wls_standard_normal):
     """Tests if the plot_rmse function returns the correct type."""
     ax = plot_rmse(
-        [expected_trajectories_gtrs_sigma_0[0], expected_trajectories_gtrs_sigma_0[1]],
-        [expected_trajectories_wls_sigma_0[0], expected_trajectories_wls_sigma_0[1]],
+        [expected_trajectories_gtrs_standard_normal[0], expected_trajectories_gtrs_standard_normal[1]],
+        [expected_trajectories_wls_standard_normal[0], expected_trajectories_wls_standard_normal[1]],
     )
     assert type(ax) is ndarray
 
 
 def test_plot_trajectories_exceptions(
-    default_values, expected_trajectories_gtrs_sigma_0, expected_trajectories_wls_sigma_0, ideal_trajectory
+    default_values,
+    expected_trajectories_gtrs_standard_normal,
+    expected_trajectories_wls_standard_normal,
+    ideal_trajectory,
 ):
     """Tests if the expected exceptions are raised."""
     with pytest.raises(
         ValueError,
         match=re.escape(
             "The number of algorithms must be the same in estimated_trajectories and names_of_the_algorithms."
         ),
     ):
         plot_trajectories(
             ideal_trajectory,
-            [expected_trajectories_gtrs_sigma_0[0], expected_trajectories_wls_sigma_0[0]],
+            [expected_trajectories_gtrs_standard_normal[0], expected_trajectories_wls_standard_normal[0]],
             default_values[0],
             ["GTRS"],
         )
 
 
 def test_plot_rmse_exceptions(
-    expected_trajectories_gtrs_sigma_0, expected_trajectories_wls_sigma_0, metrics_trajectories
+    expected_trajectories_gtrs_standard_normal, expected_trajectories_wls_standard_normal, metrics_trajectories
 ):
     """Tests if the expected exceptions are raised."""
     with pytest.raises(
         ValueError,
         match=re.escape("The number of algorithms must be the same in estimated_trajectories and true_trajectories."),
     ):
         plot_rmse(
-            [expected_trajectories_gtrs_sigma_0[1], expected_trajectories_wls_sigma_0[0]],
-            [expected_trajectories_gtrs_sigma_0[1]],
+            [expected_trajectories_gtrs_standard_normal[1], expected_trajectories_wls_standard_normal[0]],
+            [expected_trajectories_gtrs_standard_normal[1]],
         )
```

### Comparing `autonav-1.0.2/tests/test_velocity.py` & `autonav-1.0.3/tests/test_velocity.py`

 * *Files identical despite different names*


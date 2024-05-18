# Comparing `tmp/blueblack-1.0.1.tar.gz` & `tmp/blueblack-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueblack-1.0.1.tar", max compression
+gzip compressed data, was "blueblack-1.0.2.tar", max compression
```

## Comparing `blueblack-1.0.1.tar` & `blueblack-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      875 2024-05-16 18:31:22.342220 blueblack-1.0.1/README.md
--rw-r--r--   0        0        0      719 2024-05-16 18:32:34.940672 blueblack-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      148 2024-05-12 07:06:56.341139 blueblack-1.0.1/src/blueblack/__init__.py
--rw-r--r--   0        0        0     1693 2024-05-16 17:59:36.783535 blueblack-1.0.1/src/blueblack/config_loading.py
--rw-r--r--   0        0        0      212 2024-05-15 18:04:53.235372 blueblack-1.0.1/src/blueblack/local_logging.py
--rw-r--r--   0        0        0     2389 2024-05-15 18:55:37.015728 blueblack-1.0.1/src/blueblack/main.py
--rw-r--r--   0        0        0       27 2024-05-15 11:40:52.398719 blueblack-1.0.1/src/blueblack/project.py
--rw-r--r--   0        0        0     2125 2024-05-15 18:44:25.552205 blueblack-1.0.1/src/blueblack/script_runner.py
--rw-r--r--   0        0        0      134 2024-05-15 18:05:36.175687 blueblack-1.0.1/src/blueblack/states.py
--rw-r--r--   0        0        0      341 2024-05-15 11:40:52.398719 blueblack-1.0.1/src/blueblack/sun_times.py
--rw-r--r--   0        0        0     3148 2024-05-15 11:43:14.666326 blueblack-1.0.1/src/blueblack/suntimes_fetcher.py
--rw-r--r--   0        0        0     1492 2024-05-15 18:06:03.445872 blueblack-1.0.1/src/blueblack/transitions.py
--rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 blueblack-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      876 2024-05-18 08:42:28.073963 blueblack-1.0.2/README.md
+-rw-r--r--   0        0        0      582 2024-05-18 10:48:34.705033 blueblack-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      148 2024-05-12 07:06:56.341139 blueblack-1.0.2/src/blueblack/__init__.py
+-rw-r--r--   0        0        0     1693 2024-05-16 17:59:36.783535 blueblack-1.0.2/src/blueblack/config_loading.py
+-rw-r--r--   0        0        0      212 2024-05-15 18:04:53.235372 blueblack-1.0.2/src/blueblack/local_logging.py
+-rw-r--r--   0        0        0     2340 2024-05-18 08:38:21.782415 blueblack-1.0.2/src/blueblack/main.py
+-rw-r--r--   0        0        0       27 2024-05-15 11:40:52.398719 blueblack-1.0.2/src/blueblack/project.py
+-rw-r--r--   0        0        0     2125 2024-05-15 18:44:25.552205 blueblack-1.0.2/src/blueblack/script_runner.py
+-rw-r--r--   0        0        0      134 2024-05-15 18:05:36.175687 blueblack-1.0.2/src/blueblack/states.py
+-rw-r--r--   0        0        0      678 2024-05-18 08:35:41.909384 blueblack-1.0.2/src/blueblack/sun_times.py
+-rw-r--r--   0        0        0     3148 2024-05-15 11:43:14.666326 blueblack-1.0.2/src/blueblack/suntimes_fetcher.py
+-rw-r--r--   0        0        0     1492 2024-05-15 18:06:03.445872 blueblack-1.0.2/src/blueblack/transitions.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 blueblack-1.0.2/PKG-INFO
```

### Comparing `blueblack-1.0.1/README.md` & `blueblack-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 ```
 
 and change the update_days to something appropriate (e.g. 10 days).
 
 When it's slightly past sunrise or sunset time (around 5 seconds), executable scripts inside `XDG_CONFIG_HOME/blueblack/{dark,light}_mode` will run automatically.
 Some examples are provided in [the source code page](https://github.com/smitropoulos/blueblack/tree/main/configs)
 
-Internally, Blueblack will use [the Sunrise-sunset API](https://sunrise-sunset.org/api) which is currently free. Please use this responsibly so we can have free things.
+Internally, Blueblack will use [the Sunrise-sunset API](https://sunrise-sunset.org/api) which is currently free. Please use this responsibly, so we can have free things.
```

### Comparing `blueblack-1.0.1/pyproject.toml` & `blueblack-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 [tool.poetry]
 name = "blueblack"
-version = "1.0.1"
+version = "1.0.2"
 description = "Automatic light/dark mode transitions based on location"
 authors = ["Stefanos Mitropoulos"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
-certifi = "2024.2.2"
-charset-normalizer = "3.3.2"
-idna = "3.7"
-iniconfig = "2.0.0"
-packaging = "24.0"
-pluggy = "1.5.0"
 pyyaml = "6.0.1"
 requests = "2.31.0"
-urllib3 = "2.2.1"
 xdg-base-dirs = "6.0.1"
 jsonschema = "^4.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 requests-mock = "^1.12.1"
```

### Comparing `blueblack-1.0.1/src/blueblack/config_loading.py` & `blueblack-1.0.2/src/blueblack/config_loading.py`

 * *Files identical despite different names*

### Comparing `blueblack-1.0.1/src/blueblack/main.py` & `blueblack-1.0.2/src/blueblack/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,18 +45,18 @@
                 transition.execute(State.LIGHT, script_runner)
             else:
                 transition.execute(State.DARK, script_runner)
 
         elif transition.last_transition != next_transition:
             # check if we are past the time for a transition
             if next_transition == State.DARK:
-                if now_time > suntimes.sunset_time or now_time < suntimes.sunrise_time:
+                if suntimes.now_is_outside_sun_times(now_time):
                     transition.execute(State.DARK, script_runner)
             if next_transition == State.LIGHT:
-                if now_time > suntimes.sunrise_time and now_time < suntimes.sunset_time:
+                if suntimes.now_is_between_sun_times(now_time):
                     transition.execute(State.LIGHT, script_runner)
 
         # check if it is time to update the sunrise, sunset times
         if seconds_rem <= 0:
             suntimes = suntimes_fetcher.fetch_sun_times()
             seconds_rem = seconds_in_day
         else:
```

### Comparing `blueblack-1.0.1/src/blueblack/script_runner.py` & `blueblack-1.0.2/src/blueblack/script_runner.py`

 * *Files identical despite different names*

### Comparing `blueblack-1.0.1/src/blueblack/suntimes_fetcher.py` & `blueblack-1.0.2/src/blueblack/suntimes_fetcher.py`

 * *Files identical despite different names*

### Comparing `blueblack-1.0.1/src/blueblack/transitions.py` & `blueblack-1.0.2/src/blueblack/transitions.py`

 * *Files identical despite different names*

### Comparing `blueblack-1.0.1/PKG-INFO` & `blueblack-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 Metadata-Version: 2.1
 Name: blueblack
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automatic light/dark mode transitions based on location
 Author: Stefanos Mitropoulos
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: certifi (==2024.2.2)
-Requires-Dist: charset-normalizer (==3.3.2)
-Requires-Dist: idna (==3.7)
-Requires-Dist: iniconfig (==2.0.0)
 Requires-Dist: jsonschema (>=4.22.0,<5.0.0)
-Requires-Dist: packaging (==24.0)
-Requires-Dist: pluggy (==1.5.0)
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: urllib3 (==2.2.1)
 Requires-Dist: xdg-base-dirs (==6.0.1)
 Description-Content-Type: text/markdown
 
 # Blueblack
 
 Automatically change to light and dark mode depending on your location.
 
@@ -33,9 +26,9 @@
 ```
 
 and change the update_days to something appropriate (e.g. 10 days).
 
 When it's slightly past sunrise or sunset time (around 5 seconds), executable scripts inside `XDG_CONFIG_HOME/blueblack/{dark,light}_mode` will run automatically.
 Some examples are provided in [the source code page](https://github.com/smitropoulos/blueblack/tree/main/configs)
 
-Internally, Blueblack will use [the Sunrise-sunset API](https://sunrise-sunset.org/api) which is currently free. Please use this responsibly so we can have free things.
+Internally, Blueblack will use [the Sunrise-sunset API](https://sunrise-sunset.org/api) which is currently free. Please use this responsibly, so we can have free things.
```


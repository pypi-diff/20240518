# Comparing `tmp/openagents_node_sdk-0.3.4.tar.gz` & `tmp/openagents_node_sdk-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.3.4.tar", last modified: Mon May 13 09:45:43 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.3.5.tar", last modified: Sat May 18 08:29:13 2024, max compression
```

## Comparing `openagents_node_sdk-0.3.4.tar` & `openagents_node_sdk-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:43.674217 openagents_node_sdk-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 09:45:43.674217 openagents_node_sdk-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:45:36.000000 openagents_node_sdk-0.3.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:43.674217 openagents_node_sdk-0.3.4/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/JobContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:43.674217 openagents_node_sdk-0.3.4/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 09:45:43.000000 openagents_node_sdk-0.3.4/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 09:45:43.000000 openagents_node_sdk-0.3.4/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:45:43.000000 openagents_node_sdk-0.3.4/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 09:45:43.000000 openagents_node_sdk-0.3.4/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 09:45:43.000000 openagents_node_sdk-0.3.4/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:45:43.674217 openagents_node_sdk-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 09:45:35.000000 openagents_node_sdk-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/JobContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 08:29:13.000000 openagents_node_sdk-0.3.5/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 08:29:13.567087 openagents_node_sdk-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-18 08:29:04.000000 openagents_node_sdk-0.3.5/setup.py
```

### Comparing `openagents_node_sdk-0.3.4/LICENSE` & `openagents_node_sdk-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/README.md` & `openagents_node_sdk-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/Disk.py` & `openagents_node_sdk-0.3.5/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/DiskReader.py` & `openagents_node_sdk-0.3.5/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/DiskWriter.py` & `openagents_node_sdk-0.3.5/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/JobContext.py` & `openagents_node_sdk-0.3.5/openagents/JobContext.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/JobRunner.py` & `openagents_node_sdk-0.3.5/openagents/JobRunner.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/Logger.py` & `openagents_node_sdk-0.3.5/openagents/Logger.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/NodeConfig.py` & `openagents_node_sdk-0.3.5/openagents/NodeConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.3.5/openagents/OpenAgentsNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,17 +328,17 @@
 
     async def _run(self, poolAddress=None, poolPort=None, poolSsl=False):
         """
         Internal method to run the node.
         Should not be called, use start() instead.
         """
         await asyncio.sleep(5000.0/1000.0)
-        self.poolAddress = poolAddress or os.getenv('POOL_ADDRESS', "127.0.0.1")
-        self.poolPort = poolPort or int(os.getenv('POOL_PORT', "5000"))
-        self.poolSsl = poolSsl or os.getenv('POOL_SSL', "false")== "true"
+        self.poolAddress = poolAddress or os.getenv('POOL_ADDRESS', "playground.openagents.com")
+        self.poolPort = poolPort or int(os.getenv('POOL_PORT', "6021"))
+        self.poolSsl = poolSsl or os.getenv('POOL_SSL', "true")== "true"
         self.loopInterval = 1000.0/int(os.getenv('NODE_TPS', "10"))
 
         await self._loop()
         await self.reannounce()
         while True:
             await self._executePendingJob()
             await asyncio.sleep(1000.0/1000.0)
```

### Comparing `openagents_node_sdk-0.3.4/openagents/RunnerConfig.py` & `openagents_node_sdk-0.3.5/openagents/RunnerConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.4/setup.py` & `openagents_node_sdk-0.3.5/setup.py`

 * *Files identical despite different names*


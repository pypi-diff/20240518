# Comparing `tmp/crawler_user_agents-0.2.0.tar.gz` & `tmp/crawler_user_agents-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_user_agents-0.2.0.tar", last modified: Sat May 18 08:15:57 2024, max compression
+gzip compressed data, was "crawler_user_agents-0.3.0.tar", last modified: Sat May 18 08:27:05 2024, max compression
```

## Comparing `crawler_user_agents-0.2.0.tar` & `crawler_user_agents-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:15:57.691193 crawler_user_agents-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 08:15:57.691193 crawler_user_agents-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/composer.json
--rw-r--r--   0 runner    (1001) docker     (127)   171732 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/crawler-user-agents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:15:57.691193 crawler_user_agents-0.2.0/crawler_user_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-18 08:15:57.000000 crawler_user_agents-0.2.0/crawler_user_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 08:15:57.000000 crawler_user_agents-0.2.0/crawler_user_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 08:15:57.000000 crawler_user_agents-0.2.0/crawler_user_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 08:15:57.000000 crawler_user_agents-0.2.0/crawler_user_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    63625 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-18 08:15:50.000000 crawler_user_agents-0.2.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-18 08:15:53.000000 crawler_user_agents-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 08:15:57.691193 crawler_user_agents-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:27:05.412680 crawler_user_agents-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-18 08:27:05.412680 crawler_user_agents-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/composer.json
+-rw-r--r--   0 runner    (1001) docker     (127)   171732 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/crawler-user-agents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:27:05.412680 crawler_user_agents-0.3.0/crawler_user_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-18 08:27:05.000000 crawler_user_agents-0.3.0/crawler_user_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 08:27:05.000000 crawler_user_agents-0.3.0/crawler_user_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 08:27:05.000000 crawler_user_agents-0.3.0/crawler_user_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 08:27:05.000000 crawler_user_agents-0.3.0/crawler_user_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    63625 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-18 08:26:58.000000 crawler_user_agents-0.3.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-18 08:27:01.000000 crawler_user_agents-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 08:27:05.412680 crawler_user_agents-0.3.0/setup.cfg
```

### Comparing `crawler_user_agents-0.2.0/LICENSE` & `crawler_user_agents-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_user_agents-0.2.0/PKG-INFO` & `crawler_user_agents-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: crawler-user-agents
-Version: 0.2.0
+Version: 0.3.0
 Author-email: Martin Monperrus <martin.monperrus@gnieh.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # crawler-user-agents
 
 This repository contains a list of of HTTP user-agents used by robots, crawlers, and spiders as in single JSON file.
 
+* NPM package: <https://www.npmjs.com/package/crawler-user-agents>
+* Go package: <https://pkg.go.dev/github.com/monperrus/crawler-user-agents>
+* PyPi package: <https://pypi.org/project/crawler-user-agents/>
+
 ## Install
 
 ### Direct download
 
 Download the [`crawler-user-agents.json` file](https://raw.githubusercontent.com/monperrus/crawler-user-agents/master/crawler-user-agents.json) from this repository directly.
 
 ### Npm / Yarn
```

### Comparing `crawler_user_agents-0.2.0/README.md` & `crawler_user_agents-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # crawler-user-agents
 
 This repository contains a list of of HTTP user-agents used by robots, crawlers, and spiders as in single JSON file.
 
+* NPM package: <https://www.npmjs.com/package/crawler-user-agents>
+* Go package: <https://pkg.go.dev/github.com/monperrus/crawler-user-agents>
+* PyPi package: <https://pypi.org/project/crawler-user-agents/>
+
 ## Install
 
 ### Direct download
 
 Download the [`crawler-user-agents.json` file](https://raw.githubusercontent.com/monperrus/crawler-user-agents/master/crawler-user-agents.json) from this repository directly.
 
 ### Npm / Yarn
```

### Comparing `crawler_user_agents-0.2.0/composer.json` & `crawler_user_agents-0.3.0/composer.json`

 * *Files identical despite different names*

### Comparing `crawler_user_agents-0.2.0/crawler-user-agents.json` & `crawler_user_agents-0.3.0/crawler-user-agents.json`

 * *Files identical despite different names*

### Comparing `crawler_user_agents-0.2.0/crawler_user_agents.egg-info/PKG-INFO` & `crawler_user_agents-0.3.0/crawler_user_agents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: crawler-user-agents
-Version: 0.2.0
+Version: 0.3.0
 Author-email: Martin Monperrus <martin.monperrus@gnieh.org>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # crawler-user-agents
 
 This repository contains a list of of HTTP user-agents used by robots, crawlers, and spiders as in single JSON file.
 
+* NPM package: <https://www.npmjs.com/package/crawler-user-agents>
+* Go package: <https://pkg.go.dev/github.com/monperrus/crawler-user-agents>
+* PyPi package: <https://pypi.org/project/crawler-user-agents/>
+
 ## Install
 
 ### Direct download
 
 Download the [`crawler-user-agents.json` file](https://raw.githubusercontent.com/monperrus/crawler-user-agents/master/crawler-user-agents.json) from this repository directly.
 
 ### Npm / Yarn
```

### Comparing `crawler_user_agents-0.2.0/package-lock.json` & `crawler_user_agents-0.3.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `crawler_user_agents-0.2.0/package.json` & `crawler_user_agents-0.3.0/package.json`

 * *Files identical despite different names*


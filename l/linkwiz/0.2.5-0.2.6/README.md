# Comparing `tmp/linkwiz-0.2.5.tar.gz` & `tmp/linkwiz-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkwiz-0.2.5.tar", last modified: Sat May 11 04:09:05 2024, max compression
+gzip compressed data, was "linkwiz-0.2.6.tar", last modified: Sat May 11 04:47:39 2024, max compression
```

## Comparing `linkwiz-0.2.5.tar` & `linkwiz-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    18092 2024-04-23 16:54:37.021744 linkwiz-0.2.5/LICENSE
--rw-r--r--   0        0        0      997 2024-04-23 16:54:37.021744 linkwiz-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-04-23 16:54:37.021744 linkwiz-0.2.5/linkwiz/__init__.py
--rw-r--r--   0        0        0      585 2024-04-23 16:54:37.021744 linkwiz-0.2.5/linkwiz/__main__.py
--rw-r--r--   0        0        0     2236 2024-05-11 04:04:33.517315 linkwiz-0.2.5/linkwiz/browser.py
--rw-r--r--   0        0        0     2774 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/config.py
--rw-r--r--   0        0        0     1300 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/core.py
--rw-r--r--   0        0        0     4007 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/gui.py
--rw-r--r--   0        0        0     1494 2024-04-28 13:37:40.316740 linkwiz-0.2.5/linkwiz/install.py
--rw-r--r--   0        0        0     1360 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/launch.py
--rw-r--r--   0        0        0      853 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/match.py
--rw-r--r--   0        0        0      788 2024-05-11 04:09:05.738196 linkwiz-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 linkwiz-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-23 16:54:37.021744 linkwiz-0.2.6/LICENSE
+-rw-r--r--   0        0        0      997 2024-04-23 16:54:37.021744 linkwiz-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 16:54:37.021744 linkwiz-0.2.6/linkwiz/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-23 16:54:37.021744 linkwiz-0.2.6/linkwiz/__main__.py
+-rw-r--r--   0        0        0     2141 2024-05-11 04:42:19.991694 linkwiz-0.2.6/linkwiz/browser.py
+-rw-r--r--   0        0        0     2774 2024-04-23 16:54:37.025077 linkwiz-0.2.6/linkwiz/config.py
+-rw-r--r--   0        0        0     1300 2024-04-23 16:54:37.025077 linkwiz-0.2.6/linkwiz/core.py
+-rw-r--r--   0        0        0     4007 2024-04-23 16:54:37.025077 linkwiz-0.2.6/linkwiz/gui.py
+-rw-r--r--   0        0        0     1494 2024-04-28 13:37:40.316740 linkwiz-0.2.6/linkwiz/install.py
+-rw-r--r--   0        0        0     1360 2024-04-23 16:54:37.025077 linkwiz-0.2.6/linkwiz/launch.py
+-rw-r--r--   0        0        0      853 2024-04-23 16:54:37.025077 linkwiz-0.2.6/linkwiz/match.py
+-rw-r--r--   0        0        0      788 2024-05-11 04:47:39.180914 linkwiz-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 linkwiz-0.2.6/PKG-INFO
```

### Comparing `linkwiz-0.2.5/LICENSE` & `linkwiz-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/README.md` & `linkwiz-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/__main__.py` & `linkwiz-0.2.6/linkwiz/__main__.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/browser.py` & `linkwiz-0.2.6/linkwiz/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,50 +22,47 @@
 def get_browsers() -> Dict[str, Path]:
     """Get the name and exec path of browsers."""
     try:
         installed_browsers = []
         if config.main.get("auto_find_browsers", True):
             installed_browsers = find_installed_browsers()
 
-            if SELF_DESKTOP in installed_browsers:
-                installed_browsers.remove(SELF_DESKTOP)
+        browsers = get_browser_exec(installed_browsers)
+        browsers.update(config.browsers)
 
-        return get_browser_exec(installed_browsers)
+        return browsers
     except subprocess.CalledProcessError:
         logging.error("Error getting installed browsers")
         exit(1)
 
 
 def find_installed_browsers() -> List[str]:
     """Get the name of installed browsers."""
     installed_browsers = set()
     for path in MIMEINFO_PATHS:
         if not path.exists():
             continue
         with open(path, "r") as f:
-            lines = f.readlines()
-            for line in lines:
+            for line in f:
                 if not line.startswith(HTTP_HANDLER):
                     continue
                 browsers = line.split("=")[-1].strip().split(";")
                 installed_browsers.update(browsers)
                 break
+    installed_browsers.discard(SELF_DESKTOP)
     return list(installed_browsers)
 
 
 def get_browser_exec(browsers_desktop: List[str]) -> Dict[str, Path]:
     """Get the exec path of installed browsers."""
-    installed_browsers: Dict[str, Path] = {}
+    browsers_exec: Dict[str, Path] = {}
     for path in DESKTOP_PATHS:
         if not path.exists():
             continue
         for entry in path.glob("*.desktop"):
             if entry.name not in browsers_desktop:
                 continue
             desktop_entry = DesktopEntry.DesktopEntry(str(entry))
             name: str = desktop_entry.getName()
             execpath: str = desktop_entry.getExec()
-            installed_browsers[name] = Path(execpath)
-
-    installed_browsers.update(config.browsers)
-
-    return installed_browsers
+            browsers_exec[name] = Path(execpath)
+    return browsers_exec
```

### Comparing `linkwiz-0.2.5/linkwiz/config.py` & `linkwiz-0.2.6/linkwiz/config.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/core.py` & `linkwiz-0.2.6/linkwiz/core.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/gui.py` & `linkwiz-0.2.6/linkwiz/gui.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/install.py` & `linkwiz-0.2.6/linkwiz/install.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/launch.py` & `linkwiz-0.2.6/linkwiz/launch.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/linkwiz/match.py` & `linkwiz-0.2.6/linkwiz/match.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.5/pyproject.toml` & `linkwiz-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires-python = "<4.0,>=3.11"
 dependencies = [
     "pyxdg<1.0,>=0.28",
     "tomli-w<2.0.0,>=1.0.0",
     "unalix-rev<1.0.0,>=0.9.1",
 ]
 name = "linkwiz"
-version = "0.2.5"
+version = "0.2.6"
 description = "LinkWiz is a Linux tool that lets users select their preferred browser for opening links."
 readme = "README.md"
 classifiers = [
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
 ]
```

### Comparing `linkwiz-0.2.5/PKG-INFO` & `linkwiz-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkwiz
-Version: 0.2.5
+Version: 0.2.6
 Summary: LinkWiz is a Linux tool that lets users select their preferred browser for opening links.
 Author-Email: Rin <icealtria+github@gmail.com>
 License: GPL-2.0-only
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Project-URL: Repository, https://github.com/icealtria/linkwiz
 Requires-Python: <4.0,>=3.11
```


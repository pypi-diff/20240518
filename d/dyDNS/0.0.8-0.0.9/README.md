# Comparing `tmp/dyDNS-0.0.8.tar.gz` & `tmp/dyDNS-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyDNS-0.0.8.tar", last modified: Sat Apr 16 08:20:42 2022, max compression
+gzip compressed data, was "dyDNS-0.0.9.tar", last modified: Sat Apr 23 00:03:54 2022, max compression
```

## Comparing `dyDNS-0.0.8.tar` & `dyDNS-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-04-16 08:20:42.520269 dyDNS-0.0.8/
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)     3103 2022-04-16 08:20:42.520269 dyDNS-0.0.8/PKG-INFO
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)     2065 2022-04-06 03:42:55.000000 dyDNS-0.0.8/README.md
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)       38 2022-04-16 08:20:42.520269 dyDNS-0.0.8/setup.cfg
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)      926 2022-04-16 08:20:18.000000 dyDNS-0.0.8/setup.py
-drwxrwxr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-04-16 08:20:42.520269 dyDNS-0.0.8/src/
-drwxrwxr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-04-16 08:20:42.520269 dyDNS-0.0.8/src/dyDNS.egg-info/
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)     3103 2022-04-16 08:20:42.000000 dyDNS-0.0.8/src/dyDNS.egg-info/PKG-INFO
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)      199 2022-04-16 08:20:42.000000 dyDNS-0.0.8/src/dyDNS.egg-info/SOURCES.txt
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)        1 2022-04-16 08:20:42.000000 dyDNS-0.0.8/src/dyDNS.egg-info/dependency_links.txt
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)       38 2022-04-16 08:20:42.000000 dyDNS-0.0.8/src/dyDNS.egg-info/entry_points.txt
--rw-rw-r--   0 takefuji  (1000) takefuji  (1000)        6 2022-04-16 08:20:42.000000 dyDNS-0.0.8/src/dyDNS.egg-info/top_level.txt
--rwxr-xr-x   0 takefuji  (1000) takefuji  (1000)     1871 2022-04-16 08:19:55.000000 dyDNS-0.0.8/src/dydns.py
+drwxrwxr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-04-23 00:03:54.629567 dyDNS-0.0.9/
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)     3103 2022-04-23 00:03:54.629567 dyDNS-0.0.9/PKG-INFO
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)     2065 2022-04-06 03:42:55.000000 dyDNS-0.0.9/README.md
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)       38 2022-04-23 00:03:54.629567 dyDNS-0.0.9/setup.cfg
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)      926 2022-04-23 00:03:14.000000 dyDNS-0.0.9/setup.py
+drwxrwxr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-04-23 00:03:54.625567 dyDNS-0.0.9/src/
+drwxrwxr-x   0 takefuji  (1000) takefuji  (1000)        0 2022-04-23 00:03:54.625567 dyDNS-0.0.9/src/dyDNS.egg-info/
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)     3103 2022-04-23 00:03:54.000000 dyDNS-0.0.9/src/dyDNS.egg-info/PKG-INFO
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)      199 2022-04-23 00:03:54.000000 dyDNS-0.0.9/src/dyDNS.egg-info/SOURCES.txt
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)        1 2022-04-23 00:03:54.000000 dyDNS-0.0.9/src/dyDNS.egg-info/dependency_links.txt
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)       38 2022-04-23 00:03:54.000000 dyDNS-0.0.9/src/dyDNS.egg-info/entry_points.txt
+-rw-rw-r--   0 takefuji  (1000) takefuji  (1000)        6 2022-04-23 00:03:54.000000 dyDNS-0.0.9/src/dyDNS.egg-info/top_level.txt
+-rwxr-xr-x   0 takefuji  (1000) takefuji  (1000)     1919 2022-04-23 00:02:41.000000 dyDNS-0.0.9/src/dydns.py
```

### Comparing `dyDNS-0.0.8/PKG-INFO` & `dyDNS-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyDNS
-Version: 0.0.8
+Version: 0.0.9
 Summary: activating dynamicDNS for freedns.afraid.org
 Home-page: https://github.com/ytakefuji/dyDNS
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/dyDNS
 Description: # dyDNS
```

### Comparing `dyDNS-0.0.8/README.md` & `dyDNS-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dyDNS-0.0.8/setup.py` & `dyDNS-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dyDNS",
-    version="0.0.8",
+    version="0.0.9",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="activating dynamicDNS for freedns.afraid.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/dyDNS",
     project_urls={
```

### Comparing `dyDNS-0.0.8/src/dyDNS.egg-info/PKG-INFO` & `dyDNS-0.0.9/src/dyDNS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyDNS
-Version: 0.0.8
+Version: 0.0.9
 Summary: activating dynamicDNS for freedns.afraid.org
 Home-page: https://github.com/ytakefuji/dyDNS
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/dyDNS
 Description: # dyDNS
```

### Comparing `dyDNS-0.0.8/src/dydns.py` & `dyDNS-0.0.9/src/dydns.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,17 @@
  result = str(read_url(url))
  if len(result)==0: os._exit(0)
  domains = []
  name=""
  if result.startswith("ERROR"):
   print("no update")
  else:
-  r=result.split(DOMAIN)[1]
-  ip=r.split('|')[1]
-  ur=r.split('|')[2]
-  result = read_url(ur.strip())
-  print(result.replace('ERROR','No Updated'))
+  if DOMAIN in result:
+   r=result.split(DOMAIN)[1]
+   ip=r.split('|')[1]
+   ur=r.split('|')[2]
+   result = read_url(ur.strip())
+   print(result.replace('ERROR','No Updated'))
+  else: os._exit(0)
 
 if __name__ == "__main__":
  main()
```


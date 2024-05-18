# Comparing `tmp/ldplayer-tools-0.0.2.tar.gz` & `tmp/ldplayer-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldplayer-tools-0.0.2.tar", last modified: Fri May 10 14:37:02 2024, max compression
+gzip compressed data, was "ldplayer-tools-0.0.3.tar", last modified: Sat May 18 13:28:35 2024, max compression
```

## Comparing `ldplayer-tools-0.0.2.tar` & `ldplayer-tools-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:37:02.162047 ldplayer-tools-0.0.2/
--rw-rw-rw-   0        0        0     1092 2024-04-23 11:35:56.000000 ldplayer-tools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1884 2024-05-10 14:37:02.161048 ldplayer-tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1379 2024-05-10 14:22:48.000000 ldplayer-tools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 14:37:02.152048 ldplayer-tools-0.0.2/ldplayer/
--rw-rw-rw-   0        0        0       66 2024-05-10 12:06:42.000000 ldplayer-tools-0.0.2/ldplayer/__init__.py
--rw-rw-rw-   0        0        0     1306 2024-05-10 12:34:45.000000 ldplayer-tools-0.0.2/ldplayer/controller.py
--rw-rw-rw-   0        0        0     4975 2024-05-10 12:31:24.000000 ldplayer-tools-0.0.2/ldplayer/ldplayer.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:37:02.161048 ldplayer-tools-0.0.2/ldplayer_tools.egg-info/
--rw-rw-rw-   0        0        0     1884 2024-05-10 14:37:02.000000 ldplayer-tools-0.0.2/ldplayer_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-10 14:37:02.000000 ldplayer-tools-0.0.2/ldplayer_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:37:02.000000 ldplayer-tools-0.0.2/ldplayer_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-10 14:37:02.000000 ldplayer-tools-0.0.2/ldplayer_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 14:37:02.000000 ldplayer-tools-0.0.2/ldplayer_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 14:37:02.162047 ldplayer-tools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      717 2024-05-10 14:36:59.000000 ldplayer-tools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 13:28:35.905994 ldplayer-tools-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 11:35:56.000000 ldplayer-tools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1884 2024-05-18 13:28:35.904992 ldplayer-tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2024-05-10 14:22:48.000000 ldplayer-tools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 13:28:35.896992 ldplayer-tools-0.0.3/ldplayer/
+-rw-rw-rw-   0        0        0       66 2024-05-10 12:06:42.000000 ldplayer-tools-0.0.3/ldplayer/__init__.py
+-rw-rw-rw-   0        0        0     1306 2024-05-18 12:46:30.000000 ldplayer-tools-0.0.3/ldplayer/controller.py
+-rw-rw-rw-   0        0        0     4975 2024-05-10 12:31:24.000000 ldplayer-tools-0.0.3/ldplayer/ldplayer.py
+drwxrwxrwx   0        0        0        0 2024-05-18 13:28:35.904992 ldplayer-tools-0.0.3/ldplayer_tools.egg-info/
+-rw-rw-rw-   0        0        0     1884 2024-05-18 13:28:35.000000 ldplayer-tools-0.0.3/ldplayer_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-18 13:28:35.000000 ldplayer-tools-0.0.3/ldplayer_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 13:28:35.000000 ldplayer-tools-0.0.3/ldplayer_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-18 13:28:35.000000 ldplayer-tools-0.0.3/ldplayer_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-18 13:28:35.000000 ldplayer-tools-0.0.3/ldplayer_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 13:28:35.905994 ldplayer-tools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      717 2024-05-18 12:51:01.000000 ldplayer-tools-0.0.3/setup.py
```

### Comparing `ldplayer-tools-0.0.2/LICENSE` & `ldplayer-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ldplayer-tools-0.0.2/PKG-INFO` & `ldplayer-tools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldplayer-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is package for ldplayer emulator control software. (unofficial)
 Home-page: https://github.com/mantvmass/ldplayer
 Author: mantvmass (Phumin Maliwan)
 Author-email: kliop2317@gmail.com
 Maintainer: mantvmass (Phumin Maliwan)
 Maintainer-email: kliop2317@gmail.com
 License: UNKNOWN
```

### Comparing `ldplayer-tools-0.0.2/README.md` & `ldplayer-tools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ldplayer-tools-0.0.2/ldplayer/controller.py` & `ldplayer-tools-0.0.3/ldplayer/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     __device = None
     
     
     def __init__(self, device: Device) -> None:
         self.__device = device
     
     
-    def tab(self, x: int, y: int):
+    def tap(self, x: int, y: int):
         """
         Simulates a tap action at the specified coordinates.
 
         :param x: The x-coordinate of the tap action.
         :param y: The y-coordinate of the tap action.
         :return: None
         """
-        return self.__device.shell("input tab {} {}".format(x, y))
+        return self.__device.shell("input tap {} {}".format(x, y))
 
     
     def swipe(self, sx: int, sy: int, ex: int, ey: int, duration: int):
         """
         Simulates a swipe action at the specified coordinates.
 
         :param sx: The starting x-coordinate of the swipe action.
```

### Comparing `ldplayer-tools-0.0.2/ldplayer/ldplayer.py` & `ldplayer-tools-0.0.3/ldplayer/ldplayer.py`

 * *Files identical despite different names*

### Comparing `ldplayer-tools-0.0.2/ldplayer_tools.egg-info/PKG-INFO` & `ldplayer-tools-0.0.3/ldplayer_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldplayer-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is package for ldplayer emulator control software. (unofficial)
 Home-page: https://github.com/mantvmass/ldplayer
 Author: mantvmass (Phumin Maliwan)
 Author-email: kliop2317@gmail.com
 Maintainer: mantvmass (Phumin Maliwan)
 Maintainer-email: kliop2317@gmail.com
 License: UNKNOWN
```

### Comparing `ldplayer-tools-0.0.2/setup.py` & `ldplayer-tools-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "This is package for ldplayer emulator control software. (unofficial)"
 
 setup(
     name="ldplayer-tools",
     packages=find_packages(),
     version=VERSION,
     description=DESCRIPTION,
```


# Comparing `tmp/ctrip-app-ui-0.4.9.tar.gz` & `tmp/ctrip-app-ui-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.4.9.tar", last modified: Sat May 18 14:21:24 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.5.0.tar", last modified: Sat May 18 14:41:34 2024, max compression
```

## Comparing `ctrip-app-ui-0.4.9.tar` & `ctrip-app-ui-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:21:24.890128 ctrip-app-ui-0.4.9/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-18 14:21:24.888132 ctrip-app-ui-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 14:21:24.861188 ctrip-app-ui-0.4.9/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.4.9/capp_ui/__init__.py
--rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.4.9/capp_ui/config.py
--rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.4.9/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.4.9/capp_ui/device.py
--rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.4.9/capp_ui/dir.py
--rw-rw-rw-   0        0        0    44529 2024-05-18 14:20:01.000000 ctrip-app-ui-0.4.9/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.4.9/capp_ui/fee.py
--rw-rw-rw-   0        0        0     5408 2024-05-18 11:39:51.000000 ctrip-app-ui-0.4.9/capp_ui/libs.py
--rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.4.9/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.4.9/capp_ui/platforms.py
--rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.4.9/capp_ui/test.py
--rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.4.9/capp_ui/utils.py
--rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.4.9/capp_ui/validators.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:21:24.886140 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 14:21:24.000000 ctrip-app-ui-0.4.9/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 14:21:24.890128 ctrip-app-ui-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-18 14:21:17.000000 ctrip-app-ui-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:41:34.143525 ctrip-app-ui-0.5.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-18 14:41:34.141529 ctrip-app-ui-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 14:41:34.114598 ctrip-app-ui-0.5.0/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.5.0/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0      736 2024-05-06 07:02:29.000000 ctrip-app-ui-0.5.0/capp_ui/config.py
+-rw-rw-rw-   0        0        0     4060 2024-05-07 16:57:27.000000 ctrip-app-ui-0.5.0/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1664 2024-05-09 13:31:21.000000 ctrip-app-ui-0.5.0/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1391 2024-04-25 08:27:58.000000 ctrip-app-ui-0.5.0/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    44529 2024-05-18 14:41:16.000000 ctrip-app-ui-0.5.0/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.5.0/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     5414 2024-05-18 14:39:38.000000 ctrip-app-ui-0.5.0/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    24821 2024-05-13 17:15:14.000000 ctrip-app-ui-0.5.0/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1719 2024-04-28 16:15:39.000000 ctrip-app-ui-0.5.0/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0      765 2024-04-28 16:02:26.000000 ctrip-app-ui-0.5.0/capp_ui/test.py
+-rw-rw-rw-   0        0        0     5486 2024-05-11 03:13:30.000000 ctrip-app-ui-0.5.0/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     3023 2024-05-11 03:13:43.000000 ctrip-app-ui-0.5.0/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:41:34.139534 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 14:41:33.000000 ctrip-app-ui-0.5.0/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:41:34.143525 ctrip-app-ui-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-18 14:41:30.000000 ctrip-app-ui-0.5.0/setup.py
```

### Comparing `ctrip-app-ui-0.4.9/LICENSE` & `ctrip-app-ui-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/config.py` & `ctrip-app-ui-0.5.0/capp_ui/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/date_extend.py` & `ctrip-app-ui-0.5.0/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/device.py` & `ctrip-app-ui-0.5.0/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/dir.py` & `ctrip-app-ui-0.5.0/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/domain_service.py` & `ctrip-app-ui-0.5.0/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/fee.py` & `ctrip-app-ui-0.5.0/capp_ui/fee.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/libs.py` & `ctrip-app-ui-0.5.0/capp_ui/libs.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         self.action = action
 
     def __call__(self, func: Callable) -> Any:
         def wrapper(*args, **kwargs) -> dict:
             for i in range(self.loop):
                 if i > 0:
                     logger.warning("尝试第{}次{}".format(i, self.action))
-                flag = func(*args, **kwargs)
-                if flag:
-                    break
+                attr = func(*args, **kwargs)
+                if attr:
+                    return attr
                 sleep(self.sleep)
             if self.loop > 2:
                 logger.warning("{}次尝试{}都失败".format(self.loop, self.action))
             return dict()
 
         return wrapper
```

### Comparing `ctrip-app-ui-0.4.9/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.5.0/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/platforms.py` & `ctrip-app-ui-0.5.0/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/test.py` & `ctrip-app-ui-0.5.0/capp_ui/test.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/utils.py` & `ctrip-app-ui-0.5.0/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/capp_ui/validators.py` & `ctrip-app-ui-0.5.0/capp_ui/validators.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.4.9/setup.py` & `ctrip-app-ui-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.4.9',
+    version='0.5.0',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```


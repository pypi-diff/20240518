# Comparing `tmp/pyevaljs3-0.1.1.tar.gz` & `tmp/pyevaljs3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevaljs3-0.1.1.tar", last modified: Mon Mar  4 19:05:11 2024, max compression
+gzip compressed data, was "pyevaljs3-0.1.2.tar", last modified: Sat May 18 11:41:23 2024, max compression
```

## Comparing `pyevaljs3-0.1.1.tar` & `pyevaljs3-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 19:05:11.946573 pyevaljs3-0.1.1/
--rw-rw-rw-   0        0        0     1093 2023-12-13 10:50:19.000000 pyevaljs3-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3332 2024-03-04 19:05:11.943571 pyevaljs3-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2542 2024-03-04 18:42:48.000000 pyevaljs3-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-04 19:05:11.922572 pyevaljs3-0.1.1/pyevaljs3/
--rw-rw-rw-   0        0        0     2565 2024-03-04 18:41:30.000000 pyevaljs3-0.1.1/pyevaljs3/__init__.py
--rw-rw-rw-   0        0        0       55 2024-03-04 19:04:45.000000 pyevaljs3-0.1.1/pyevaljs3/__version__.py
--rw-rw-rw-   0        0        0     1955 2024-03-04 18:03:49.000000 pyevaljs3-0.1.1/pyevaljs3/evaljs.py
--rw-rw-rw-   0        0        0       96 2023-12-13 08:02:55.000000 pyevaljs3-0.1.1/pyevaljs3/exception.py
--rw-rw-rw-   0        0        0     4200 2024-03-04 18:58:31.000000 pyevaljs3-0.1.1/pyevaljs3/runtime.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:05:11.941571 pyevaljs3-0.1.1/pyevaljs3.egg-info/
--rw-rw-rw-   0        0        0     3332 2024-03-04 19:05:11.000000 pyevaljs3-0.1.1/pyevaljs3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-03-04 19:05:11.000000 pyevaljs3-0.1.1/pyevaljs3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 19:05:11.000000 pyevaljs3-0.1.1/pyevaljs3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-04 19:05:11.000000 pyevaljs3-0.1.1/pyevaljs3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-04 19:05:11.946573 pyevaljs3-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1193 2024-03-04 17:52:32.000000 pyevaljs3-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 19:05:11.938571 pyevaljs3-0.1.1/tests/
--rw-rw-rw-   0        0        0      792 2024-03-04 18:42:48.000000 pyevaljs3-0.1.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.752388 pyevaljs3-0.1.2/
+-rw-rw-rw-   0        0        0     1093 2023-12-13 10:50:19.000000 pyevaljs3-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3332 2024-05-18 11:41:23.751387 pyevaljs3-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2542 2024-03-04 18:42:48.000000 pyevaljs3-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.730365 pyevaljs3-0.1.2/pyevaljs3/
+-rw-rw-rw-   0        0        0     2565 2024-03-04 18:41:30.000000 pyevaljs3-0.1.2/pyevaljs3/__init__.py
+-rw-rw-rw-   0        0        0       55 2024-05-18 11:35:06.000000 pyevaljs3-0.1.2/pyevaljs3/__version__.py
+-rw-rw-rw-   0        0        0     1860 2024-05-18 11:31:35.000000 pyevaljs3-0.1.2/pyevaljs3/evaljs.py
+-rw-rw-rw-   0        0        0       96 2023-12-13 08:02:55.000000 pyevaljs3-0.1.2/pyevaljs3/exception.py
+-rw-rw-rw-   0        0        0     4200 2024-03-04 18:58:31.000000 pyevaljs3-0.1.2/pyevaljs3/runtime.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.749387 pyevaljs3-0.1.2/pyevaljs3.egg-info/
+-rw-rw-rw-   0        0        0     3332 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:41:23.753388 pyevaljs3-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2024-03-04 17:52:32.000000 pyevaljs3-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.748386 pyevaljs3-0.1.2/tests/
+-rw-rw-rw-   0        0        0      792 2024-03-04 18:42:48.000000 pyevaljs3-0.1.2/tests/test.py
```

### Comparing `pyevaljs3-0.1.1/LICENSE` & `pyevaljs3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.1/PKG-INFO` & `pyevaljs3-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevaljs3
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个依赖node.js来执行js代码的python库
 Home-page: https://github.com/Smawexi/PyevalJS3
 Author: Samwe
 Author-email: 1281722462@qq.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyevaljs3-0.1.1/README.md` & `pyevaljs3-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.1/pyevaljs3/__init__.py` & `pyevaljs3-0.1.2/pyevaljs3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.1/pyevaljs3/evaljs.py` & `pyevaljs3-0.1.2/pyevaljs3/evaljs.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,9 @@
     def call(self, func, *args):
         """
         调用指定的函数, 返回其结果
         :param func: 函数名
         :param args: 函数的参数列表
         :return:
         """
-        if len(args) == 1:
-            args = args[0]
-
-        if isinstance(args, (str, int)):
-            args = [args]
-
-        return self._call(func, list(args))
+        _args = [arg for arg in args]
+        return self._call(func, _args)
```

### Comparing `pyevaljs3-0.1.1/pyevaljs3/runtime.py` & `pyevaljs3-0.1.2/pyevaljs3/runtime.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.1/pyevaljs3.egg-info/PKG-INFO` & `pyevaljs3-0.1.2/pyevaljs3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevaljs3
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个依赖node.js来执行js代码的python库
 Home-page: https://github.com/Smawexi/PyevalJS3
 Author: Samwe
 Author-email: 1281722462@qq.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyevaljs3-0.1.1/setup.py` & `pyevaljs3-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.1/tests/test.py` & `pyevaljs3-0.1.2/tests/test.py`

 * *Files identical despite different names*


# Comparing `tmp/pymonit-1.4.2.tar.gz` & `tmp/pymonit-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.2.tar", last modified: Sat May 18 18:58:51 2024, max compression
+gzip compressed data, was "pymonit-1.4.3.tar", last modified: Sat May 18 19:03:30 2024, max compression
```

## Comparing `pymonit-1.4.2.tar` & `pymonit-1.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 18:58:51.840644 pymonit-1.4.2/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.2/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1927 2024-05-18 18:58:51.840644 pymonit-1.4.2/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1292 2024-05-18 18:58:15.000000 pymonit-1.4.2/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 18:58:51.840644 pymonit-1.4.2/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.2/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.2/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.2/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2054 2024-05-18 18:45:14.000000 pymonit-1.4.2/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.2/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.2/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.2/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.2/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 18:58:51.840644 pymonit-1.4.2/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1927 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 18:58:51.840644 pymonit-1.4.2/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 18:58:48.000000 pymonit-1.4.2/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:03:30.561219 pymonit-1.4.3/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.3/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1904 2024-05-18 19:03:30.561219 pymonit-1.4.3/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1269 2024-05-18 19:01:26.000000 pymonit-1.4.3/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:03:30.561219 pymonit-1.4.3/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.3/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.3/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.3/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2054 2024-05-18 18:45:14.000000 pymonit-1.4.3/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.3/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.3/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.3/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.3/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 19:03:30.561219 pymonit-1.4.3/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1904 2024-05-18 19:03:30.000000 pymonit-1.4.3/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 19:03:30.000000 pymonit-1.4.3/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 19:03:30.000000 pymonit-1.4.3/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 19:03:30.000000 pymonit-1.4.3/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 19:03:30.000000 pymonit-1.4.3/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 19:03:30.561219 pymonit-1.4.3/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 19:03:23.000000 pymonit-1.4.3/setup.py
```

### Comparing `pymonit-1.4.2/LICENSE` & `pymonit-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/PKG-INFO` & `pymonit-1.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.2
+Version: 1.4.3
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -78,19 +78,15 @@
 
         sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify(e)
 
-    num = 0
-    for _ in range(3):
-        num += 1
+    monit.msg("O Script terminou com sucesso.") # whatsapp
 
-    monit.msg(f"Total count in for loop: {num}") # whatsapp
-
-    monit.end()
+    monit.end() # manda sinal de fim sem erros
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.2/README.md` & `pymonit-1.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,19 +59,15 @@
 
         sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify(e)
 
-    num = 0
-    for _ in range(3):
-        num += 1
+    monit.msg("O Script terminou com sucesso.") # whatsapp
 
-    monit.msg(f"Total count in for loop: {num}") # whatsapp
-
-    monit.end()
+    monit.end() # manda sinal de fim sem erros
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.2/monit/config.py` & `pymonit-1.4.3/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/monit/core.py` & `pymonit-1.4.3/monit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/monit/func.py` & `pymonit-1.4.3/monit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/monit/http.py` & `pymonit-1.4.3/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/monit/log2file.py` & `pymonit-1.4.3/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/monit/logger.py` & `pymonit-1.4.3/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.2/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.3/pymonit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.2
+Version: 1.4.3
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -78,19 +78,15 @@
 
         sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify(e)
 
-    num = 0
-    for _ in range(3):
-        num += 1
+    monit.msg("O Script terminou com sucesso.") # whatsapp
 
-    monit.msg(f"Total count in for loop: {num}") # whatsapp
-
-    monit.end()
+    monit.end() # manda sinal de fim sem erros
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.2/setup.py` & `pymonit-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.2',
+    version='1.4.3',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```


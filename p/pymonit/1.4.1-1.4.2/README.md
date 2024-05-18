# Comparing `tmp/pymonit-1.4.1.tar.gz` & `tmp/pymonit-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.4.1.tar", last modified: Sat May 18 17:38:29 2024, max compression
+gzip compressed data, was "pymonit-1.4.2.tar", last modified: Sat May 18 18:58:51 2024, max compression
```

## Comparing `pymonit-1.4.1.tar` & `pymonit-1.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:38:29.110113 pymonit-1.4.1/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.1/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2029 2024-05-18 17:38:29.110113 pymonit-1.4.1/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1394 2024-05-18 17:30:43.000000 pymonit-1.4.1/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:38:29.106779 pymonit-1.4.1/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.1/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.1/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      741 2024-05-18 17:23:53.000000 pymonit-1.4.1/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2013 2024-05-18 17:24:26.000000 pymonit-1.4.1/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.1/monit/http.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      453 2024-05-18 17:31:11.000000 pymonit-1.4.1/monit/init.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.1/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.1/monit/logger.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:38:29.110113 pymonit-1.4.1/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2029 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 17:38:29.000000 pymonit-1.4.1/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 17:38:28.000000 pymonit-1.4.1/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 17:38:29.110113 pymonit-1.4.1/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 17:38:25.000000 pymonit-1.4.1/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 18:58:51.840644 pymonit-1.4.2/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.2/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1927 2024-05-18 18:58:51.840644 pymonit-1.4.2/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1292 2024-05-18 18:58:15.000000 pymonit-1.4.2/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 18:58:51.840644 pymonit-1.4.2/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.2/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.2/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      730 2024-05-18 18:44:31.000000 pymonit-1.4.2/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2054 2024-05-18 18:45:14.000000 pymonit-1.4.2/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.2/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      441 2024-05-18 18:04:46.000000 pymonit-1.4.2/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.2/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.2/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 18:58:51.840644 pymonit-1.4.2/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1927 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 18:58:51.000000 pymonit-1.4.2/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 18:58:51.840644 pymonit-1.4.2/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 18:58:48.000000 pymonit-1.4.2/setup.py
```

### Comparing `pymonit-1.4.1/LICENSE` & `pymonit-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.1/PKG-INFO` & `pymonit-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.1
+Version: 1.4.2
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 **Exemplo arquivo `.monit`:**
 ```bash
 PROJECT='project_name'
 COMPANY='company_name'
 DEV='coder'
 LOCATION='location_name'
 HANDLER_URL='https://example.com'
-PHONE='556199999999'
+PHONE='556199999999' # whatsapp deixe em branco para desativar
 ```
 ### Exemplo de Uso:
 
 **Utilização simples**
 ```python
 import time
 
@@ -58,45 +58,39 @@
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
 
 ```Python
-import time
+from time import sleep
 
 from monit.core import Monitor as monit
 from monit.logger import Logger
 from monit.log2file import Log2File
 
 def main():
 
     Log2File() # Salva todo o log em um arquivo
     log = Logger()
 
     try:
         log.info("Hello, World!")
-        time.sleep(5)
 
+        sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify(e)
 
-    try:
-        time.sleep(2)
-        raise ValueError("This is another a sample error.")
-
-    except Exception as e:
-        monit.notify(e, "Custom message")
-
     num = 0
     for _ in range(3):
         num += 1
-    monit.msg(f"Total count in for loop: {num}")
+
+    monit.msg(f"Total count in for loop: {num}") # whatsapp
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.1/README.md` & `pymonit-1.4.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 **Exemplo arquivo `.monit`:**
 ```bash
 PROJECT='project_name'
 COMPANY='company_name'
 DEV='coder'
 LOCATION='location_name'
 HANDLER_URL='https://example.com'
-PHONE='556199999999'
+PHONE='556199999999' # whatsapp deixe em branco para desativar
 ```
 ### Exemplo de Uso:
 
 **Utilização simples**
 ```python
 import time
 
@@ -39,45 +39,39 @@
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
 
 ```Python
-import time
+from time import sleep
 
 from monit.core import Monitor as monit
 from monit.logger import Logger
 from monit.log2file import Log2File
 
 def main():
 
     Log2File() # Salva todo o log em um arquivo
     log = Logger()
 
     try:
         log.info("Hello, World!")
-        time.sleep(5)
 
+        sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify(e)
 
-    try:
-        time.sleep(2)
-        raise ValueError("This is another a sample error.")
-
-    except Exception as e:
-        monit.notify(e, "Custom message")
-
     num = 0
     for _ in range(3):
         num += 1
-    monit.msg(f"Total count in for loop: {num}")
+
+    monit.msg(f"Total count in for loop: {num}") # whatsapp
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.1/monit/config.py` & `pymonit-1.4.2/monit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.1/monit/func.py` & `pymonit-1.4.2/monit/func.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,45 +4,46 @@
 import datetime
 import traceback
 import platform
 from datetime import datetime
 
 from monit import config
 
-def build_json(msg, err, init_time):
+def build_json(err=None, init_time=None):
     data = {
         "project": config.project,
         "company": config.company,
         "location": config.location,
         "dev": config.dev,
         "stderr": bool(err),
-        "custom_msg": msg,
         "phone": config.phone
     }
 
-    fim = datetime.now()
-    total_time = fim - init_time
-    data["runtime"] = total_time.total_seconds()
-    data["date_init"] = init_time.isoformat()
-    data["date_end"] = fim.isoformat()
+    if init_time:
+        fim = datetime.now()
+        init_time = datetime.now()
+        total_time = fim - init_time
+        data["runtime"] = total_time.total_seconds()
+        data["date_init"] = init_time.isoformat()
+        data["date_end"] = fim.isoformat()
 
     data["cpu"] = _get_cpu_usage()
     data["mem"] = _get_memory_usage()
     data["disk"] = _get_disk_usage()
     data["ping"] = _ping_host()
     data["system"] = platform.system()
 
     if err:
         error = str(err).replace('\n', '')
         data["error"] = error
-        _print_error_to_console(msg, err)
+        _print_error_to_console(err)
 
     return data
 
-def _print_error_to_console(msg, err):
+def _print_error_to_console(err):
     if err:
         tb = traceback.extract_tb(err.__traceback__)
         filename, line, func, text = tb[-1]
         strerror = f"{func}: File \"{filename}\", line {line}\n\t{text}\n\n"
         print(strerror)
 
 def _ping_host():
```

### Comparing `pymonit-1.4.1/monit/http.py` & `pymonit-1.4.2/monit/http.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.1/monit/log2file.py` & `pymonit-1.4.2/monit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.1/monit/logger.py` & `pymonit-1.4.2/monit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.4.1/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.2/pymonit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.4.1
+Version: 1.4.2
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 **Exemplo arquivo `.monit`:**
 ```bash
 PROJECT='project_name'
 COMPANY='company_name'
 DEV='coder'
 LOCATION='location_name'
 HANDLER_URL='https://example.com'
-PHONE='556199999999'
+PHONE='556199999999' # whatsapp deixe em branco para desativar
 ```
 ### Exemplo de Uso:
 
 **Utilização simples**
 ```python
 import time
 
@@ -58,45 +58,39 @@
 if __name__ == "__main__":
     main()
 ```
 
 **Utilização avançada**
 
 ```Python
-import time
+from time import sleep
 
 from monit.core import Monitor as monit
 from monit.logger import Logger
 from monit.log2file import Log2File
 
 def main():
 
     Log2File() # Salva todo o log em um arquivo
     log = Logger()
 
     try:
         log.info("Hello, World!")
-        time.sleep(5)
 
+        sleep(2)
         raise ValueError("This is a sample error.")
 
     except Exception as e:
         monit.notify(e)
 
-    try:
-        time.sleep(2)
-        raise ValueError("This is another a sample error.")
-
-    except Exception as e:
-        monit.notify(e, "Custom message")
-
     num = 0
     for _ in range(3):
         num += 1
-    monit.msg(f"Total count in for loop: {num}")
+
+    monit.msg(f"Total count in for loop: {num}") # whatsapp
 
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.4.1/setup.py` & `pymonit-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.4.1',
+    version='1.4.2',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```


# Comparing `tmp/pymonit-1.3.21.tar.gz` & `tmp/pymonit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.21.tar", last modified: Thu May 16 15:22:21 2024, max compression
+gzip compressed data, was "pymonit-1.4.0.tar", last modified: Sat May 18 17:28:05 2024, max compression
```

## Comparing `pymonit-1.3.21.tar` & `pymonit-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 15:22:21.966981 pymonit-1.3.21/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.21/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2223 2024-05-16 15:22:21.966981 pymonit-1.3.21/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1587 2024-05-16 15:21:50.000000 pymonit-1.3.21/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 15:22:21.963648 pymonit-1.3.21/monit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.21/monit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.21/monit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      725 2024-05-16 12:44:15.000000 pymonit-1.3.21/monit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-16 12:44:25.000000 pymonit-1.3.21/monit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.21/monit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3128 2024-05-16 12:41:20.000000 pymonit-1.3.21/monit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.21/monit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.21/monit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.21/monit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-16 15:22:21.966981 pymonit-1.3.21/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2223 2024-05-16 15:22:21.000000 pymonit-1.3.21/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      329 2024-05-16 15:22:21.000000 pymonit-1.3.21/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-16 15:22:21.000000 pymonit-1.3.21/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-16 15:22:21.000000 pymonit-1.3.21/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-16 15:22:21.000000 pymonit-1.3.21/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-16 15:22:21.966981 pymonit-1.3.21/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-16 15:19:33.000000 pymonit-1.3.21/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:28:05.015844 pymonit-1.4.0/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.4.0/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2188 2024-05-18 17:28:05.015844 pymonit-1.4.0/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1553 2024-05-18 17:12:03.000000 pymonit-1.4.0/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:28:05.012511 pymonit-1.4.0/monit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.4.0/monit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      977 2024-05-18 17:24:00.000000 pymonit-1.4.0/monit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      741 2024-05-18 17:23:53.000000 pymonit-1.4.0/monit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2013 2024-05-18 17:24:26.000000 pymonit-1.4.0/monit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1180 2024-05-18 17:24:34.000000 pymonit-1.4.0/monit/http.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      459 2024-05-18 17:24:45.000000 pymonit-1.4.0/monit/init.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      950 2024-05-18 17:25:03.000000 pymonit-1.4.0/monit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1698 2024-05-18 17:25:39.000000 pymonit-1.4.0/monit/logger.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-18 17:28:05.015844 pymonit-1.4.0/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2188 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      304 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        6 2024-05-18 17:28:04.000000 pymonit-1.4.0/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-18 17:28:05.015844 pymonit-1.4.0/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      865 2024-05-18 17:27:57.000000 pymonit-1.4.0/setup.py
```

### Comparing `pymonit-1.3.21/LICENSE` & `pymonit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.21/PKG-INFO` & `pymonit-1.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.21
+Version: 1.4.0
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -45,20 +45,19 @@
 # Email info
 # Deixe em branco para desativar o envio de e-mails
 EMAIL=
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
-**Utilização do Monit para notificação de erros**
+**Utilização simples**
 ```python
 import time
 
 from monit.core import Monitor as monit
-from monit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
@@ -67,41 +66,48 @@
         monit.notify_and_exit(e)
 
 
 if __name__ == "__main__":
     main()
 ```
 
-**Utilização do Monit para notificação de erros que
-não são grandes o suficientes para exigir que o
-processo seja interrompido.**
+**Utilização avançada**
 
 ```Python
 import time
 
 from monit.core import Monitor as monit
-from monit.error import SetupError
-# from monit.logger import Logger
-# from monit.log2file import Log2File
+from monit.logger import Logger
+from monit.log2file import Log2File
 
 def main():
-    # Initialize the Monitor
-    monit = Monitor()
 
-    # Log2File()
-    # log = Logger()
+    Log2File() # Salva todo o log em um arquivo
+    log = Logger()
 
     try:
-        # Your code that might raise exceptions
+        log.info("Hello, World!")
         time.sleep(5)
+
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        print("Erro: Ocorreu um erro inesperado.")
         monit.notify(e)
 
+    try:
+        time.sleep(2)
+        raise ValueError("This is another a sample error.")
+
+    except Exception as e:
+        monit.notify(e, "Custom message")
+
+    num = 0
+    for _ in range(3):
+        num += 1
+    monit.msg(f"Total count in for loop: {num}")
+
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.3.21/README.md` & `pymonit-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 # Email info
 # Deixe em branco para desativar o envio de e-mails
 EMAIL=
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
-**Utilização do Monit para notificação de erros**
+**Utilização simples**
 ```python
 import time
 
 from monit.core import Monitor as monit
-from monit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
@@ -48,41 +47,48 @@
         monit.notify_and_exit(e)
 
 
 if __name__ == "__main__":
     main()
 ```
 
-**Utilização do Monit para notificação de erros que
-não são grandes o suficientes para exigir que o
-processo seja interrompido.**
+**Utilização avançada**
 
 ```Python
 import time
 
 from monit.core import Monitor as monit
-from monit.error import SetupError
-# from monit.logger import Logger
-# from monit.log2file import Log2File
+from monit.logger import Logger
+from monit.log2file import Log2File
 
 def main():
-    # Initialize the Monitor
-    monit = Monitor()
 
-    # Log2File()
-    # log = Logger()
+    Log2File() # Salva todo o log em um arquivo
+    log = Logger()
 
     try:
-        # Your code that might raise exceptions
+        log.info("Hello, World!")
         time.sleep(5)
+
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        print("Erro: Ocorreu um erro inesperado.")
         monit.notify(e)
 
+    try:
+        time.sleep(2)
+        raise ValueError("This is another a sample error.")
+
+    except Exception as e:
+        monit.notify(e, "Custom message")
+
+    num = 0
+    for _ in range(3):
+        num += 1
+    monit.msg(f"Total count in for loop: {num}")
+
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.3.21/monit/config.py` & `pymonit-1.4.0/monit/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from dotenv import load_dotenv
 import os
-import json
 import inspect
 
+from monit.init import create_template
+
 calling_script_dir = os.path.dirname(os.path.abspath(inspect.stack()[1].filename))
 env_path = os.path.join(calling_script_dir, '.monit')
 load_dotenv(dotenv_path=env_path)
 
-# Code info
+if not os.path.isfile(env_path):
+    create_template()
+    raise Exception("Arquivo de configuraçao '.monit' não existe")
+
 project = os.getenv('PROJECT')
 company = os.getenv('COMPANY')
 dev = os.getenv('DEV')
-
-# Database info
-user = os.getenv('DB_USER')
-password = os.getenv('DB_PASSWORD')
-host = os.getenv('DB_HOST')
-database = os.getenv('DB_DATABASE')
-
-db_url = f'mysql+pymysql://{user}:{password}@{host}/{database}'
-
-# Email info
-email = os.getenv('EMAIL')
-email_password = os.getenv('EMAIL_PASSWORD')
-
-if not project or not company or not dev:
-    raise Exception("Por favor, as informações do código não podem ficar em branco.")
-
-if not user or not password or not host or not database:
-    raise Exception("Por favor, as informações do banco de dados não podem ficar em branco.")
+location = os.getenv('LOCATION')
+handler_url = os.getenv('HANDLER_URL')
+phone = os.getenv('PHONE')
+
+if not project or not company or not dev or not location or not handler_url:
+    empty_vars = [name for name, value in [("project", project), ("company", company), ("dev", dev), ("location", location), ("handler_url", handler_url)] if not value]
+    error_msg = f"Informações do código não foram preenchidas no arquivo de configuração: {', '.join(empty_vars)}"
+    raise Exception(error_msg)
```

### Comparing `pymonit-1.3.21/pymonit.egg-info/PKG-INFO` & `pymonit-1.4.0/pymonit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.21
+Version: 1.4.0
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -45,20 +45,19 @@
 # Email info
 # Deixe em branco para desativar o envio de e-mails
 EMAIL=
 EMAIL_PASSWORD=
 ```
 ### Exemplo de Uso:
 
-**Utilização do Monit para notificação de erros**
+**Utilização simples**
 ```python
 import time
 
 from monit.core import Monitor as monit
-from monit.error import SetupError
 
 def main():
 
     try:
         time.sleep(5)
         raise ValueError("This is a sample error.")
 
@@ -67,41 +66,48 @@
         monit.notify_and_exit(e)
 
 
 if __name__ == "__main__":
     main()
 ```
 
-**Utilização do Monit para notificação de erros que
-não são grandes o suficientes para exigir que o
-processo seja interrompido.**
+**Utilização avançada**
 
 ```Python
 import time
 
 from monit.core import Monitor as monit
-from monit.error import SetupError
-# from monit.logger import Logger
-# from monit.log2file import Log2File
+from monit.logger import Logger
+from monit.log2file import Log2File
 
 def main():
-    # Initialize the Monitor
-    monit = Monitor()
 
-    # Log2File()
-    # log = Logger()
+    Log2File() # Salva todo o log em um arquivo
+    log = Logger()
 
     try:
-        # Your code that might raise exceptions
+        log.info("Hello, World!")
         time.sleep(5)
+
         raise ValueError("This is a sample error.")
 
     except Exception as e:
-        print("Erro: Ocorreu um erro inesperado.")
         monit.notify(e)
 
+    try:
+        time.sleep(2)
+        raise ValueError("This is another a sample error.")
+
+    except Exception as e:
+        monit.notify(e, "Custom message")
+
+    num = 0
+    for _ in range(3):
+        num += 1
+    monit.msg(f"Total count in for loop: {num}")
+
     monit.end()
 
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `pymonit-1.3.21/setup.py` & `pymonit-1.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.21',
+    version='1.4.0',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```


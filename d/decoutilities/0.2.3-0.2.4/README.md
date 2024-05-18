# Comparing `tmp/decoutilities-0.2.3.tar.gz` & `tmp/decoutilities-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.3.tar", last modified: Wed May  8 08:04:29 2024, max compression
+gzip compressed data, was "decoutilities-0.2.4.tar", last modified: Sat May 18 20:26:37 2024, max compression
```

## Comparing `decoutilities-0.2.3.tar` & `decoutilities-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.928145 decoutilities-0.2.3/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    12036 2024-05-08 08:04:29.915233 decoutilities-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    11565 2024-05-08 08:01:40.000000 decoutilities-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.473198 decoutilities-0.2.3/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.3/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.710605 decoutilities-0.2.3/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.3/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.3/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.3/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.809938 decoutilities-0.2.3/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.3/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.3/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.3/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.839738 decoutilities-0.2.3/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.3/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.2.3/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.887419 decoutilities-0.2.3/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.3/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 08:04:29.901330 decoutilities-0.2.3/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    12036 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 08:04:29.000000 decoutilities-0.2.3/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 08:04:29.928145 decoutilities-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-08 08:03:28.000000 decoutilities-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.645125 decoutilities-0.2.4/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0    12193 2024-05-18 20:26:37.643042 decoutilities-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11722 2024-05-18 20:24:49.000000 decoutilities-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.624572 decoutilities-0.2.4/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.632977 decoutilities-0.2.4/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.636711 decoutilities-0.2.4/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.638817 decoutilities-0.2.4/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.2.4/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.639876 decoutilities-0.2.4/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.2.4/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:26:37.641983 decoutilities-0.2.4/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    12193 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-18 20:26:37.000000 decoutilities-0.2.4/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 20:26:37.645125 decoutilities-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-18 20:20:07.000000 decoutilities-0.2.4/setup.py
```

### Comparing `decoutilities-0.2.3/LICENSE` & `decoutilities-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/PKG-INFO` & `decoutilities-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.3
+Version: 0.2.4
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -279,14 +279,15 @@
 # Access the registered setting
 api_key = config_container.getValue("api_key")
 ```
 
 ### Inject System
 
 `decoutilities` comes with an easy to use injector class (EXPERIMENTAL) that allows to easily share information.
+Note: The recently added `registerClass` method allows to register classes instead of single functions, recommended combination with `singleton` decorator.
 
 ```python
 from decoutilities.inject import injector
 
 # Create an instance of the injector
 injector_instance = injector()
```

### Comparing `decoutilities-0.2.3/README.md` & `decoutilities-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,15 @@
 # Access the registered setting
 api_key = config_container.getValue("api_key")
 ```
 
 ### Inject System
 
 `decoutilities` comes with an easy to use injector class (EXPERIMENTAL) that allows to easily share information.
+Note: The recently added `registerClass` method allows to register classes instead of single functions, recommended combination with `singleton` decorator.
 
 ```python
 from decoutilities.inject import injector
 
 # Create an instance of the injector
 injector_instance = injector()
```

### Comparing `decoutilities-0.2.3/decoutilities/__init__.py` & `decoutilities-0.2.4/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/decoutilities/config/config.py` & `decoutilities-0.2.4/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/decoutilities/config/configContainer.py` & `decoutilities-0.2.4/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/decoutilities/data/dataEncryptor.py` & `decoutilities-0.2.4/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/decoutilities/data/keyManager.py` & `decoutilities-0.2.4/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/decoutilities/queue/__init__.py` & `decoutilities-0.2.4/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.3/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.4/decoutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.3
+Version: 0.2.4
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -279,14 +279,15 @@
 # Access the registered setting
 api_key = config_container.getValue("api_key")
 ```
 
 ### Inject System
 
 `decoutilities` comes with an easy to use injector class (EXPERIMENTAL) that allows to easily share information.
+Note: The recently added `registerClass` method allows to register classes instead of single functions, recommended combination with `singleton` decorator.
 
 ```python
 from decoutilities.inject import injector
 
 # Create an instance of the injector
 injector_instance = injector()
```

### Comparing `decoutilities-0.2.3/setup.py` & `decoutilities-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.3',
+version='0.2.4',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```


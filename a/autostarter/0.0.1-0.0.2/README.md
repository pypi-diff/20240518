# Comparing `tmp/autostarter-0.0.1.tar.gz` & `tmp/autostarter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autostarter-0.0.1.tar", last modified: Sun Jan  8 02:49:33 2023, max compression
+gzip compressed data, was "autostarter-0.0.2.tar", last modified: Sat May 18 07:35:47 2024, max compression
```

## Comparing `autostarter-0.0.1.tar` & `autostarter-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-01-08 02:49:33.894578 autostarter-0.0.1/
--rw-r--r--   0 sam        (501) staff       (20)     1060 2023-01-08 02:06:22.000000 autostarter-0.0.1/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)     2602 2023-01-08 02:49:33.894439 autostarter-0.0.1/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     2137 2023-01-08 02:49:08.000000 autostarter-0.0.1/README.md
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-01-08 02:49:33.893498 autostarter-0.0.1/autostarter/
--rw-r--r--   0 sam        (501) staff       (20)       37 2023-01-08 02:47:26.000000 autostarter-0.0.1/autostarter/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     1966 2023-01-08 02:47:54.000000 autostarter-0.0.1/autostarter/autostarter.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2023-01-08 02:49:33.894222 autostarter-0.0.1/autostarter.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)     2602 2023-01-08 02:49:33.000000 autostarter-0.0.1/autostarter.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      217 2023-01-08 02:49:33.000000 autostarter-0.0.1/autostarter.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2023-01-08 02:49:33.000000 autostarter-0.0.1/autostarter.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)       12 2023-01-08 02:49:33.000000 autostarter-0.0.1/autostarter.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)       38 2023-01-08 02:49:33.894631 autostarter-0.0.1/setup.cfg
--rw-r--r--   0 sam        (501) staff       (20)      673 2023-01-08 02:46:38.000000 autostarter-0.0.1/setup.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-18 07:35:47.058226 autostarter-0.0.2/
+-rw-r--r--   0 sam        (501) staff       (20)     1060 2024-05-18 07:31:46.000000 autostarter-0.0.2/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)     2604 2024-05-18 07:35:47.057979 autostarter-0.0.2/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     2137 2024-05-18 07:31:46.000000 autostarter-0.0.2/README.md
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-18 07:35:47.056089 autostarter-0.0.2/autostarter/
+-rw-r--r--   0 sam        (501) staff       (20)       81 2024-05-18 07:31:46.000000 autostarter-0.0.2/autostarter/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     1970 2024-05-18 07:32:54.000000 autostarter-0.0.2/autostarter/autostarter.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-18 07:35:47.057523 autostarter-0.0.2/autostarter/systems/
+-rw-r--r--   0 sam        (501) staff       (20)       36 2024-05-18 07:31:46.000000 autostarter-0.0.2/autostarter/systems/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     2822 2024-05-18 07:31:46.000000 autostarter-0.0.2/autostarter/systems/darwin.py
+-rw-r--r--   0 sam        (501) staff       (20)     2510 2024-05-18 07:31:46.000000 autostarter-0.0.2/autostarter/systems/linux.py
+-rw-r--r--   0 sam        (501) staff       (20)     2246 2024-05-18 07:31:46.000000 autostarter-0.0.2/autostarter/systems/windows.py
+-rw-r--r--   0 sam        (501) staff       (20)      651 2024-05-18 07:32:51.000000 autostarter-0.0.2/autostarter/util.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-05-18 07:35:47.057729 autostarter-0.0.2/autostarter.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)     2604 2024-05-18 07:35:47.000000 autostarter-0.0.2/autostarter.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)      359 2024-05-18 07:35:47.000000 autostarter-0.0.2/autostarter.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-05-18 07:35:47.000000 autostarter-0.0.2/autostarter.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)       12 2024-05-18 07:35:47.000000 autostarter-0.0.2/autostarter.egg-info/top_level.txt
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-05-18 07:35:47.058277 autostarter-0.0.2/setup.cfg
+-rw-r--r--   0 sam        (501) staff       (20)      675 2024-05-18 07:32:46.000000 autostarter-0.0.2/setup.py
```

### Comparing `autostarter-0.0.1/LICENSE` & `autostarter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autostarter-0.0.1/PKG-INFO` & `autostarter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autostarter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module for adding and removing startup scripts on Windows, Mac, and Linux systems
-Home-page: https://github.com/ctrlsam/autostart
+Home-page: https://github.com/ctrlsam/autostarter
 Author: Sam Redmond
 Author-email: samredmondtech@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `autostarter-0.0.1/README.md` & `autostarter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autostarter-0.0.1/autostarter/autostarter.py` & `autostarter-0.0.2/autostarter/autostarter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import uuid
 
 @functools.lru_cache()
 def _get_os_module():
     """
     Returns the OS-specific module for the current operating system.
     """
-    return importlib.import_module('startup.systems.' + platform.system().lower())
+    return importlib.import_module('autostarter.systems.' + platform.system().lower())
 
 def add(script_location, **kwargs):
     """
     Adds a startup script with the specified parameters.
 
     Parameters:
     - script_location (str): The location of the script to be added as a startup script.
```

### Comparing `autostarter-0.0.1/autostarter.egg-info/PKG-INFO` & `autostarter-0.0.2/autostarter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autostarter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A module for adding and removing startup scripts on Windows, Mac, and Linux systems
-Home-page: https://github.com/ctrlsam/autostart
+Home-page: https://github.com/ctrlsam/autostarter
 Author: Sam Redmond
 Author-email: samredmondtech@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `autostarter-0.0.1/setup.py` & `autostarter-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autostarter",
-    version="0.0.1",
+    version="0.0.2",
     author="Sam Redmond",
     author_email="samredmondtech@gmail.com",
     description="A module for adding and removing startup scripts on Windows, Mac, and Linux systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ctrlsam/autostart",
+    url="https://github.com/ctrlsam/autostarter",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```


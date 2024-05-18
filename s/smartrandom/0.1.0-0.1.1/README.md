# Comparing `tmp/smartrandom-0.1.0.tar.gz` & `tmp/smartrandom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartrandom-0.1.0.tar", last modified: Wed May 15 05:04:00 2024, max compression
+gzip compressed data, was "smartrandom-0.1.1.tar", last modified: Sat May 18 07:30:58 2024, max compression
```

## Comparing `smartrandom-0.1.0.tar` & `smartrandom-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:04:00.729252 smartrandom-0.1.0/
--rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-08 03:52:29.000000 smartrandom-0.1.0/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)     3683 2024-05-15 05:04:00.729252 smartrandom-0.1.0/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     2679 2024-05-15 04:50:25.000000 smartrandom-0.1.0/README.md
--rw-r--r--   0 smart     (1000) smart     (1000)     1191 2024-05-15 05:04:00.729252 smartrandom-0.1.0/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      442 2024-05-15 05:03:25.000000 smartrandom-0.1.0/setup.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:04:00.725918 smartrandom-0.1.0/smartrandom/
--rw-r--r--   0 smart     (1000) smart     (1000)      621 2024-05-15 04:46:27.000000 smartrandom-0.1.0/smartrandom/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)     2503 2024-05-15 04:58:19.000000 smartrandom-0.1.0/smartrandom/random_master.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-15 05:04:00.729252 smartrandom-0.1.0/smartrandom.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     3683 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      263 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-15 05:04:00.000000 smartrandom-0.1.0/smartrandom.egg-info/top_level.txt
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:30:58.958706 smartrandom-0.1.1/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1498 2024-05-18 07:14:25.000000 smartrandom-0.1.1/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      123 2024-05-18 07:29:54.000000 smartrandom-0.1.1/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     3706 2024-05-18 07:30:58.958706 smartrandom-0.1.1/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     2679 2024-05-18 07:20:58.000000 smartrandom-0.1.1/README.md
+-rw-r--r--   0 smart     (1000) smart     (1000)        0 2024-05-18 07:28:29.000000 smartrandom-0.1.1/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1215 2024-05-18 07:30:58.958706 smartrandom-0.1.1/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      442 2024-05-18 07:14:25.000000 smartrandom-0.1.1/setup.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:30:58.955373 smartrandom-0.1.1/smartrandom/
+-rw-r--r--   0 smart     (1000) smart     (1000)      621 2024-05-18 07:20:58.000000 smartrandom-0.1.1/smartrandom/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     2746 2024-05-18 07:17:00.000000 smartrandom-0.1.1/smartrandom/random_master.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-18 07:30:58.958706 smartrandom-0.1.1/smartrandom.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     3706 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      292 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       12 2024-05-18 07:30:58.000000 smartrandom-0.1.1/smartrandom.egg-info/top_level.txt
```

### Comparing `smartrandom-0.1.0/LICENSE` & `smartrandom-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartrandom-0.1.0/PKG-INFO` & `smartrandom-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.1.0
+Version: 0.1.1
 Summary: Random Data Generators.
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
-Keywords: password generator,code generator,random generator,random code generator,random string generator,smartrandom,smartlegionlab
+Keywords: password generator,code generator,random generator,random code generator,random string generator,random bytes generator,smartrandom,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.1.0</sup>
+# smartrandom <sup>v0.1.1</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, and symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
```

### Comparing `smartrandom-0.1.0/README.md` & `smartrandom-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# smartrandom <sup>v0.1.0</sup>
+# smartrandom <sup>v0.1.1</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, and symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
```

### Comparing `smartrandom-0.1.0/setup.cfg` & `smartrandom-0.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 keywords = 
 	password generator
 	code generator
 	random generator
 	random code generator
 	random string generator
+	random bytes generator
 	smartrandom
 	smartlegionlab
 
 [options]
 package_dir = 
 packages = find:
 python_requires = >= 3.6
```

### Comparing `smartrandom-0.1.0/smartrandom/__init__.py` & `smartrandom-0.1.1/smartrandom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # https://github.com/smartlegionlab
 # --------------------------------------------------------
 """Smart Random - Random Data Generators.
 
 Allows you to generate random strings of a given length from letters, numbers, and symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
 """
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

### Comparing `smartrandom-0.1.0/smartrandom/random_master.py` & `smartrandom-0.1.1/smartrandom/random_master.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Copyright © 2018-2024, A.A Suvorov
 # All rights reserved.
 # --------------------------------------------------------
 # https://github.com/smartlegionlab
 # --------------------------------------------------------
 """Random Data Generators."""
 import hashlib
+import os
 import random
 import string
 
 
 class RandomLettersMaster:
     letters = string.ascii_letters
 
@@ -41,19 +42,26 @@
     def create(cls, text: str):
         text = str(text)
         sha = hashlib.sha3_512(text.encode('utf-8'))
         new_hash = sha.hexdigest()
         return new_hash
 
 
+class UrandomGen:
+    @classmethod
+    def generate(cls, size=32):
+        return os.urandom(size)
+
+
 class RandomStringMaster:
     letters_master = RandomLettersMaster()
     numeric_master = RandomNumericMaster()
     symbols_master = RandomSymbolsMaster()
     hash_master = HashMaster()
+    urandom_gen = UrandomGen()
 
     @classmethod
     def create_string(cls, length=10):
         random_string = cls.letters_master.letters + cls.numeric_master.numbers + cls.symbols_master.symbols
         return ''.join((random.choice(random_string) for _ in range(length)))
 
     @classmethod
@@ -80,7 +88,11 @@
         if numeric_flag:
             data += cls.numeric_master.numbers
         if symbols_flag:
             data += cls.symbols_master.symbols
         if data:
             return ''.join((random.choice(data) for _ in range(length)))
         return None
+
+    @classmethod
+    def get_random_bytes(cls, size):
+        return cls.urandom_gen.generate(size)
```

### Comparing `smartrandom-0.1.0/smartrandom.egg-info/PKG-INFO` & `smartrandom-0.1.1/smartrandom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: smartrandom
-Version: 0.1.0
+Version: 0.1.1
 Summary: Random Data Generators.
 Home-page: https://github.com/smartlegionlab/smartrandom/
 Author: A.A Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/smartrandom/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/smartrandom/releases
-Keywords: password generator,code generator,random generator,random code generator,random string generator,smartrandom,smartlegionlab
+Keywords: password generator,code generator,random generator,random code generator,random string generator,random bytes generator,smartrandom,smartlegionlab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# smartrandom <sup>v0.1.0</sup>
+# smartrandom <sup>v0.1.1</sup>
 ---
 
 ## Random Data Generators:
 
 Allows you to generate random strings of a given length from letters, numbers, and symbols.
 Helps to generate passwords, service codes (for example, for sending via SMS), hashes, and much more.
```


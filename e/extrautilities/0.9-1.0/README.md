# Comparing `tmp/extrautilities-0.9.tar.gz` & `tmp/extrautilities-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-0.9.tar", last modified: Thu May 16 15:53:41 2024, max compression
+gzip compressed data, was "extrautilities-1.0.tar", last modified: Sat May 18 11:20:09 2024, max compression
```

## Comparing `extrautilities-0.9.tar` & `extrautilities-1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:53:41.193700 extrautilities-0.9/
-drwxrwxrwx   0        0        0        0 2024-05-16 15:53:41.179380 extrautilities-0.9/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-0.9/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-0.9/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-0.9/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     4317 2024-05-16 15:52:59.000000 extrautilities-0.9/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     3307 2024-05-16 15:53:41.193700 extrautilities-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 15:53:41.193199 extrautilities-0.9/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3307 2024-05-16 15:53:41.000000 extrautilities-0.9/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-16 15:53:41.000000 extrautilities-0.9/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:53:41.000000 extrautilities-0.9/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:53:41.000000 extrautilities-0.9/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 15:53:41.000000 extrautilities-0.9/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:53:41.193700 extrautilities-0.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-16 15:53:40.000000 extrautilities-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 11:20:09.617848 extrautilities-1.0/
+drwxrwxrwx   0        0        0        0 2024-05-18 11:20:09.598828 extrautilities-1.0/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.0/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.0/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-1.0/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.0/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     4453 2024-05-16 16:25:09.000000 extrautilities-1.0/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     3322 2024-05-18 11:20:09.617348 extrautilities-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 11:20:09.616844 extrautilities-1.0/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3322 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 11:20:09.617848 extrautilities-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2024-05-18 11:20:01.000000 extrautilities-1.0/setup.py
```

### Comparing `extrautilities-0.9/ExtraUtils/RateLimit.py` & `extrautilities-1.0/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.9/ExtraUtils/asyncTokens.py` & `extrautilities-1.0/ExtraUtils/asyncTokens.py`

 * *Files identical despite different names*

### Comparing `extrautilities-0.9/ExtraUtils/timeBasedToken.py` & `extrautilities-1.0/ExtraUtils/timeBasedToken.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
         # Kombiniere Token und Zeitstempel und erstelle einen SHA-256 Hash
         combined = f"{self.__special}{timestamp}".encode()
         hash_result = hashlib.sha256(combined).hexdigest()
 
         # Erstelle eine Bitmap aus den ersten 8 Zeichen des Hashes
         bitmap = bin(int(hash_result[:8], 16))[2:].zfill(32)
-        print(bitmap)
+
 
         # Erstelle eine "zufällige" Reihenfolge aus den nächsten 8 Zeichen
         order_seed = int(hash_result[8:16], 16)
         order = sorted(range(32), key=lambda x: (order_seed >> (x % 8)) & 1)
-        print(order)
+
 
         # Extrahiere und sortiere Zeichen basierend auf der Bitmap und der Reihenfolge
         extracted_chars = ''.join([self.__special[i] for i, bit in enumerate(bitmap) if bit == '1'])
         sorted_chars = ''.join([extracted_chars[i] for i in order if i < len(extracted_chars)])
 
         # Kombiniere den self.__primary mit den sortierten Zeichen und erstelle einen finalen Hash
         final_combined = f"{self.__primary}{sorted_chars}".encode()
@@ -71,20 +71,23 @@
         encrypted_bytes = cipher.encrypt(pad(plaintext.encode(), AES.block_size))
         
         # Kombiniere IV und verschlüsselten Text, kodiere beides in Base64 für einfache Handhabung
         encrypted_data = base64.b64encode(self.__iv + encrypted_bytes).decode()
         
         return encrypted_data
 
-    def decrypt(self, encrypted_data):
+    def decrypt(self, encrypted):
         # Konvertiere den Hex-Schlüssel in Bytes
         key_bytes = bytes.fromhex(self.__enckey)
-        
+        if not encrypted:
+            raise ValueError("Encrypted data can't be empty")
+        if not isinstance(encrypted, str):
+            raise ValueError("Encrypted data must be string")
         # Dekodiere die Daten aus Base64
-        encrypted_bytes = base64.b64decode(encrypted_data)
+        encrypted_bytes = base64.b64decode(encrypted)
         
 
         encrypted_text = encrypted_bytes[AES.block_size:]
         
         # Initialisiere den AES Cipher im CBC Modus
         cipher = AES.new(key_bytes, AES.MODE_CBC, self.__iv)
```

### Comparing `extrautilities-0.9/PKG-INFO` & `extrautilities-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.9
+Version: 1.0
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit,timeBasedToken
+Keywords: RateLimit,timeBasedToken,getFileContent
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `extrautilities-0.9/README.md` & `extrautilities-1.0/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-0.9/extrautilities.egg-info/PKG-INFO` & `extrautilities-1.0/extrautilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 0.9
+Version: 1.0
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit,timeBasedToken
+Keywords: RateLimit,timeBasedToken,getFileContent
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `extrautilities-0.9/setup.py` & `extrautilities-1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='0.9',
+    version='1.0',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    keywords='RateLimit, timeBasedToken',
+    keywords='RateLimit, timeBasedToken, getFileContent',
     install_requires=["extradecorators", "cryptography","pycryptodome"],
 )
```


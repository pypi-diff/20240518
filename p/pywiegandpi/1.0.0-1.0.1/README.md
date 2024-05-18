# Comparing `tmp/pywiegandpi-1.0.0.tar.gz` & `tmp/pywiegandpi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywiegandpi-1.0.0.tar", last modified: Thu May 16 16:53:06 2024, max compression
+gzip compressed data, was "pywiegandpi-1.0.1.tar", last modified: Sat May 18 03:22:48 2024, max compression
```

## Comparing `pywiegandpi-1.0.0.tar` & `pywiegandpi-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:53:06.985206 pywiegandpi-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 16:53:03.000000 pywiegandpi-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 16:53:06.985206 pywiegandpi-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 16:53:03.000000 pywiegandpi-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-16 16:53:03.000000 pywiegandpi-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:53:06.985206 pywiegandpi-1.0.0/pywiegandpi/
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-16 16:53:03.000000 pywiegandpi-1.0.0/pywiegandpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:53:06.985206 pywiegandpi-1.0.0/pywiegandpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 16:53:06.000000 pywiegandpi-1.0.0/pywiegandpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 16:53:06.000000 pywiegandpi-1.0.0/pywiegandpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:53:06.000000 pywiegandpi-1.0.0/pywiegandpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 16:53:06.000000 pywiegandpi-1.0.0/pywiegandpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 16:53:06.000000 pywiegandpi-1.0.0/pywiegandpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:53:06.985206 pywiegandpi-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:22:48.786387 pywiegandpi-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-18 03:22:45.000000 pywiegandpi-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-18 03:22:48.786387 pywiegandpi-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-18 03:22:45.000000 pywiegandpi-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-18 03:22:45.000000 pywiegandpi-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:22:48.786387 pywiegandpi-1.0.1/pywiegandpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-18 03:22:45.000000 pywiegandpi-1.0.1/pywiegandpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 03:22:48.786387 pywiegandpi-1.0.1/pywiegandpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-18 03:22:48.000000 pywiegandpi-1.0.1/pywiegandpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-18 03:22:48.000000 pywiegandpi-1.0.1/pywiegandpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 03:22:48.000000 pywiegandpi-1.0.1/pywiegandpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 03:22:48.000000 pywiegandpi-1.0.1/pywiegandpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 03:22:48.000000 pywiegandpi-1.0.1/pywiegandpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 03:22:48.786387 pywiegandpi-1.0.1/setup.cfg
```

### Comparing `pywiegandpi-1.0.0/LICENSE` & `pywiegandpi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywiegandpi-1.0.0/PKG-INFO` & `pywiegandpi-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywiegandpi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatically decode Wiegand data from Raspberry Pi GPIO pins.
 Author-email: Jaimyn Mayer <hello@jaimyn.dev>
 Project-URL: Homepage, https://github.com/membermatters/pywiegandpi
 Project-URL: Issues, https://github.com/membermatters/pywiegandpi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywiegandpi-1.0.0/README.md` & `pywiegandpi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pywiegandpi-1.0.0/pyproject.toml` & `pywiegandpi-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywiegandpi"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
     "pigpio >= 1.78",
 ]
 authors = [
   { name="Jaimyn Mayer", email="hello@jaimyn.dev" },
 ]
 description = "Automatically decode Wiegand data from Raspberry Pi GPIO pins."
```

### Comparing `pywiegandpi-1.0.0/pywiegandpi/__init__.py` & `pywiegandpi-1.0.1/pywiegandpi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                     if self.raw_mode:
                         self.callback(self.bits, self.num)
                     else:
                         # get only the bits we're interested in
                         card_mask_26bit = 0b0_00000000_11111111_11111111_11111111_0
                         card_mask_34bit = 0b0_11111111_11111111_11111111_11111111_0
                         card_mask = card_mask_34bit if self.wiegand_32bit_mode else card_mask_26bit
-                        card_uid = self.num & card_mask >> 1  # strip off the remaining parity bit
+                        card_uid = (self.num & card_mask) >> 1  # strip off the remaining parity bit
                         self.callback(self.bits, card_uid)
 
     def cancel(self):
         """
         Cancel the Wiegand decoder.
         """
```

### Comparing `pywiegandpi-1.0.0/pywiegandpi.egg-info/PKG-INFO` & `pywiegandpi-1.0.1/pywiegandpi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywiegandpi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatically decode Wiegand data from Raspberry Pi GPIO pins.
 Author-email: Jaimyn Mayer <hello@jaimyn.dev>
 Project-URL: Homepage, https://github.com/membermatters/pywiegandpi
 Project-URL: Issues, https://github.com/membermatters/pywiegandpi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```


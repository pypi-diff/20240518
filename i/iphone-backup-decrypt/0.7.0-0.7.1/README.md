# Comparing `tmp/iphone_backup_decrypt-0.7.0.tar.gz` & `tmp/iphone_backup_decrypt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iphone_backup_decrypt-0.7.0.tar", last modified: Thu May  9 19:21:21 2024, max compression
+gzip compressed data, was "iphone_backup_decrypt-0.7.1.tar", last modified: Sat May 18 21:36:23 2024, max compression
```

## Comparing `iphone_backup_decrypt-0.7.0.tar` & `iphone_backup_decrypt-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.355233 iphone_backup_decrypt-0.7.0/
--rw-rw-rw-   0        0        0     2777 2019-11-13 20:01:32.000000 iphone_backup_decrypt-0.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5307 2024-05-09 19:21:21.353279 iphone_backup_decrypt-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4671 2024-05-09 19:07:00.000000 iphone_backup_decrypt-0.7.0/README.md
--rw-rw-rw-   0        0        0      745 2024-05-09 19:11:00.000000 iphone_backup_decrypt-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 19:21:21.355233 iphone_backup_decrypt-0.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.285915 iphone_backup_decrypt-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.316181 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/
--rw-rw-rw-   0        0        0      218 2024-05-09 19:06:29.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/__init__.py
--rw-rw-rw-   0        0        0     4911 2024-05-06 13:05:23.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/google_iphone_dataprotection.py
--rw-rw-rw-   0        0        0    20354 2024-05-09 19:19:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/iphone_backup.py
--rw-rw-rw-   0        0        0     6470 2024-05-09 19:06:29.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:21:21.351326 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/
--rw-rw-rw-   0        0        0     5307 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-09 19:21:21.000000 iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-18 21:36:23.471846 iphone_backup_decrypt-0.7.1/
+-rw-rw-rw-   0        0        0     2777 2019-11-13 20:01:32.000000 iphone_backup_decrypt-0.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5307 2024-05-18 21:36:23.470869 iphone_backup_decrypt-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4671 2024-05-09 19:07:00.000000 iphone_backup_decrypt-0.7.1/README.md
+-rw-rw-rw-   0        0        0      745 2024-05-18 21:33:44.000000 iphone_backup_decrypt-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-18 21:36:23.472821 iphone_backup_decrypt-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 21:36:23.390715 iphone_backup_decrypt-0.7.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-18 21:36:23.433770 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/
+-rw-rw-rw-   0        0        0      218 2024-05-09 19:06:29.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/__init__.py
+-rw-rw-rw-   0        0        0     4911 2024-05-06 13:05:23.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/google_iphone_dataprotection.py
+-rw-rw-rw-   0        0        0    20354 2024-05-09 19:19:21.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/iphone_backup.py
+-rw-rw-rw-   0        0        0     6474 2024-05-18 21:31:34.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-18 21:36:23.468916 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/
+-rw-rw-rw-   0        0        0     5307 2024-05-18 21:36:23.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-05-18 21:36:23.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 21:36:23.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-18 21:36:23.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-18 21:36:23.000000 iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/top_level.txt
```

### Comparing `iphone_backup_decrypt-0.7.0/LICENSE.txt` & `iphone_backup_decrypt-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iphone_backup_decrypt-0.7.0/PKG-INFO` & `iphone_backup_decrypt-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphone_backup_decrypt
-Version: 0.7.0
+Version: 0.7.1
 Summary: Decrypt and extract files from an iOS13+ encrypted local backup.
 Author: James Sharkey
 Project-URL: Homepage, https://github.com/jsharkey13/iphone_backup_decrypt
 Keywords: iPhone,backup,forensics,iOS,WhatsApp,decryption,iOS backup,iTunes Backup
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
```

### Comparing `iphone_backup_decrypt-0.7.0/README.md` & `iphone_backup_decrypt-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `iphone_backup_decrypt-0.7.0/pyproject.toml` & `iphone_backup_decrypt-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iphone_backup_decrypt"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="James Sharkey" },
 ]
 description = "Decrypt and extract files from an iOS13+ encrypted local backup."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/google_iphone_dataprotection.py` & `iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/google_iphone_dataprotection.py`

 * *Files identical despite different names*

### Comparing `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/iphone_backup.py` & `iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/iphone_backup.py`

 * *Files identical despite different names*

### Comparing `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt/utils.py` & `iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,14 @@
             n = int(dec_data[-1])  # RFC 1423, final byte contains number of padding bytes.
             if n > _CBC_BLOCK_SIZE or n > len(dec_data):
                 raise ValueError('AES decrypt: invalid CBC padding')
             dec_data = dec_data[:-n]
         dec_filehandle.write(dec_data)
     # Check output size:
     if dec_filehandle.tell() != file_plist.filesize:
-        print(f"WARN: decrypted {dec_filehandle.tell()} bytes of '{out_filepath}', expected {file_plist.size} bytes!")
+        print(f"WARN: decrypted {dec_filehandle.tell()} bytes of '{out_filepath}', expected {file_plist.filesize} bytes!")
     # Close filehandles:
     enc_filehandle.close()
     dec_filehandle.close()
     # Set the correct last_modified time on the output file, if possible:
     if file_plist.mtime:
         os.utime(out_filepath, times=(file_plist.mtime, file_plist.mtime))
```

### Comparing `iphone_backup_decrypt-0.7.0/src/iphone_backup_decrypt.egg-info/PKG-INFO` & `iphone_backup_decrypt-0.7.1/src/iphone_backup_decrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iphone_backup_decrypt
-Version: 0.7.0
+Version: 0.7.1
 Summary: Decrypt and extract files from an iOS13+ encrypted local backup.
 Author: James Sharkey
 Project-URL: Homepage, https://github.com/jsharkey13/iphone_backup_decrypt
 Keywords: iPhone,backup,forensics,iOS,WhatsApp,decryption,iOS backup,iTunes Backup
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
```


# Comparing `tmp/offlinesec_client-1.1.4.tar.gz` & `tmp/offlinesec_client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinesec_client-1.1.4.tar", last modified: Sat May 11 07:31:22 2024, max compression
+gzip compressed data, was "offlinesec_client-1.1.5.tar", last modified: Sat May 18 07:45:24 2024, max compression
```

## Comparing `offlinesec_client-1.1.4.tar` & `offlinesec_client-1.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 07:31:22.951358 offlinesec_client-1.1.4/
--rw-rw-rw-   0        0        0     6793 2024-05-11 07:31:22.950323 offlinesec_client-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6499 2024-05-03 06:54:42.000000 offlinesec_client-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 07:31:22.942903 offlinesec_client-1.1.4/offlinesec_client/
--rw-rw-rw-   0        0        0       23 2024-05-11 07:26:12.000000 offlinesec_client-1.1.4/offlinesec_client/__init__.py
--rw-rw-rw-   0        0        0      110 2023-07-14 20:07:51.000000 offlinesec_client-1.1.4/offlinesec_client/__main__.py
--rw-rw-rw-   0        0        0     4254 2024-05-11 07:25:47.000000 offlinesec_client-1.1.4/offlinesec_client/abap_system.py
--rw-rw-rw-   0        0        0     4080 2023-10-03 17:05:46.000000 offlinesec_client-1.1.4/offlinesec_client/agr_1251.py
--rw-rw-rw-   0        0        0     1853 2024-05-05 07:15:11.000000 offlinesec_client-1.1.4/offlinesec_client/api_sec_notes.py
--rw-rw-rw-   0        0        0     1255 2024-05-03 05:48:17.000000 offlinesec_client-1.1.4/offlinesec_client/bo_system.py
--rw-rw-rw-   0        0        0     2893 2023-09-14 14:17:57.000000 offlinesec_client-1.1.4/offlinesec_client/config.py
--rw-rw-rw-   0        0        0      577 2023-09-17 12:59:15.000000 offlinesec_client-1.1.4/offlinesec_client/const.py
--rw-rw-rw-   0        0        0     1594 2023-10-10 16:14:36.000000 offlinesec_client-1.1.4/offlinesec_client/cwbntcust.py
--rw-rw-rw-   0        0        0     4342 2023-12-03 15:32:46.000000 offlinesec_client-1.1.4/offlinesec_client/func.py
--rw-rw-rw-   0        0        0     3435 2023-08-21 06:40:25.000000 offlinesec_client-1.1.4/offlinesec_client/get_reports.py
--rw-rw-rw-   0        0        0     2235 2024-05-03 05:48:17.000000 offlinesec_client-1.1.4/offlinesec_client/java_system.py
--rw-rw-rw-   0        0        0     1847 2024-04-07 08:20:55.000000 offlinesec_client-1.1.4/offlinesec_client/multi_systems.py
--rw-rw-rw-   0        0        0     4118 2023-10-21 13:22:58.000000 offlinesec_client-1.1.4/offlinesec_client/req_bo_notes.py
--rw-rw-rw-   0        0        0     4642 2023-11-17 19:46:10.000000 offlinesec_client-1.1.4/offlinesec_client/req_java_notes.py
--rw-rw-rw-   0        0        0     4601 2023-10-14 08:09:41.000000 offlinesec_client-1.1.4/offlinesec_client/req_notes_report.py
--rw-rw-rw-   0        0        0     4652 2023-07-15 08:41:30.000000 offlinesec_client-1.1.4/offlinesec_client/req_param_report.py
--rw-rw-rw-   0        0        0     2095 2024-05-04 06:59:30.000000 offlinesec_client-1.1.4/offlinesec_client/req_patch_day.py
--rw-rw-rw-   0        0        0     4060 2023-10-03 20:26:25.000000 offlinesec_client-1.1.4/offlinesec_client/req_roles_report.py
--rw-rw-rw-   0        0        0     2054 2024-05-04 06:59:30.000000 offlinesec_client-1.1.4/offlinesec_client/req_sec_notes.py
--rw-rw-rw-   0        0        0     2502 2024-05-04 07:05:36.000000 offlinesec_client-1.1.4/offlinesec_client/resolve_report.py
--rw-rw-rw-   0        0        0     5092 2024-03-10 09:46:08.000000 offlinesec_client-1.1.4/offlinesec_client/rsparam.py
--rw-rw-rw-   0        0        0     5028 2023-09-19 06:24:24.000000 offlinesec_client-1.1.4/offlinesec_client/sap_gui.py
--rw-rw-rw-   0        0        0     2931 2023-11-19 10:07:16.000000 offlinesec_client-1.1.4/offlinesec_client/sap_system.py
-drwxrwxrwx   0        0        0        0 2024-05-11 07:31:22.949250 offlinesec_client-1.1.4/offlinesec_client.egg-info/
--rw-rw-rw-   0        0        0     6793 2024-05-11 07:31:22.000000 offlinesec_client-1.1.4/offlinesec_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2024-05-11 07:31:22.000000 offlinesec_client-1.1.4/offlinesec_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 07:31:22.000000 offlinesec_client-1.1.4/offlinesec_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      641 2024-05-11 07:31:22.000000 offlinesec_client-1.1.4/offlinesec_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2024-05-11 07:31:22.000000 offlinesec_client-1.1.4/offlinesec_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-11 07:31:22.000000 offlinesec_client-1.1.4/offlinesec_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 07:31:22.951358 offlinesec_client-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1725 2024-05-05 06:58:23.000000 offlinesec_client-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:45:24.696598 offlinesec_client-1.1.5/
+-rw-rw-rw-   0        0        0     6793 2024-05-18 07:45:24.695577 offlinesec_client-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6499 2024-05-03 06:54:42.000000 offlinesec_client-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 07:45:24.687308 offlinesec_client-1.1.5/offlinesec_client/
+-rw-rw-rw-   0        0        0       23 2024-05-18 06:31:04.000000 offlinesec_client-1.1.5/offlinesec_client/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-07-14 20:07:51.000000 offlinesec_client-1.1.5/offlinesec_client/__main__.py
+-rw-rw-rw-   0        0        0     4703 2024-05-18 06:58:57.000000 offlinesec_client-1.1.5/offlinesec_client/abap_system.py
+-rw-rw-rw-   0        0        0     4080 2023-10-03 17:05:46.000000 offlinesec_client-1.1.5/offlinesec_client/agr_1251.py
+-rw-rw-rw-   0        0        0     1853 2024-05-05 07:15:11.000000 offlinesec_client-1.1.5/offlinesec_client/api_sec_notes.py
+-rw-rw-rw-   0        0        0     1255 2024-05-03 05:48:17.000000 offlinesec_client-1.1.5/offlinesec_client/bo_system.py
+-rw-rw-rw-   0        0        0     2893 2023-09-14 14:17:57.000000 offlinesec_client-1.1.5/offlinesec_client/config.py
+-rw-rw-rw-   0        0        0      577 2023-09-17 12:59:15.000000 offlinesec_client-1.1.5/offlinesec_client/const.py
+-rw-rw-rw-   0        0        0     1594 2023-10-10 16:14:36.000000 offlinesec_client-1.1.5/offlinesec_client/cwbntcust.py
+-rw-rw-rw-   0        0        0     4376 2024-05-18 06:31:04.000000 offlinesec_client-1.1.5/offlinesec_client/func.py
+-rw-rw-rw-   0        0        0     3439 2024-05-18 07:42:02.000000 offlinesec_client-1.1.5/offlinesec_client/get_reports.py
+-rw-rw-rw-   0        0        0     2235 2024-05-03 05:48:17.000000 offlinesec_client-1.1.5/offlinesec_client/java_system.py
+-rw-rw-rw-   0        0        0     1847 2024-04-07 08:20:55.000000 offlinesec_client-1.1.5/offlinesec_client/multi_systems.py
+-rw-rw-rw-   0        0        0     4118 2023-10-21 13:22:58.000000 offlinesec_client-1.1.5/offlinesec_client/req_bo_notes.py
+-rw-rw-rw-   0        0        0     4642 2023-11-17 19:46:10.000000 offlinesec_client-1.1.5/offlinesec_client/req_java_notes.py
+-rw-rw-rw-   0        0        0     4582 2024-05-18 07:05:04.000000 offlinesec_client-1.1.5/offlinesec_client/req_notes_report.py
+-rw-rw-rw-   0        0        0     4652 2023-07-15 08:41:30.000000 offlinesec_client-1.1.5/offlinesec_client/req_param_report.py
+-rw-rw-rw-   0        0        0     2095 2024-05-04 06:59:30.000000 offlinesec_client-1.1.5/offlinesec_client/req_patch_day.py
+-rw-rw-rw-   0        0        0     4060 2023-10-03 20:26:25.000000 offlinesec_client-1.1.5/offlinesec_client/req_roles_report.py
+-rw-rw-rw-   0        0        0     2054 2024-05-04 06:59:30.000000 offlinesec_client-1.1.5/offlinesec_client/req_sec_notes.py
+-rw-rw-rw-   0        0        0     2502 2024-05-04 07:05:36.000000 offlinesec_client-1.1.5/offlinesec_client/resolve_report.py
+-rw-rw-rw-   0        0        0     5092 2024-03-10 09:46:08.000000 offlinesec_client-1.1.5/offlinesec_client/rsparam.py
+-rw-rw-rw-   0        0        0     5044 2024-05-18 06:31:04.000000 offlinesec_client-1.1.5/offlinesec_client/sap_gui.py
+-rw-rw-rw-   0        0        0     2931 2023-11-19 10:07:16.000000 offlinesec_client-1.1.5/offlinesec_client/sap_system.py
+drwxrwxrwx   0        0        0        0 2024-05-18 07:45:24.694544 offlinesec_client-1.1.5/offlinesec_client.egg-info/
+-rw-rw-rw-   0        0        0     6793 2024-05-18 07:45:24.000000 offlinesec_client-1.1.5/offlinesec_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2024-05-18 07:45:24.000000 offlinesec_client-1.1.5/offlinesec_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 07:45:24.000000 offlinesec_client-1.1.5/offlinesec_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      641 2024-05-18 07:45:24.000000 offlinesec_client-1.1.5/offlinesec_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2024-05-18 07:45:24.000000 offlinesec_client-1.1.5/offlinesec_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-18 07:45:24.000000 offlinesec_client-1.1.5/offlinesec_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 07:45:24.696598 offlinesec_client-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1725 2024-05-05 06:58:23.000000 offlinesec_client-1.1.5/setup.py
```

### Comparing `offlinesec_client-1.1.4/PKG-INFO` & `offlinesec_client-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinesec_client
-Version: 1.1.4
+Version: 1.1.5
 Summary: Offline Security Client
 Home-page: https://offlinesec.com
 Author: Offline Security
 Author-email: info@offlinesec.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `offlinesec_client-1.1.4/README.md` & `offlinesec_client-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/abap_system.py` & `offlinesec_client-1.1.5/offlinesec_client/abap_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 from offlinesec_client.sap_system import SAPSystem
 from offlinesec_client.cwbntcust import Cwbntcust
 import os
 import re
 
 ABAP = "ABAP"
+KRNL_VERSION = "krnl_version"
+KRNL_PATCH = "krnl_patch"
+ABAP_SOFTS = "softs"
+CWBNTCUST = "cwbntcust"
+EXCLUDE_NOTES = "exclude"
+ABAP_NAME = "name"
 
 
 class ABAPSystem (SAPSystem):
     def __init__(self, **args):
         super().__init__(args["name"])
         self.type = ABAP
         root_dir = args["root_dir"] if "root_dir" in args else None
 
-        self.kernel_version = ABAPSystem.check_kernel_version(args["krnl_version"]) if "krnl_version" in args.keys() \
-            else ""
-        self.kernel_patch = ABAPSystem.check_kernel_patch(args["krnl_patch"]) if "krnl_patch" in args.keys() else ""
-        self.softs = ABAPSystem.parse_softs_file(args["softs"], root_dir) if "softs" in args.keys() else list()
-        if self.kernel_version == "" or len(self.softs) == 0:
-            raise ValueError("[ERROR] System '{}' you must specify 'soft' or 'krnl_version' keys"
+        self.kernel_version = ABAPSystem.check_kernel_version(args["krnl_version"]) \
+            if ("krnl_version" in args.keys() and args["krnl_version"] is not None and args["krnl_version"] != "") else ""
+
+        self.kernel_patch = ABAPSystem.check_kernel_patch(args["krnl_patch"]) \
+            if "krnl_patch" in args.keys() and args["krnl_patch"] is not None and args["krnl_patch"] != ""else ""
+
+        self.softs = ABAPSystem.parse_softs_file(args["softs"], root_dir) \
+            if "softs" in args.keys() else list()
+
+        if self.kernel_version == "" and len(self.softs) == 0:
+            raise ValueError("[ERROR] System '{}' you must specify 'softs' or 'krnl_version' keys"
                              .format(self.system_name))
+
         self.cwbntcust = ABAPSystem.parse_cwbntcust_file(args["cwbntcust"], root_dir, self.system_name) \
-            if "cwbntcust" in args.keys() else list()
+            if "cwbntcust" in args.keys() and args["cwbntcust"] is not None and args["cwbntcust"] != ""else list()
+
         self.exclude = ABAPSystem.parse_exclude_file(args["exclude"], root_dir, self.system_name) \
-            if "exclude" in args.keys() else list()
+            if "exclude" in args.keys() and args["exclude"] is not None and args["exclude"] != ""else list()
 
     @staticmethod
     def check_kernel_version(kernel_version):
         kernel_version = str(kernel_version).replace(',', '')
         kernel_version = kernel_version.replace('.', '')
         try:
             return int(kernel_version)
@@ -36,28 +49,27 @@
     @staticmethod
     def check_kernel_patch(kernel_patch):
         kernel_patch = str(kernel_patch).replace(',', '')
         kernel_patch = kernel_patch.replace('.', '')
         try:
             return int(kernel_patch)
         except ValueError:
-            raise ValueError("Kernel Version must be numeric. For example: 1100.")
+            raise ValueError("Kernel Patch Level must be numeric. For example: 1100.")
 
     @staticmethod
     def parse_softs_file(softs_file, root_dir):
         if root_dir:
             path = os.path.join(root_dir, softs_file)
         else:
             path = softs_file
         if not os.path.exists(path):
             raise FileNotFoundError("File %s not found" % (path,))
 
         if not softs_file.upper().endswith(".TXT"):
             raise ValueError("File {} has wrong extension. Only TXT files supported".format(softs_file))
-
         softs = list()
         with open(path, 'r', encoding="utf-8") as f:
             num = 0
             for line in f:
                 num += 1
                 line = line.strip('\r\n').strip()
                 line = re.sub(' +', ' ', line).split()
@@ -72,14 +84,15 @@
                     package = line[3]
                     softs.append((soft, version, pkg_num, package))
                 else:
                     print("[ERROR] File %s Line %s: %s" % (softs_file, str(num), " ".join(line)))
 
         if not len(softs):
             raise ValueError("File {} has wrong format".format(softs_file))
+
         return softs
 
     @staticmethod
     def parse_cwbntcust_file(cwbntcust_file, root_dir, system_name):
         if root_dir:
             path = os.path.join(root_dir, cwbntcust_file)
         else:
```

### Comparing `offlinesec_client-1.1.4/offlinesec_client/agr_1251.py` & `offlinesec_client-1.1.5/offlinesec_client/agr_1251.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/api_sec_notes.py` & `offlinesec_client-1.1.5/offlinesec_client/api_sec_notes.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/bo_system.py` & `offlinesec_client-1.1.5/offlinesec_client/bo_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/config.py` & `offlinesec_client-1.1.5/offlinesec_client/config.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/const.py` & `offlinesec_client-1.1.5/offlinesec_client/const.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/cwbntcust.py` & `offlinesec_client-1.1.5/offlinesec_client/cwbntcust.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/func.py` & `offlinesec_client-1.1.5/offlinesec_client/func.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 def check_server():
     conn = config.data[CONNECTION_STR]
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         result = sock.connect_ex((conn.split(":")[0], int(conn.split(":")[1])))
     except:
-        print("The Server %s not available now. Please try later" % (conn,))
+        print("The Offline Security Server %s not available now. Please try later" % (conn,))
         return False
 
     if result != 0:
-        print("The Server %s not available now. Please try later" % (conn,))
+        print("The Offline Security Server %s not available now. Please try later" % (conn,))
         return False
 
     sock.close()
     return True
 
 
 def get_connection_str(url):
```

### Comparing `offlinesec_client-1.1.4/offlinesec_client/get_reports.py` & `offlinesec_client-1.1.5/offlinesec_client/get_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         return
 
     if "errors" in response.keys() and response["errors"]:
         print("Some Reports not generated due to errors:")
         for error in response["errors"]:
             print(" * " + error)
 
-    print("%s report(s) are available to download from server" % (response["files_num"],))
+    print("%s report(s) are available to download from the server" % (response["files_num"],))
 
     i = 0
     for file in response["files"]:
         new_data = offlinesec_client.func.get_base_json(action=ACTION_GET_FILE)
         new_data[FILENAME] = file
         print("Downloading the report '%s'" % (file,))
         files = {'json': ('Get file', json.dumps(new_data), 'application/json')}
```

### Comparing `offlinesec_client-1.1.4/offlinesec_client/java_system.py` & `offlinesec_client-1.1.5/offlinesec_client/java_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/multi_systems.py` & `offlinesec_client-1.1.5/offlinesec_client/multi_systems.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_bo_notes.py` & `offlinesec_client-1.1.5/offlinesec_client/req_bo_notes.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_java_notes.py` & `offlinesec_client-1.1.5/offlinesec_client/req_java_notes.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_notes_report.py` & `offlinesec_client-1.1.5/offlinesec_client/req_notes_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import requests
 import argparse
 import os
 import sys
 import offlinesec_client.func
 from offlinesec_client.const import ERR_MESSAGE, FILE, SYSTEM_NAME, KRNL_PL, KRNL_VER, CWBNTCUST
+import abap_system
 import json
 import time
 
-UPLOAD_URL = "/file-upload"
+UPLOAD_URL = "/sec-notes"
 
 
 def check_version(s):
     return offlinesec_client.func.check_num_param("".join(s.split('.')), "Kernel Version")
 
 
 def check_patch_level(s):
@@ -37,71 +38,71 @@
     parser.add_argument("-s", "--%s" % (SYSTEM_NAME,), action="store", type=check_system_name,
                         help="SAP System Name (max 20 characters)", required=False)
     parser.add_argument("-k", "--%s" % (KRNL_VER,), action="store", type=check_version,
                         help="Kernel Version (for instance 7.53)", required=False)
     parser.add_argument("-p", "--%s" % (KRNL_PL,), action="store", type=check_patch_level,
                         help="Kernel Patch Level (for instance 1200)", required=False)
     parser.add_argument("-c", "--%s" % (CWBNTCUST,), action="store", type=check_cwbntcust,
-                        help="SAP System Name (max 20 characters)", required=False)
+                        help="CWBNTCUST table (txt or xlsx)", required=False)
     parser.add_argument("-e", "--exclude", action="store",
                         help='Exclude SAP security notes ("1111111, 2222222, 3333333")', required=False)
-    parser.add_argument('--wait', action='store_true', help="Wait 5 minutes and download the report")
+    parser.add_argument('-w', '--wait', action='store_true', help="Wait 5 minutes and download the report")
     parser.add_argument('--guiscript', action='store_true', help="Run GUI script to prepare the input data")
     parser.parse_args()
     return vars(parser.parse_args())
 
 
+def convert_to_dict(**args):
+    system_list = list()
+    new_abap_system = abap_system.ABAPSystem(args)
+    if new_abap_system is not None:
+        system_list.append(system_list)
+
+
 def send_file(file, system_name="", kernel_version="", kernel_patch="", cwbntcust="", exclude=""):
-    url = offlinesec_client.func.get_connection_str(UPLOAD_URL)
-    data = offlinesec_client.func.get_base_json(system_name=system_name,
-                                                kernel_version=kernel_version,
-                                                kernel_patch=kernel_patch,
-                                                cwbntcust=cwbntcust,
-                                                exclude=exclude)
-
-    files = {
-        'json': ('description', json.dumps(data), 'application/json'),
-        'file': (os.path.basename(file), open(file, 'rb'), 'application/octet-stream')
-    }
-    print("Uploading file %s" % (os.path.basename(file)))
-    r = requests.post(url, files=files)
-
-    if r.content:
-        try:
-            response = json.loads(r.content)
-            if ERR_MESSAGE in response:
-                print(" * " + response[ERR_MESSAGE])
-                return
-        except:
-            pass
+    additional_keys = dict()
+    system_list = list()
+
+    if system_name is None or system_name == "":
+        system_name = "ABAP System"
+
+    new_abap_system = abap_system.ABAPSystem(krnl_version=kernel_version,
+                                             krnl_patch=kernel_patch,
+                                             cwbntcust=cwbntcust,
+                                             exclude=exclude,
+                                             name=system_name,
+                                             softs=file)
+    if new_abap_system is not None:
+        system_list.append(new_abap_system)
 
-    print("No response from server. Please try later")
+    offlinesec_client.func.send_to_server(system_list, UPLOAD_URL, additional_keys)
 
 
 def process_it(file, system_name="", kernel_version="", kernel_patch="", cwbntcust="", guiscript=False, wait=False, exclude=""):
     if not offlinesec_client.func.check_server():
         return
 
     if guiscript:
         import platform
         if platform.system() == 'Windows':
             from offlinesec_client.sap_gui import SAPConnection
             conn = SAPConnection.sap_notes_report(system_name=system_name, wait=wait)
         else:
-            print("SAP GUI Scripting not supported on this platform")
+            print("SAP GUI Scripting not supported on this platform. Run SAP Gui Scripting only on Windows platform")
         return
 
     send_file(file, system_name, kernel_version, kernel_patch, cwbntcust, exclude)
 
     if wait:
         for remaining in range(310, 0, -1):
             sys.stdout.write("\r")
             sys.stdout.write("{:2d} seconds remaining.".format(remaining))
             sys.stdout.flush()
             time.sleep(1)
+        print("")
         os.system("offlinesec_get_reports")
 
 
 def main():
     args = init_args()
     if (FILE in args and args[FILE]) or ("guiscript" in args and args["guiscript"]):
         process_it(args[FILE], args[SYSTEM_NAME], args[KRNL_VER], args[KRNL_PL], args[CWBNTCUST], args["guiscript"], args["wait"], args["exclude"])
```

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_param_report.py` & `offlinesec_client-1.1.5/offlinesec_client/req_param_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_patch_day.py` & `offlinesec_client-1.1.5/offlinesec_client/req_patch_day.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_roles_report.py` & `offlinesec_client-1.1.5/offlinesec_client/req_roles_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/req_sec_notes.py` & `offlinesec_client-1.1.5/offlinesec_client/req_sec_notes.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/resolve_report.py` & `offlinesec_client-1.1.5/offlinesec_client/resolve_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/rsparam.py` & `offlinesec_client-1.1.5/offlinesec_client/rsparam.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client/sap_gui.py` & `offlinesec_client-1.1.5/offlinesec_client/sap_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import datetime
 import os
 from pathlib import Path
 
 
 class SAPConnection:
     @staticmethod
-    def sap_notes_report(system_name=None, wait=False):
+    def sap_notes_report(system_name=None, wait=False, exclude=None):
         try:
             sap_sessions = SAPExistedSession.get_multi_sap_session_with_info()
         except RuntimeError as error:
             print(str(error))
         else:
             if not len(sap_sessions):
                 print(' * Active SAP sessions not found. Do not forget to enable SAP GUI scripting')
@@ -57,15 +57,15 @@
 
                 else:
                     if os.path.exists(filename):
                         out_dict["cwbntcust"] = filename
                         print(" * The CWBNTCUST table +")
 
                 if len(out_dict):
-                    SAPConnection.send_it_to_server(out_dict,system_name,wait)
+                    SAPConnection.send_it_to_server(out_dict, system_name, wait)
 
     @staticmethod
     def load_software_components(sap_session):
         data = SAPSoftwareComponents.load_software_components(sap_session)
         if data:
             return data
```

### Comparing `offlinesec_client-1.1.4/offlinesec_client/sap_system.py` & `offlinesec_client-1.1.5/offlinesec_client/sap_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client.egg-info/PKG-INFO` & `offlinesec_client-1.1.5/offlinesec_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinesec-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: Offline Security Client
 Home-page: https://offlinesec.com
 Author: Offline Security
 Author-email: info@offlinesec.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `offlinesec_client-1.1.4/offlinesec_client.egg-info/SOURCES.txt` & `offlinesec_client-1.1.5/offlinesec_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/offlinesec_client.egg-info/entry_points.txt` & `offlinesec_client-1.1.5/offlinesec_client.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.4/setup.py` & `offlinesec_client-1.1.5/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/azcp_wrapper-0.0.5.tar.gz` & `tmp/azcp_wrapper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azcp_wrapper-0.0.5.tar", last modified: Wed May  8 02:31:49 2024, max compression
+gzip compressed data, was "azcp_wrapper-0.0.7.tar", last modified: Sat May 18 16:03:23 2024, max compression
```

## Comparing `azcp_wrapper-0.0.5.tar` & `azcp_wrapper-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:31:49.712906 azcp_wrapper-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 02:31:49.712906 azcp_wrapper-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:31:49.708906 azcp_wrapper-0.0.5/azcp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/azcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/azcp_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/azcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:31:49.708906 azcp_wrapper-0.0.5/azcp_wrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/azcp_wrapper/utils/execute_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:31:49.712906 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 02:31:49.000000 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 02:31:49.000000 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:31:49.000000 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 02:31:49.000000 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 02:31:49.000000 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 02:31:49.000000 azcp_wrapper-0.0.5/azcp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:31:49.712906 azcp_wrapper-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 02:31:42.000000 azcp_wrapper-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.414786 azcp_wrapper-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 16:03:23.414786 azcp_wrapper-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.410786 azcp_wrapper-0.0.7/azcp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/azcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/azcp_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14580 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/azcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.410786 azcp_wrapper-0.0.7/azcp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/azcp_wrapper/utils/execute_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:03:23.410786 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 16:03:23.000000 azcp_wrapper-0.0.7/azcp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:03:23.414786 azcp_wrapper-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-18 16:03:19.000000 azcp_wrapper-0.0.7/setup.py
```

### Comparing `azcp_wrapper-0.0.5/LICENSE` & `azcp_wrapper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.5/PKG-INFO` & `azcp_wrapper-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azcp_wrapper
-Version: 0.0.5
+Version: 0.0.7
 Summary: A simple AzCopy wrapper to transfer data
 Home-page: https://github.com/eabdala/azcp_wrapper
 Author: Erik Alejandro Abdala
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper/azcp_client.py` & `azcp_wrapper-0.0.7/azcp_wrapper/azcp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,26 @@
     Type,
     TypeVar,
     Union,
 )
 from azcp_wrapper.azcp_summary import (
     get_transfer_copy_summary_info,
     get_sync_summary_info,
+    get_transfer_list_summary_info,
 )
 
 from typing_extensions import Annotated, Doc
 from azcp_wrapper.azcp_utils import (
     AzCopyJobInfo,
     AzCopyOptions,
     AzLocalLocation,
     AzRemoteSASLocation,
     AzSyncJobInfo,
     AzSyncOptions,
+    AzListJobInfo,
     LocationType,
 )
 
 from pathlib import Path
 
 from azcp_wrapper.logging_config import run_name, run_log_directory, logger
 from azcp_wrapper.utils.execute_command import execute_command
@@ -52,29 +54,51 @@
         self,
         exe_to_use: Annotated[str, Doc("")] = "azcopy",
         process_name: Annotated[Optional[str], Doc("process_name")] = __name__,
         artefact_dir: Annotated[Optional[str], Doc("")] = None,
     ) -> None:
         self.exe_to_use = (
             exe_to_use
-            if not (Path("~/.azcp/azcopy.exe").expanduser().exists() or Path("~/.azcp/azcopy").expanduser().exists()) else Path("~/.azcp/azcopy").expanduser()
+            if not (
+                Path("~/.azcp/azcopy.exe").expanduser().exists()
+                or Path("~/.azcp/azcopy").expanduser().exists()
+            )
+            else Path("~/.azcp/azcopy").expanduser()
         )
         self.process_name = process_name
         self.artefact_dir = artefact_dir
         self.run_name, self.run_log_directory, self.logger = (
             run_name,
             run_log_directory,
             logger,
         )
         self.logger.info(f"Process Name: {self.process_name}")
         self.logger.info(f"Run name: {self.run_name}")
         self.logger.info(f"Run log directory: {self.run_log_directory}/{self.run_name}")
         self.logger.info(f"Executable to use: {self.exe_to_use}")
         # self.logger.warn([x for x in execute_command(['python','-m', 'pip', '-V'])])
 
+    def List(self, src: Union[AzRemoteSASLocation, AzLocalLocation]) -> AzListJobInfo:
+        cmd = [
+            self.exe_to_use,
+            "ls",
+            str(src),
+        ] + ["--running-tally"]
+        print(cmd)
+        summary = ""
+        job_info = AzListJobInfo()
+        for output_line in execute_command(cmd):
+            # print(output_line, end="")
+            # if "File count:" in output_line:
+            summary += output_line
+
+        job_info = get_transfer_list_summary_info(job_info, summary=summary)
+        str(job_info)
+        return job_info
+
     def copy(
         self,
         src: Union[AzRemoteSASLocation, AzLocalLocation],
         dest: Union[AzRemoteSASLocation, AzLocalLocation],
         transfer_options: AzCopyOptions,
     ) -> AzCopyJobInfo:
         """
@@ -164,95 +188,96 @@
             raise Exception(job_info.error_msg)
         else:
             job_info.error_msg += "; Error while transferring data"
             job_info.completed = False
             raise Exception(job_info.error_msg)
 
         return job_info
+
     def sync(
-            self,
-            src: Union[AzRemoteSASLocation, AzLocalLocation],
-            dest: Union[AzRemoteSASLocation, AzLocalLocation],
-            transfer_options: AzSyncOptions,
-        ) -> AzSyncJobInfo:
-            """
-            Syncs that data from source to destionation
-            with the transfer options specified
-            """
-            # Generating the command to be used for subprocess
-            cmd = [
-                self.exe_to_use,
-                "sync",
-                str(src),
-                str(dest),
-            ] + transfer_options.get_options_list()
-
-            # Creating AzSyncJobInfo object to store the job info
-            job_info = AzSyncJobInfo()
-
-            try:
-                summary = ""
-                # A boolean flag to be set as True when
-                # azcopy starts sending summary information
-                unlock_summary = False
-
-                for output_line in execute_command(cmd):
-                    print(output_line, end="")
-
-                    # Extracting the percent complete information from the
-                    # current output line and updating it in the job_info
-                    if "%" in output_line:
-
-                        percent_expression = r"(?P<percent_complete>\d+\.\d+) %,"
-                        transfer_match = re.match(percent_expression, output_line)
-
-                        if transfer_match is not None:
-                            transfer_info = transfer_match.groupdict()
-
-                            job_info.percent_complete = float(
-                                transfer_info["percent_complete"]
-                            )
-
-                    # If azcopy has started sending summary then
-                    # appending it to summary text
-                    if unlock_summary:
-                        summary += output_line.replace("(", "").replace(")", "")
-
-                    # Job summary starts with line ->
-                    # Job {job_id} summary
-                    output_line_cleaned = output_line.strip().lower()
-
-                    if (
-                        output_line_cleaned.startswith("job")
-                        and "summary" in output_line_cleaned
-                    ):
-                        unlock_summary = True
-
-                    if "AuthenticationFailed" in output_line:
-                        job_info.error_msg = output_line
-
-                    if "Final Job Status:" in output_line:
-                        job_info.final_job_status_msg = output_line.split(":")[-1].strip()
-
-            except Exception as e:
-                job_info.completed = False
-
-            # Get the final job summary info
-            job_info = get_sync_summary_info(job_info, summary)
-
-            if (
-                job_info.final_job_status_msg == "Completed"
-                or job_info.final_job_status_msg == "CompletedWithSkipped"
-            ):
-                job_info.completed = True
-            elif job_info.number_of_copy_transfers_failed > 0:
-                job_info.error_msg += "; Tranfers failed = {}".format(
-                    job_info.number_of_copy_transfers_failed
-                )
-                job_info.completed = False
-                raise Exception(job_info.error_msg)
-            else:
-                job_info.error_msg += "; Error while transferring data"
-                job_info.completed = False
-                raise Exception(job_info.error_msg)
+        self,
+        src: Union[AzRemoteSASLocation, AzLocalLocation],
+        dest: Union[AzRemoteSASLocation, AzLocalLocation],
+        transfer_options: AzSyncOptions,
+    ) -> AzSyncJobInfo:
+        """
+        Syncs that data from source to destionation
+        with the transfer options specified
+        """
+        # Generating the command to be used for subprocess
+        cmd = [
+            self.exe_to_use,
+            "sync",
+            str(src),
+            str(dest),
+        ] + transfer_options.get_options_list()
+
+        # Creating AzSyncJobInfo object to store the job info
+        job_info = AzSyncJobInfo()
+
+        try:
+            summary = ""
+            # A boolean flag to be set as True when
+            # azcopy starts sending summary information
+            unlock_summary = False
+
+            for output_line in execute_command(cmd):
+                print(output_line, end="")
+
+                # Extracting the percent complete information from the
+                # current output line and updating it in the job_info
+                if "%" in output_line:
+
+                    percent_expression = r"(?P<percent_complete>\d+\.\d+) %,"
+                    transfer_match = re.match(percent_expression, output_line)
+
+                    if transfer_match is not None:
+                        transfer_info = transfer_match.groupdict()
+
+                        job_info.percent_complete = float(
+                            transfer_info["percent_complete"]
+                        )
+
+                # If azcopy has started sending summary then
+                # appending it to summary text
+                if unlock_summary:
+                    summary += output_line.replace("(", "").replace(")", "")
+
+                # Job summary starts with line ->
+                # Job {job_id} summary
+                output_line_cleaned = output_line.strip().lower()
+
+                if (
+                    output_line_cleaned.startswith("job")
+                    and "summary" in output_line_cleaned
+                ):
+                    unlock_summary = True
+
+                if "AuthenticationFailed" in output_line:
+                    job_info.error_msg = output_line
+
+                if "Final Job Status:" in output_line:
+                    job_info.final_job_status_msg = output_line.split(":")[-1].strip()
 
-            return job_info
+        except Exception as e:
+            job_info.completed = False
+
+        # Get the final job summary info
+        job_info = get_sync_summary_info(job_info, summary)
+
+        if (
+            job_info.final_job_status_msg == "Completed"
+            or job_info.final_job_status_msg == "CompletedWithSkipped"
+        ):
+            job_info.completed = True
+        elif job_info.number_of_copy_transfers_failed > 0:
+            job_info.error_msg += "; Tranfers failed = {}".format(
+                job_info.number_of_copy_transfers_failed
+            )
+            job_info.completed = False
+            raise Exception(job_info.error_msg)
+        else:
+            job_info.error_msg += "; Error while transferring data"
+            job_info.completed = False
+            raise Exception(job_info.error_msg)
+
+        return job_info
```

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper/azcp_summary.py` & `azcp_wrapper-0.0.7/azcp_wrapper/azcp_summary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
 
-from azcp_wrapper.azcp_utils import AzCopyJobInfo, AzSyncJobInfo
+from azcp_wrapper.azcp_utils import AzCopyJobInfo, AzSyncJobInfo, AzListJobInfo
 
 
 def get_property_value(key: str, job_summary: str) -> int:
     property_value = 0
 
     try:
-        property_key_match = re.search(r"{}: (\d+(\.\d+)?)".format(re.escape(key)), job_summary)
+        property_key_match = re.search(
+            r"{}: (\d+(\.\d+)?)".format(re.escape(key)), job_summary
+        )
         # print(r"{}: (\d+(\.\d+)?)".format(re.escape(key)),property_key_match)
         if property_key_match is not None:
 
             property_key_text = property_key_match.group()
             property_value_match = re.search(r"(\d+(\.\d+)?)", property_key_text)
 
             # If the property key text exists in the job summary,
@@ -20,14 +22,50 @@
                 property_value = str(property_value_match.group())
     except Exception as e:
         print(e)
 
     return property_value
 
 
+def get_transfer_list_summary_info(
+    job_info: AzListJobInfo, summary: str
+) -> AzListJobInfo:
+    """
+    Extract all properties of Job Info from the Azcopy job summary
+    """
+    properties_required = [
+        "File count",
+        "Total file size",
+    ]
+
+    for property_key in properties_required:
+
+        # Converting the property key string to attribute form
+        property_attribute = property_key.lower().replace(" ", "_")
+        property_value = get_property_value(property_key, summary)
+
+        # Set the attribute in job_info object
+        setattr(job_info, property_attribute, property_value)
+    # Crear una lista para almacenar los datos
+    file_data = []
+
+    # Usar una expresión regular para encontrar todos los pares archivo-tamaño
+    pattern = re.compile(r"INFO: ([^;]+);  Content Length: ([\d.]+ \w+)")
+    matches = pattern.findall(summary)
+
+    # Rellenar la lista con los datos encontrados
+    for match in matches:
+        file_name, content_length = match
+        file_info = {"Archivo": file_name.strip(), "peso": content_length.strip()}
+        file_data.append(file_info)
+
+    job_info.list_files = file_data
+    return job_info
+
+
 def get_transfer_copy_summary_info(
     job_info: AzCopyJobInfo, summary: str
 ) -> AzCopyJobInfo:
     """
     Extract all properties of Job Info from the Azcopy job summary
     """
     properties_required = [
@@ -105,8 +143,7 @@
     #     # the gets the property value
     #     if property_value_match is not None:
     #         property_value = float(property_value_match.group())  # type: ignore
 
     # sync_job_info.elapsed_time_minutes = property_value
 
     return sync_job_info
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper/azcp_utils.py` & `azcp_wrapper-0.0.7/azcp_wrapper/azcp_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 )
 from typing_extensions import Annotated, Doc
 import time
 import datetime
 from urllib.parse import parse_qs
 from azcp_wrapper.logging_config import logger
 
+
 class LocationType:
     """
     This type is used to specify the location
     type of the object created for transfer
     for the AzCopy command
     """
 
     SRC = "source"
     DEST = "destination"
 
+
 class AzRemoteSASLocation:
     """
     Class to create Azure Remote Location with SAS Token
     Returns the remote location url string with the information
     specified while creating the object
     """
 
@@ -39,31 +41,30 @@
         self,
         storage_account: Annotated[str, Doc("")] = "",
         container: Annotated[str, Doc("")] = "",
         path: Annotated[str, Doc("")] = "",
         use_wildcard: Annotated[bool, Doc("")] = False,
         sas_token: Annotated[str, Doc("")] = "",
         location_type: Annotated[Optional[str], Doc("")] = None,
-        blob_or_file: Annotated[str, Doc("")] = 'blob'
+        blob_or_file: Annotated[str, Doc("")] = "blob",
     ) -> None:
         if len(sas_token) > 0:
             sas_token_expiry_flag = self.is_sas_token_session_expired(token=sas_token)
 
             if sas_token_expiry_flag == True:
                 raise Exception("SAS token is expired")
 
         self.storage_account = storage_account
         self.container = container
         self.sas_token = sas_token
         self.use_wildcard = use_wildcard
         self.path = path
         self.location_type = location_type
         self.logger = logger
-        self.blob_or_file = blob_or_file.lower() if blob_or_file is not None else 'blob' 
-
+        self.blob_or_file = blob_or_file.lower() if blob_or_file is not None else "blob"
 
     def is_sas_token_session_expired(self, token: str) -> bool:
         """
         Checks if the SAS token is expired
         """
         parsed = parse_qs(token.lstrip("?"))
 
@@ -88,40 +89,42 @@
         current_unix_timestamp = int(time.mktime(current_timestamp.timetuple()))
 
         if current_unix_timestamp > session_expiry_unix_timestamp:
             return True
         else:
             return False
 
-
     def get_resource_uri(self) -> str:
         url = f"https://{self.storage_account}.{self.blob_or_file}.core.windows.net/{self.container}/"
-        self.logger.info(f'URL: {url}')
+        self.logger.info(f"URL: {url}")
         return url
-    
+
     def __str__(self) -> str:
         """
         Creates the remote location url with sas token to be used for the final location
         """
         if len(self.sas_token) > 0:
-            sas_token_expiry_flag = self.is_sas_token_session_expired(token=self.sas_token)
+            sas_token_expiry_flag = self.is_sas_token_session_expired(
+                token=self.sas_token
+            )
 
             if sas_token_expiry_flag == True:
-                
+
                 raise Exception("SAS token is expired")
 
         resource_uri = self.get_resource_uri()
 
         wildcard = ""
         if self.use_wildcard == True:
             wildcard = "*"
 
         all_command = resource_uri + self.path + wildcard + "?" + self.sas_token
         return all_command
 
+
 class AzLocalLocation:
     """
     Class to create Local Path for data transfer using Azcopy
     """
 
     path: str
     use_wildcard: bool
@@ -140,87 +143,179 @@
     def __str__(self) -> str:
         wildcard = ""
         if self.use_wildcard == True:
             wildcard = "*"
 
         return self.path + wildcard
 
+
 @dataclass
 class AzCopyOptions:
-    as_subdir: Annotated[bool, Doc("Places folder sources as subdirectories under the destination.")] = None
-    force_if_read_only: Annotated[bool, Doc("Places folder sources as subdirectories under the destination.")] = None
-    block_size_mb: Annotated[str, Doc("Use this block size (specified in MiB) when uploading to Azure Storage, and downloading from Azure Storage.")] = None
-    check_length: Annotated[bool, Doc("Check the length of a file on the destination after the transfer.")] = None
-    dry_run: Annotated[str, Doc("Prints the file paths that would be copied by this command.")] = None
-    exclude_path: Annotated[str, Doc("Exclude these paths when copying. This option doesn't support wildcard characters (*). Checks relative path prefix.")] = None
-    exclude_pattern: Annotated[str, Doc("Exclude these files when copying. This option supports wildcard characters (*).")] = None
+    as_subdir: Annotated[
+        bool, Doc("Places folder sources as subdirectories under the destination.")
+    ] = None
+    force_if_read_only: Annotated[
+        bool, Doc("Places folder sources as subdirectories under the destination.")
+    ] = None
+    block_size_mb: Annotated[
+        str,
+        Doc(
+            "Use this block size (specified in MiB) when uploading to Azure Storage, and downloading from Azure Storage."
+        ),
+    ] = None
+    check_length: Annotated[
+        bool, Doc("Check the length of a file on the destination after the transfer.")
+    ] = None
+    dry_run: Annotated[
+        str, Doc("Prints the file paths that would be copied by this command.")
+    ] = None
+    exclude_path: Annotated[
+        str,
+        Doc(
+            "Exclude these paths when copying. This option doesn't support wildcard characters (*). Checks relative path prefix."
+        ),
+    ] = None
+    exclude_pattern: Annotated[
+        str,
+        Doc(
+            "Exclude these files when copying. This option supports wildcard characters (*)."
+        ),
+    ] = None
     exclude_regex: Annotated[str, Doc("")] = None
     follow_symlinks: Annotated[str, Doc("")] = None
     include_after: Annotated[str, Doc("")] = None
     include_before: Annotated[str, Doc("")] = None
     include_path: Annotated[str, Doc("")] = None
     include_pattern: Annotated[str, Doc("")] = None
     include_regex: Annotated[str, Doc("")] = None
-    log_level: Annotated[str, Doc("Define the log verbosity for the log file, available levels: INFO, WARNING, ERROR, and NONE.")] = None
-    metadata: Annotated[str, Doc("Upload to Azure Storage with these key-value pairs as metadata.") ]= None
-    overwrite: Annotated[str, Doc("""# Overwrite the conflicting files and blobs at the destination if this flag is set to true.
+    log_level: Annotated[
+        str,
+        Doc(
+            "Define the log verbosity for the log file, available levels: INFO, WARNING, ERROR, and NONE."
+        ),
+    ] = None
+    metadata: Annotated[
+        str, Doc("Upload to Azure Storage with these key-value pairs as metadata.")
+    ] = None
+    overwrite: Annotated[
+        str,
+        Doc(
+            """# Overwrite the conflicting files and blobs at the destination if this flag is set to true.
                                     # Possible values include 'true', 'false', 'prompt', and 'ifSourceNewer'.
-                                    # """)] = 'ifSourceNewer'
-    put_md5: Annotated[bool, Doc("Create an MD5 hash of each file, and save the hash as the Content-MD5 property of the destination blob or file.")] = None
-    recursive: Annotated[bool, Doc("Look into subdirectories recursively when uploading from local file system.")] = True
+                                    # """
+        ),
+    ] = "ifSourceNewer"
+    put_md5: Annotated[
+        bool,
+        Doc(
+            "Create an MD5 hash of each file, and save the hash as the Content-MD5 property of the destination blob or file."
+        ),
+    ] = None
+    recursive: Annotated[
+        bool,
+        Doc(
+            "Look into subdirectories recursively when uploading from local file system."
+        ),
+    ] = True
 
     def get_options_list(self):
         dict_conf = asdict(self)
-        config = {k.replace('_','-'): v for k, v in dict_conf.items() if v != 'NULL'}
+        config = {k.replace("_", "-"): v for k, v in dict_conf.items() if v != "NULL"}
         cmd_parts = []
         for option, value in config.items():
             if isinstance(value, bool) and value:
                 cmd_parts.append(f"--{option}=true")
             elif value is not None:
                 cmd_parts.append(f"--{option}={value}")
         return cmd_parts
 
+
 @dataclass
 class AzSyncOptions:
-   
-    exclude_path: Annotated[str, Doc("Exclude these paths when copying. This option doesn't support wildcard characters (*). Checks relative path prefix.")] = None
-    put_md5: Annotated[bool, Doc("Create an MD5 hash of each file, and save the hash as the Content-MD5 property of the destination blob or file.")] = None
-    recursive: Annotated[bool, Doc("Look into subdirectories recursively when uploading from local file system.")] = True
+
+    exclude_path: Annotated[
+        str,
+        Doc(
+            "Exclude these paths when copying. This option doesn't support wildcard characters (*). Checks relative path prefix."
+        ),
+    ] = None
+    put_md5: Annotated[
+        bool,
+        Doc(
+            "Create an MD5 hash of each file, and save the hash as the Content-MD5 property of the destination blob or file."
+        ),
+    ] = None
+    recursive: Annotated[
+        bool,
+        Doc(
+            "Look into subdirectories recursively when uploading from local file system."
+        ),
+    ] = True
 
     def get_options_list(self):
         dict_conf = asdict(self)
-        config = {k.replace('_','-'): v for k, v in dict_conf.items() if v != 'NULL'}
+        config = {k.replace("_", "-"): v for k, v in dict_conf.items() if v != "NULL"}
         cmd_parts = []
         for option, value in config.items():
             if isinstance(value, bool) and value:
                 cmd_parts.append(f"--{option}=true")
             elif value is not None:
                 cmd_parts.append(f"--{option}={value}")
         return cmd_parts
 
-class AzCopyJobInfo:
+
+class AzListJobInfo:
     """
     Created the job info of the Azcopy job executed by the user
     """
 
+    def __init__(
+        self,
+        file_count: Annotated[int, Doc("")] = 0,
+        total_file_size: Annotated[float, Doc("")] = float(0),
+        list_files: Annotated[Dict, Doc("")] = dict(),
+    ) -> None:
+        self.file_count = file_count
+        self.total_file_size = total_file_size
+        self.logger = logger
+        self.list_files = list_files
+
+    def __str__(self) -> str:
+        """
+        Get a human-readable string representation of the AzCopyJobInfo object.
+        """
+        self.logger.info(f"AzCopy Job Info List:")
+        self.logger.info(f"File count: {self.file_count}")
+        self.logger.info(f"Total file size: {self.total_file_size} GB")
+        return (
+            f"AzCopy Job Info List:\n"
+            f"File count: {self.file_count}\n"
+            f"Total file size: {self.total_file_size}GB"
+        )
+
+
+class AzCopyJobInfo:
+    """
+    Created the job info of the Azcopy job executed by the user
+    """
 
     def __init__(
         self,
         percent_complete: Annotated[float, Doc("")] = float(0),
         elapsed_time_minutes: Annotated[float, Doc("")] = float(0),
         error_msg: Annotated[str, Doc("")] = "",
         final_job_status_msg: Annotated[str, Doc("")] = "",
         number_of_file_transfers: Annotated[int, Doc("")] = 0,
         number_of_folder_property_transfers: Annotated[int, Doc("")] = 0,
         total_number_of_transfers: Annotated[int, Doc("")] = 0,
         number_of_transfers_completed: Annotated[int, Doc("")] = 0,
-        number_of_transfers_failed: Annotated[int , Doc("")]= 0,
+        number_of_transfers_failed: Annotated[int, Doc("")] = 0,
         number_of_file_transfers_skipped: Annotated[int, Doc("")] = 0,
         total_bytes_transferred: Annotated[int, Doc("")] = 0,
-        completed: Annotated[bool, Doc("")]= False,
+        completed: Annotated[bool, Doc("")] = False,
     ) -> None:
         # NOTE: Sometimes, azcopy doesn't return value as 100%
         # even if the entire data is transferred.
         # This might be because if the transfer is completed in between
         # the value sent by azcopy, then azcopy fails to send the final
         # percent value and directly sends the job summary
         self.percent_complete = percent_complete
@@ -231,35 +326,37 @@
         self.number_of_folder_property_transfers = number_of_folder_property_transfers
         self.total_number_of_transfers = total_number_of_transfers
         self.number_of_transfers_completed = number_of_transfers_completed
         self.number_of_transfers_failed = number_of_transfers_failed
         self.number_of_file_transfers_skipped = number_of_file_transfers_skipped
         self.total_bytes_transferred = total_bytes_transferred
         self.completed = completed
+
     def __str__(self) -> str:
         """
         Get a human-readable string representation of the AzCopyJobInfo object.
         """
-        return f"AzCopy Job Info:\n" \
-            f"Elapsed Time (Minutes): {self.elapsed_time_minutes}\n" \
-               f"Percent Complete: {self.percent_complete}%\n" \
-               f"Final Job Status: {self.final_job_status_msg}\n" \
-                f"Number of File Transfers: {self.number_of_file_transfers}\n" \
-               f"Transfers Completed: {self.number_of_transfers_completed}\n" \
-               f"Transfers Failed: {self.number_of_transfers_failed}\n" \
-               f"Transfers Skipped: {self.number_of_file_transfers_skipped}\n" \
-               f"Total Bytes Transferred: {self.total_bytes_transferred}"
+        return (
+            f"AzCopy Job Info:\n"
+            f"Elapsed Time (Minutes): {self.elapsed_time_minutes}\n"
+            f"Percent Complete: {self.percent_complete}%\n"
+            f"Final Job Status: {self.final_job_status_msg}\n"
+            f"Number of File Transfers: {self.number_of_file_transfers}\n"
+            f"Transfers Completed: {self.number_of_transfers_completed}\n"
+            f"Transfers Failed: {self.number_of_transfers_failed}\n"
+            f"Transfers Skipped: {self.number_of_file_transfers_skipped}\n"
+            f"Total Bytes Transferred: {self.total_bytes_transferred}"
+        )
 
 
 class AzSyncJobInfo:
     """
     Created the job info of the Azcopy job executed by the user
     """
 
-
     def __init__(
         self,
         percent_complete: Annotated[float, Doc("")] = float(0),
         error_msg: Annotated[str, Doc("")] = "",
         files_scanned_at_source: Annotated[int, Doc("")] = 0,
         files_scanned_at_destination: Annotated[int, Doc("")] = 0,
         # elapsed_time_minutes: float = float(0),
@@ -267,16 +364,16 @@
         number_of_copy_transfers_for_folder_properties: Annotated[int, Doc("")] = 0,
         number_of_folder_property_transfers: Annotated[int, Doc("")] = 0,
         total_number_of_copy_transfers: Annotated[int, Doc("")] = 0,
         number_of_copy_transfers_completed: Annotated[int, Doc("")] = 0,
         number_of_copy_transfers_failed: Annotated[int, Doc("")] = 0,
         number_of_deletions_at_destination: Annotated[int, Doc("")] = 0,
         total_number_of_bytes_transferred: Annotated[int, Doc("")] = 0,
-        total_number_of_bytes_enumerated: Annotated[int , Doc("")]= 0,
-        final_job_status_msg: Annotated[str , Doc("")]= "",
+        total_number_of_bytes_enumerated: Annotated[int, Doc("")] = 0,
+        final_job_status_msg: Annotated[str, Doc("")] = "",
         completed: Annotated[bool, Doc("")] = False,
     ) -> None:
         # NOTE: Sometimes, azcopy doesn't return value as 100%
         # even if the entire data is transferred.
         # This might be because if the transfer is completed in between
         # the value sent by azcopy, then azcopy fails to send the final
         # percent value and directly sends the job summary
@@ -293,8 +390,8 @@
         self.number_of_folder_property_transfers = number_of_folder_property_transfers
         self.total_number_of_copy_transfers = total_number_of_copy_transfers
         self.number_of_copy_transfers_completed = number_of_copy_transfers_completed
         self.number_of_copy_transfers_failed = number_of_copy_transfers_failed
         self.number_of_deletions_at_destination = number_of_deletions_at_destination
         self.total_number_of_bytes_transferred = total_number_of_bytes_transferred
         self.total_number_of_bytes_enumerated = total_number_of_bytes_enumerated
-        self.completed = completed
+        self.completed = completed
```

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper/logging_config.py` & `azcp_wrapper-0.0.7/azcp_wrapper/logging_config.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper/setup.py` & `azcp_wrapper-0.0.7/azcp_wrapper/setup.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper/utils/execute_command.py` & `azcp_wrapper-0.0.7/azcp_wrapper/utils/execute_command.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.5/azcp_wrapper.egg-info/PKG-INFO` & `azcp_wrapper-0.0.7/azcp_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azcp_wrapper
-Version: 0.0.5
+Version: 0.0.7
 Summary: A simple AzCopy wrapper to transfer data
 Home-page: https://github.com/eabdala/azcp_wrapper
 Author: Erik Alejandro Abdala
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azcp_wrapper-0.0.5/setup.py` & `azcp_wrapper-0.0.7/setup.py`

 * *Files identical despite different names*


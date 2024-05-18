# Comparing `tmp/aind_data_transfer_models-0.2.0.tar.gz` & `tmp/aind_data_transfer_models-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_data_transfer_models-0.2.0.tar", last modified: Thu May  9 21:37:33 2024, max compression
+gzip compressed data, was "aind_data_transfer_models-0.3.0.tar", last modified: Sat May 18 00:10:59 2024, max compression
```

## Comparing `aind_data_transfer_models-0.2.0.tar` & `aind_data_transfer_models-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.987480 aind_data_transfer_models-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.979480 aind_data_transfer_models-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.979480 aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-09 21:37:33.987480 aind_data_transfer_models-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:37:33.987480 aind_data_transfer_models-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.979480 aind_data_transfer_models-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 21:37:24.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-09 21:37:33.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-09 21:37:33.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:37:33.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-09 21:37:33.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 21:37:33.000000 aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:37:33.983480 aind_data_transfer_models-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-09 21:37:23.000000 aind_data_transfer_models-0.2.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.288639 aind_data_transfer_models-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.288639 aind_data_transfer_models-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.296639 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 00:10:59.000000 aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 00:10:59.292639 aind_data_transfer_models-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-18 00:10:46.000000 aind_data_transfer_models-0.3.0/tests/test_core.py
```

### Comparing `aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_data_transfer_models-0.3.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/.github/workflows/tag_and_publish.yml` & `aind_data_transfer_models-0.3.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/.github/workflows/test_and_lint.yml` & `aind_data_transfer_models-0.3.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/.gitignore` & `aind_data_transfer_models-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/LICENSE` & `aind_data_transfer_models-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/PKG-INFO` & `aind_data_transfer_models-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: aind-data-transfer-models
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: aind-data-schema-models==0.1.1
 Requires-Dist: aind-slurm-rest==0.1.0
+Requires-Dist: email-validator
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
```

### Comparing `aind_data_transfer_models-0.2.0/README.md` & `aind_data_transfer_models-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/doc_template/Makefile` & `aind_data_transfer_models-0.3.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/doc_template/make.bat` & `aind_data_transfer_models-0.3.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/doc_template/source/_static/dark-logo.svg` & `aind_data_transfer_models-0.3.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/doc_template/source/_static/favicon.ico` & `aind_data_transfer_models-0.3.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/doc_template/source/_static/light-logo.svg` & `aind_data_transfer_models-0.3.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/doc_template/source/conf.py` & `aind_data_transfer_models-0.3.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_data_transfer_models-0.2.0/pyproject.toml` & `aind_data_transfer_models-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
     'pydantic>=2.0',
     'pydantic-settings>=2.0',
     'aind-data-schema-models==0.1.1',
-    'aind-slurm-rest==0.1.0'
+    'aind-slurm-rest==0.1.0',
+    'email-validator'
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
     'flake8',
```

### Comparing `aind_data_transfer_models-0.2.0/src/aind_data_transfer_models/core.py` & `aind_data_transfer_models-0.3.0/src/aind_data_transfer_models/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 """Core models for using aind-data-transfer-service"""
 
 import re
 from datetime import datetime
 from enum import Enum
 from pathlib import PurePosixPath
-from typing import Any, ClassVar, List, Optional, Union
+from typing import Any, ClassVar, List, Optional, Set, Union
 
 from aind_data_schema_models.data_name_patterns import build_data_name
 from aind_data_schema_models.modalities import Modality
 from aind_data_schema_models.platforms import Platform
 from aind_slurm_rest import V0036JobSubmission
 from pydantic import (
     ConfigDict,
+    EmailStr,
     Field,
     ValidationInfo,
     computed_field,
     field_validator,
 )
 from pydantic_settings import BaseSettings
 
 
+class EmailNotificationType(str, Enum):
+    """Types of email notifications a user can select"""
+
+    BEGIN = "begin"
+    END = "end"
+    FAIL = "fail"
+    RETRY = "retry"
+    ALL = "all"
+
+
 class BucketType(str, Enum):
     """Types of s3 bucket users can write to through service"""
 
     PRIVATE = "private"
     OPEN = "open"
     SCRATCH = "scratch"
 
@@ -107,15 +118,14 @@
     model_config = ConfigDict(extra="allow", use_enum_values=True)
 
     # Need some way to extract abbreviations. Maybe a public method can be
     # added to the Platform class
     _PLATFORM_MAP: ClassVar = {
         p().abbreviation.upper(): p().abbreviation for p in Platform._ALL
     }
-    _MODALITY_ENTRY_PATTERN: ClassVar = re.compile(r"^modality(\d*)$")
     _DATETIME_PATTERN1: ClassVar = re.compile(
         r"^\d{4}-\d{2}-\d{2}[ |T]\d{2}:\d{2}:\d{2}$"
     )
     _DATETIME_PATTERN2: ClassVar = re.compile(
         r"^\d{1,2}/\d{1,2}/\d{4} \d{1,2}:\d{2}:\d{2} [APap][Mm]$"
     )
 
@@ -227,7 +237,28 @@
         elif is_str:
             raise ValueError(
                 "Incorrect datetime format, should be"
                 " YYYY-MM-DD HH:mm:ss or MM/DD/YYYY I:MM:SS P"
             )
         else:
             return datetime_val
+
+
+class SubmitJobRequest(BaseSettings):
+    """Main request that will be sent to the backend. Bundles jobs into a list
+    and allows a user to add an email address to receive notifications."""
+
+    user_email: Optional[EmailStr] = Field(
+        default=None,
+        description=(
+            "Optional email address to receive job status notifications"
+        ),
+    )
+    email_notification_types: Set[EmailNotificationType] = Field(
+        default={EmailNotificationType.FAIL},
+        description=(
+            "Types of job statuses to receive email notifications about"
+        ),
+    )
+    upload_jobs: List[BasicUploadJobConfigs] = Field(
+        ..., description="List of upload jobs to process"
+    )
```

### Comparing `aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/PKG-INFO` & `aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: aind-data-transfer-models
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pydantic-settings>=2.0
 Requires-Dist: aind-data-schema-models==0.1.1
 Requires-Dist: aind-slurm-rest==0.1.0
+Requires-Dist: email-validator
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
```

### Comparing `aind_data_transfer_models-0.2.0/src/aind_data_transfer_models.egg-info/SOURCES.txt` & `aind_data_transfer_models-0.3.0/src/aind_data_transfer_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


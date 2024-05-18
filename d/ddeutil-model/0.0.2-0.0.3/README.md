# Comparing `tmp/ddeutil_model-0.0.2.tar.gz` & `tmp/ddeutil_model-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_model-0.0.2.tar", last modified: Wed May 15 14:17:41 2024, max compression
+gzip compressed data, was "ddeutil_model-0.0.3.tar", last modified: Sat May 18 12:23:40 2024, max compression
```

## Comparing `ddeutil_model-0.0.2.tar` & `ddeutil_model-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.541697 ddeutil_model-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.541697 ddeutil_model-0.0.2/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.545697 ddeutil_model-0.0.2/src/ddeutil/model/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__enums.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/__types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.545697 ddeutil_model-0.0.2/src/ddeutil/model/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/col.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/datasets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/src/ddeutil/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 14:17:41.000000 ddeutil_model-0.0.2/src/ddeutil_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:17:41.549697 ddeutil_model-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dataset_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dataset_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 14:17:37.000000 ddeutil_model-0.0.2/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.788979 ddeutil_model-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 12:23:40.788979 ddeutil_model-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.780979 ddeutil_model-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.780979 ddeutil_model-0.0.3/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/src/ddeutil/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/__types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/src/ddeutil/model/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/datasets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/src/ddeutil/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 12:23:40.000000 ddeutil_model-0.0.3/src/ddeutil_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 12:23:40.784979 ddeutil_model-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dataset_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dataset_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 12:23:33.000000 ddeutil_model-0.0.3/tests/test_types.py
```

### Comparing `ddeutil_model-0.0.2/LICENSE` & `ddeutil_model-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/PKG-INFO` & `ddeutil_model-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Developer & Engineer Model Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil-model/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil-model/
 Keywords: data,model,utility,pipeline
 Classifier: Topic :: Utilities
@@ -23,14 +23,18 @@
 License-File: LICENSE
 Requires-Dist: ddeutil
 Requires-Dist: tzdata
 Requires-Dist: pydantic==2.7.1
 
 # Data Utility Package: *Model*
 
+[![test](https://github.com/ddeutils/ddeutil-model/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ddeutils/ddeutil-model/actions/workflows/tests.yml)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ddeutil-model?logo=pypi)](https://pypi.org/project/ddeutil-model/)
+[![size](https://img.shields.io/github/languages/code-size/ddeutils/ddeutil-model)](https://github.com/ddeutils/ddeutil-model)
+
 **Table of Contents**:
 
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
```

### Comparing `ddeutil_model-0.0.2/README.md` & `ddeutil_model-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Data Utility Package: *Model*
 
+[![test](https://github.com/ddeutils/ddeutil-model/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ddeutils/ddeutil-model/actions/workflows/tests.yml)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ddeutil-model?logo=pypi)](https://pypi.org/project/ddeutil-model/)
+[![size](https://img.shields.io/github/languages/code-size/ddeutils/ddeutil-model)](https://github.com/ddeutils/ddeutil-model)
+
 **Table of Contents**:
 
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
```

### Comparing `ddeutil_model-0.0.2/pyproject.toml` & `ddeutil_model-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 
 [tool.ruff]
 line-length = 80
 exclude = [
     ".git",
     ".mypy_cache",
     ".ruff_cache",
+    ".venv",
     "__pypackages__",
     "build",
     "dist",
     "venv",
 ]
 
 [tool.ruff.lint]
```

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/__base.py` & `ddeutil_model-0.0.3/src/ddeutil/model/__base.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/__enums.py` & `ddeutil_model-0.0.3/src/ddeutil/model/__enums.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/__types.py` & `ddeutil_model-0.0.3/src/ddeutil/model/__types.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/action.py` & `ddeutil_model-0.0.3/src/ddeutil/model/action.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/conn.py` & `ddeutil_model-0.0.3/src/ddeutil/model/conn.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,24 +12,56 @@
     Optional,
     Union,
 )
 
 from pydantic import Field
 from pydantic.functional_validators import field_validator
 from pydantic.types import SecretStr
+from pydantic_core import Url
 
 from .__base import BaseUpdatableModel
 from .__types import CustomUrl, FileUrl
 from .utils import unquote_str
 
 
 class BaseConn(BaseUpdatableModel):
     type: str = "base"
 
 
+class Conn(BaseConn):
+    type: Literal["conn"] = "conn"
+    dialect: str
+    host: Optional[str] = None
+    port: Optional[int] = None
+    user: Optional[str] = None
+    pwd: Optional[SecretStr] = None
+    endpoint: Optional[str] = None
+    options: Annotated[dict[str, Any], Field(default_factory=dict)]
+
+    @classmethod
+    def from_url(cls, url: Union[Url, str]) -> Conn:
+        if isinstance(url, str):
+            url = Url(url=url)
+        elif not isinstance(url, Url):
+            raise ValueError("A url value must be string or `CustomUrl` object")
+        return cls(
+            dialect=url.scheme,
+            host=unquote_str(url.host),
+            port=url.port,
+            user=unquote_str(url.username),
+            pwd=unquote_str(url.password),
+            endpoint=url.path,
+            options=dict(url.query_params()),
+        )
+
+    @field_validator("endpoint")
+    def __check_endpoint_name(cls, v: str) -> str:
+        return v.lstrip("/")
+
+
 class FlConn(BaseConn):
     type: Literal["file"] = "file"
     sys: str
     pointer: Optional[str] = None
     port: Optional[int] = None
     user: Optional[str] = None
     pwd: Optional[SecretStr] = None
@@ -86,8 +118,8 @@
             pwd=unquote_str(url.password),
             db=url.path,
             options=dict(url.query_params()),
         )
 
     @field_validator("db")
     def __check_db_name(cls, v: str) -> str:
-        return v.split("/")[0]
+        return v.lstrip("/").split("/")[0]
```

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/const.py` & `ddeutil_model-0.0.3/src/ddeutil/model/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,20 @@
     Optional,
 )
 
 from pydantic import BaseModel, Field
 
 
 class Const(BaseModel):
-    """Constraint Model"""
+    """Constraint Model
+
+    Examples:
+        >>> Const(of='foo').name
+        'foo_const'
+    """
 
     of: Annotated[
         Optional[str],
         Field(description="Owner of Constraint"),
     ] = None
 
     @property
@@ -54,29 +59,31 @@
         raise ValueError("This primary key does not have any columns.")
 
 
 class Ref(BaseModel):
     """Reference Model
 
     Examples:
-        *   {
-                "tbl": "foo",
-                "col": "bar",
-            }
+        >>> data = {
+        ...     "tbl": "foo",
+        ...     "col": "bar",
+        ... }
+        >>> Ref.model_validate(data).tbl
+        'foo'
     """
 
     tbl: str
     col: str
 
 
 class Fk(Const):
     """Foreign Key Model.
 
     Examples:
-        >>> data={
+        >>> data = {
         ...     "of": "foo",
         ...     "to": "bar",
         ...     "ref": {
         ...         "tbl": "ref_table",
         ...         "col": "ref_column"
         ...     }
         ... }
```

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/datasets/col.py` & `ddeutil_model-0.0.3/src/ddeutil/model/datasets/col.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/datasets/db.py` & `ddeutil_model-0.0.3/src/ddeutil/model/datasets/db.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/datasets/file.py` & `ddeutil_model-0.0.3/src/ddeutil/model/datasets/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,34 +7,35 @@
 
 from ..__base import BaseUpdatableModel
 from .col import Col
 
 
 class BaseFl(BaseUpdatableModel):
     name: str
+    encoding: str = "utf-8"
 
 
 class CsvFl(BaseFl):
     """Csv File Model"""
 
     type: Literal["csv"] = "csv"
     header: bool = True
     feature: list[Col]
     sep: str = ","
     comment: str = "#"
     skip_rows: int = 0
     skip_footer: int = 0
     quote_char: str = '"'
-    encoding: str = "utf-8"
 
 
 class JsonFl(BaseFl):
     """Json File Model"""
 
     type: Literal["json"] = "json"
+    nestest: int = -1
 
 
 class ParqFl(BaseFl):
     """Parquet File Model"""
 
     type: Literal["parquet"] = "parquet"
     compress: str = "gzip"
```

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/dtype.py` & `ddeutil_model-0.0.3/src/ddeutil/model/dtype.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/lineage.py` & `ddeutil_model-0.0.3/src/ddeutil/model/lineage.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,40 +12,51 @@
     Optional,
 )
 from zoneinfo import ZoneInfo
 
 from pydantic import BaseModel, Field
 from pydantic.functional_validators import field_validator, model_validator
 
-from .__base import BaseUpdatableModel
-from .__enums import Status
-from .settings import TSConf
+try:
+    from .__base import BaseUpdatableModel
+    from .__enums import Status
+    from .settings import TsConf
+except ImportError:
+    from __base import BaseUpdatableModel
+    from __enums import Status
+    from settings import TsConf
 
 
 def dt_now() -> datetime:
     return datetime.now(timezone.utc)
 
 
-class TS(BaseModel):
-    """Time Model"""
+class Ts(BaseModel):
+    """Timestamp Model
+
+    Examples:
+        >>> from datetime import datetime
+        >>> Ts(ts=datetime(2024, 1, 1, 5)).ts.tzinfo
+        zoneinfo.ZoneInfo(key='Asia/Bangkok')
+    """
 
     ts: Annotated[datetime, Field(default_factory=dt_now, alias="Timestamp")]
-    tz: Annotated[str, Field(alias="TimeZone")] = TSConf.tz
+    tz: Annotated[str, Field(alias="TimeZone")] = TsConf.tz
 
     @model_validator(mode="after")
     def __prepare_time(self):
         self.ts: datetime = self.ts.astimezone(ZoneInfo(self.tz))
         return self
 
     def now(self) -> datetime:
         """Return updated timestamp"""
         return datetime.now(tz=self.tz)
 
 
-class Tag(TS):
+class Tag(Ts):
     """Tag Model"""
 
     author: Annotated[
         Optional[str],
         Field(validate_default=True, description="Author"),
     ] = None
     desc: Annotated[
@@ -58,15 +69,15 @@
     ]
     vs: Annotated[
         Optional[date],
         Field(validate_default=True, description="Version of Tag"),
     ] = None
 
     @field_validator("author")
-    def __set_author(cls, value: Optional[str]):
+    def __set_author(cls, value: str | None):
         return value or "undefined"
 
     @field_validator("vs")
     def __set_version(cls, value: Optional[date]):
         """Pre initialize the `version` value that parsing from default"""
         return value if value else date(year=1990, month=1, day=1)
```

### Comparing `ddeutil_model-0.0.2/src/ddeutil/model/utils.py` & `ddeutil_model-0.0.3/src/ddeutil/model/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/src/ddeutil_model.egg-info/PKG-INFO` & `ddeutil_model-0.0.3/src/ddeutil_model.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Developer & Engineer Model Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil-model/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil-model/
 Keywords: data,model,utility,pipeline
 Classifier: Topic :: Utilities
@@ -23,14 +23,18 @@
 License-File: LICENSE
 Requires-Dist: ddeutil
 Requires-Dist: tzdata
 Requires-Dist: pydantic==2.7.1
 
 # Data Utility Package: *Model*
 
+[![test](https://github.com/ddeutils/ddeutil-model/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ddeutils/ddeutil-model/actions/workflows/tests.yml)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ddeutil-model?logo=pypi)](https://pypi.org/project/ddeutil-model/)
+[![size](https://img.shields.io/github/languages/code-size/ddeutils/ddeutil-model)](https://github.com/ddeutils/ddeutil-model)
+
 **Table of Contents**:
 
 - [Installation](#installation)
 - [Models](#models)
   - [Data Types](#data-types)
   - [Constraints](#constraints)
   - [Datasets](#datasets)
```

### Comparing `ddeutil_model-0.0.2/src/ddeutil_model.egg-info/SOURCES.txt` & `ddeutil_model-0.0.3/src/ddeutil_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_action.py` & `ddeutil_model-0.0.3/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_base.py` & `ddeutil_model-0.0.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_conn.py` & `ddeutil_model-0.0.3/tests/test_conn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,41 @@
 import ddeutil.model.conn as conn
 
 
+def test_conn_from_url():
+    t = conn.Conn.from_url(
+        url=(
+            "postgres+psycopg://demo:P%40ssw0rd@localhost/postgres"
+            "?echo=True&timeout=10"
+        )
+    )
+    assert t.port is None
+    assert "postgres+psycopg" == t.dialect
+    assert "postgres" == t.endpoint
+    assert "demo" == t.user
+    assert "P@ssw0rd" == t.pwd.get_secret_value()
+    assert "localhost" == t.host
+
+    t = conn.Conn.from_url(url="sqlite:///foo.db")
+
+    assert t.port is None
+    assert t.user is None
+    assert t.pwd is None
+    assert t.host is None
+    assert "foo.db" == t.endpoint
+
+    t = conn.Conn.from_url(url="sqlite:////absolute/path/to/foo.db")
+
+    assert "absolute/path/to/foo.db" == t.endpoint
+
+    t = conn.Conn.from_url(url=r"sqlite:///C:\path\to\foo.db")
+
+    assert "C:\\path\\to\\foo.db" == t.endpoint
+
+
 def test_db_conn_from_url():
     t = conn.DbConn.from_url(
         url=(
             "postgres+psycopg://demo:P%40ssw0rd@localhost:5432/db"
             "?echo=True&timeout=10"
         )
     )
```

### Comparing `ddeutil_model-0.0.2/tests/test_const.py` & `ddeutil_model-0.0.3/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_dataset_column.py` & `ddeutil_model-0.0.3/tests/test_dataset_column.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_dataset_schema.py` & `ddeutil_model-0.0.3/tests/test_dataset_schema.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_dataset_table.py` & `ddeutil_model-0.0.3/tests/test_dataset_table.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_dtype.py` & `ddeutil_model-0.0.3/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `ddeutil_model-0.0.2/tests/test_lineage.py` & `ddeutil_model-0.0.3/tests/test_lineage.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import ddeutil.model.lineage as lineages
 import ddeutil.model.settings as st
 
 
 @mock.patch("ddeutil.model.lineage.datetime", wraps=datetime.datetime)
 def test_ts_init(mock_datetime):
     mock_datetime.now.return_value = datetime.datetime(2023, 1, 1, 0, 0, 0)
-    t = lineages.TS()
+    t = lineages.Ts()
     assert t.model_dump(by_alias=False) == {
         "ts": datetime.datetime(2023, 1, 1, 0, 0, 0).astimezone(
-            tz=ZoneInfo(st.TSConf.tz)
+            tz=ZoneInfo(st.TsConf.tz)
         ),
         "tz": "Asia/Bangkok",
     }
 
 
 @mock.patch("ddeutil.model.lineage.date", wraps=datetime.date)
 @mock.patch("ddeutil.model.lineage.datetime", wraps=datetime.datetime)
@@ -26,15 +26,15 @@
     mock_datetime.now.return_value = datetime.datetime(2023, 1, 1, 0, 0, 0)
     t = lineages.Tag()
     assert t.model_dump(by_alias=False) == {
         "author": "undefined",
         "desc": None,
         "labels": [],
         "ts": datetime.datetime(2023, 1, 1, 0, 0, 0).astimezone(
-            tz=ZoneInfo(st.TSConf.tz)
+            tz=ZoneInfo(st.TsConf.tz)
         ),
         "vs": datetime.date(2023, 1, 1),
         "tz": "Asia/Bangkok",
     }
 
 
 def test_task_init():
```


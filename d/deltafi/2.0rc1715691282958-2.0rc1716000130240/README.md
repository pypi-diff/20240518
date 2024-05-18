# Comparing `tmp/deltafi-2.0rc1715691282958.tar.gz` & `tmp/deltafi-2.0rc1716000130240.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-2.0rc1715691282958.tar", max compression
+gzip compressed data, was "deltafi-2.0rc1716000130240.tar", max compression
```

## Comparing `deltafi-2.0rc1715691282958.tar` & `deltafi-2.0rc1716000130240.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      189 2023-08-18 19:46:59.247988 deltafi-2.0rc1715691282958/README.md
--rw-r--r--   0        0        0      709 2023-10-18 22:01:21.233230 deltafi-2.0rc1715691282958/deltafi/__init__.py
--rw-r--r--   0        0        0     5343 2024-05-09 17:57:35.270646 deltafi-2.0rc1715691282958/deltafi/action.py
--rw-r--r--   0        0        0     2847 2023-10-18 22:01:21.233230 deltafi-2.0rc1715691282958/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      913 2024-05-09 17:57:35.293647 deltafi-2.0rc1715691282958/deltafi/actiontype.py
--rw-r--r--   0        0        0    12112 2024-05-09 17:57:35.320649 deltafi-2.0rc1715691282958/deltafi/domain.py
--rw-r--r--   0        0        0      943 2024-05-09 17:57:35.330650 deltafi-2.0rc1715691282958/deltafi/exception.py
--rw-r--r--   0        0        0     1090 2023-11-15 21:51:57.337445 deltafi-2.0rc1715691282958/deltafi/genericmodel.py
--rw-r--r--   0        0        0     1656 2024-05-09 17:57:35.343650 deltafi-2.0rc1715691282958/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-08-18 19:46:59.249988 deltafi-2.0rc1715691282958/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-08-18 19:46:59.249988 deltafi-2.0rc1715691282958/deltafi/metric.py
--rw-r--r--   0        0        0    12422 2024-05-09 17:57:35.361652 deltafi-2.0rc1715691282958/deltafi/plugin.py
--rw-r--r--   0        0        0     8210 2024-05-09 17:57:35.385653 deltafi-2.0rc1715691282958/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-08-18 19:46:59.249988 deltafi-2.0rc1715691282958/deltafi/storage.py
--rw-r--r--   0        0        0      709 2023-10-18 22:01:21.234230 deltafi-2.0rc1715691282958/deltafi/test_kit/__init__.py
--rw-r--r--   0        0        0     1378 2023-10-18 22:01:21.235230 deltafi-2.0rc1715691282958/deltafi/test_kit/assertions.py
--rw-r--r--   0        0        0    12957 2024-05-13 20:31:46.468118 deltafi-2.0rc1715691282958/deltafi/test_kit/compare_helpers.py
--rw-r--r--   0        0        0      833 2023-10-18 22:01:21.235230 deltafi-2.0rc1715691282958/deltafi/test_kit/constants.py
--rw-r--r--   0        0        0     2090 2024-01-24 00:43:35.834381 deltafi-2.0rc1715691282958/deltafi/test_kit/domain.py
--rw-r--r--   0        0        0     1899 2024-01-17 20:15:36.113816 deltafi-2.0rc1715691282958/deltafi/test_kit/egress.py
--rw-r--r--   0        0        0     2587 2024-01-24 00:43:35.834381 deltafi-2.0rc1715691282958/deltafi/test_kit/enrich.py
--rw-r--r--   0        0        0    13033 2024-05-09 17:57:35.386653 deltafi-2.0rc1715691282958/deltafi/test_kit/framework.py
--rw-r--r--   0        0        0     4085 2024-05-09 17:57:35.387653 deltafi-2.0rc1715691282958/deltafi/test_kit/transform.py
--rw-r--r--   0        0        0     1933 2024-01-24 00:43:35.836381 deltafi-2.0rc1715691282958/deltafi/test_kit/validate.py
--rw-r--r--   0        0        0     1310 2024-05-14 12:55:12.823647 deltafi-2.0rc1715691282958/pyproject.toml
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1715691282958/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:34:58.932322 deltafi-2.0rc1716000130240/README.md
+-rw-r--r--   0        0        0      709 2023-09-08 11:24:47.608536 deltafi-2.0rc1716000130240/deltafi/__init__.py
+-rw-r--r--   0        0        0     5343 2024-05-13 15:09:25.516588 deltafi-2.0rc1716000130240/deltafi/action.py
+-rw-r--r--   0        0        0     2847 2023-10-13 13:53:29.360657 deltafi-2.0rc1716000130240/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      913 2024-05-13 15:09:25.517588 deltafi-2.0rc1716000130240/deltafi/actiontype.py
+-rw-r--r--   0        0        0    12112 2024-05-13 15:09:25.517588 deltafi-2.0rc1716000130240/deltafi/domain.py
+-rw-r--r--   0        0        0      943 2024-05-13 15:09:25.517588 deltafi-2.0rc1716000130240/deltafi/exception.py
+-rw-r--r--   0        0        0     1090 2023-11-16 03:01:54.189409 deltafi-2.0rc1716000130240/deltafi/genericmodel.py
+-rw-r--r--   0        0        0     1656 2024-05-13 15:09:25.517588 deltafi-2.0rc1716000130240/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:34:58.937322 deltafi-2.0rc1716000130240/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:34:58.938322 deltafi-2.0rc1716000130240/deltafi/metric.py
+-rw-r--r--   0        0        0    12422 2024-05-13 15:09:25.517588 deltafi-2.0rc1716000130240/deltafi/plugin.py
+-rw-r--r--   0        0        0     8212 2024-05-17 15:57:39.038425 deltafi-2.0rc1716000130240/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-17 20:43:32.061753 deltafi-2.0rc1716000130240/deltafi/storage.py
+-rw-r--r--   0        0        0      709 2023-09-08 11:24:47.609536 deltafi-2.0rc1716000130240/deltafi/test_kit/__init__.py
+-rw-r--r--   0        0        0     1378 2023-09-08 11:24:47.609536 deltafi-2.0rc1716000130240/deltafi/test_kit/assertions.py
+-rw-r--r--   0        0        0    12957 2024-05-14 19:35:36.023644 deltafi-2.0rc1716000130240/deltafi/test_kit/compare_helpers.py
+-rw-r--r--   0        0        0      833 2023-08-07 14:10:09.593662 deltafi-2.0rc1716000130240/deltafi/test_kit/constants.py
+-rw-r--r--   0        0        0     2090 2024-01-26 17:47:35.400662 deltafi-2.0rc1716000130240/deltafi/test_kit/domain.py
+-rw-r--r--   0        0        0     1899 2024-01-26 17:47:35.400662 deltafi-2.0rc1716000130240/deltafi/test_kit/egress.py
+-rw-r--r--   0        0        0     2587 2024-01-26 17:47:35.400662 deltafi-2.0rc1716000130240/deltafi/test_kit/enrich.py
+-rw-r--r--   0        0        0    13078 2024-05-16 22:09:04.691290 deltafi-2.0rc1716000130240/deltafi/test_kit/framework.py
+-rw-r--r--   0        0        0     4085 2024-05-13 15:09:25.518588 deltafi-2.0rc1716000130240/deltafi/test_kit/transform.py
+-rw-r--r--   0        0        0     1933 2024-01-26 17:47:35.408662 deltafi-2.0rc1716000130240/deltafi/test_kit/validate.py
+-rw-r--r--   0        0        0     1310 2024-05-18 02:42:41.721354 deltafi-2.0rc1716000130240/pyproject.toml
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1716000130240/PKG-INFO
```

### Comparing `deltafi-2.0rc1715691282958/deltafi/__init__.py` & `deltafi-2.0rc1716000130240/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/action.py` & `deltafi-2.0rc1716000130240/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/actioneventqueue.py` & `deltafi-2.0rc1716000130240/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/actiontype.py` & `deltafi-2.0rc1716000130240/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/domain.py` & `deltafi-2.0rc1716000130240/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/exception.py` & `deltafi-2.0rc1716000130240/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/genericmodel.py` & `deltafi-2.0rc1716000130240/deltafi/genericmodel.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/input.py` & `deltafi-2.0rc1716000130240/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/logger.py` & `deltafi-2.0rc1716000130240/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/metric.py` & `deltafi-2.0rc1716000130240/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/plugin.py` & `deltafi-2.0rc1716000130240/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/result.py` & `deltafi-2.0rc1716000130240/deltafi/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,27 +155,27 @@
 class IngressResult(Result):
     def __init__(self, context: Context):
         super().__init__('ingress', 'INGRESS', context)
         self.memo = None
         self.ingress_result_items = []
         self.execute_immediate = False
         self.status = IngressStatusEnum.HEALTHY
-        self.statusMessage = None
+        self.status_message = None
 
     def add_item(self, ingress_result_item: IngressResultItem):
         self.ingress_result_items.append(ingress_result_item)
         return self
 
     def response(self):
         return {
             'memo': self.memo,
             'executeImmediate': self.execute_immediate,
             'ingressItems': [ingress_result_item.response() for ingress_result_item in self.ingress_result_items],
             'status': self.status.value,
-            'statusMessage': self.statusMessage
+            'statusMessage': self.status_message
         }
 
 
 class TransformResult(Result):
     def __init__(self, context: Context):
         super().__init__('transform', 'TRANSFORM', context)
         self.content = []
```

### Comparing `deltafi-2.0rc1715691282958/deltafi/storage.py` & `deltafi-2.0rc1716000130240/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/__init__.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/assertions.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/assertions.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/compare_helpers.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/compare_helpers.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/constants.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/constants.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/domain.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/egress.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/egress.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/enrich.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/enrich.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/framework.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             self.content_name = content_name
         if content_type is None:
             self.content_type = IOContent.file_type(file_name)
         else:
             self.content_type = content_type
         self.offset = offset
         self.content_bytes = content_bytes
+        self.segment_uuid = uuid.uuid4()
 
     @classmethod
     def file_type(cls, name: str):
         if name.endswith(".json"):
             return "application/json"
         elif name.endswith(".xml"):
             return "application/xnl"
@@ -76,15 +77,15 @@
         self.content_type = ioc.content_type
         self.offset = ioc.offset
         if data is not None:
             self.data = data
         else:
             self.data = ioc.content_bytes
         self.segment = Segment.from_dict(
-            {"uuid": str(uuid.uuid4()), "offset": self.offset, "size": len(self.data), "did": did})
+            {"uuid": str(ioc.segment_uuid), "offset": self.offset, "size": len(self.data), "did": did})
 
 
 class InternalContentService:
     def __init__(self):
         self.loaded_content = {}
         self.outputs = {}
```

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/transform.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/transform.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/deltafi/test_kit/validate.py` & `deltafi-2.0rc1716000130240/deltafi/test_kit/validate.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1715691282958/pyproject.toml` & `deltafi-2.0rc1716000130240/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "2.0rc1715691282958"
+version = "2.0rc1716000130240"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-2.0rc1715691282958/PKG-INFO` & `deltafi-2.0rc1716000130240/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 2.0rc1715691282958
+Version: 2.0rc1716000130240
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```


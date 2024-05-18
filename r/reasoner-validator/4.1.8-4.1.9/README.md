# Comparing `tmp/reasoner_validator-4.1.8.tar.gz` & `tmp/reasoner_validator-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.8.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.9.tar", max compression
```

## Comparing `reasoner_validator-4.1.8.tar` & `reasoner_validator-4.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/LICENSE
--rw-r--r--   0        0        0    13727 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/README.md
--rw-r--r--   0        0        0      131 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/conf.py
--rw-r--r--   0        0        0    20564 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/index.rst
--rw-r--r--   0        0        0      795 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/make.bat
--rw-r--r--   0        0        0      136 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    43520 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2341 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 03:38:50.621482 reasoner_validator-4.1.8/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    96715 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    47438 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/github.py
--rw-r--r--   0        0        0     3995 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/message.py
--rw-r--r--   0        0        0    47007 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    38176 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/conftest.py
--rw-r--r--   0        0        0   151994 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    49059 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_semver.py
--rw-r--r--   0        0        0     2351 2024-05-17 03:38:50.625482 reasoner_validator-4.1.8/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36764 2024-05-17 03:38:50.629482 reasoner_validator-4.1.8/tests/test_validate.py
--rw-r--r--   0        0        0    30423 2024-05-17 03:38:50.629482 reasoner_validator-4.1.8/tests/test_validation_report.py
--rw-r--r--   0        0        0     3421 2024-05-17 03:38:50.629482 reasoner_validator-4.1.8/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/README.md
+-rw-r--r--   0        0        0      131 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    43520 2024-05-17 18:11:08.506573 reasoner_validator-4.1.9/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2341 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    97110 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    47438 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3995 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/message.py
+-rw-r--r--   0        0        0    47007 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    38176 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 18:11:08.510573 reasoner_validator-4.1.9/tests/conftest.py
+-rw-r--r--   0        0        0   151994 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    49059 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_semver.py
+-rw-r--r--   0        0        0     2351 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36764 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_validate.py
+-rw-r--r--   0        0        0    30423 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3421 2024-05-17 18:11:08.514573 reasoner_validator-4.1.9/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.9/PKG-INFO
```

### Comparing `reasoner_validator-4.1.8/LICENSE` & `reasoner_validator-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/README.md` & `reasoner_validator-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/docs/Makefile` & `reasoner_validator-4.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/docs/conf.py` & `reasoner_validator-4.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/docs/index.rst` & `reasoner_validator-4.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/docs/make.bat` & `reasoner_validator-4.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.9/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/pyproject.toml` & `reasoner_validator-4.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.8"
+version = "4.1.9"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.1.8/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.9/reasoner_validator/biolink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -781,16 +781,17 @@
             # also track primary_knowledge_source attribute cardinality now
             found_primary_knowledge_source: List[str] = list()
 
             # Track presence of 'knowledge_level' and 'agent_type' attributes
             found_knowledge_level = False
             found_agent_type = False
 
-            # Track presence of 'support_graph' for some predicates (e.g. 'treats')
-            found_support_graph = False
+            # TODO: Defer tracking of the presence of 'biolink:support_graphs'
+            #       for specified predicates like 'treats' or its descendants
+            # found_support_graphs = False
 
             for attribute in attributes:
 
                 # Validate attribute_type_id
                 if 'attribute_type_id' not in attribute:
                     self.report(
                         code="error.knowledge_graph.edge.attribute.type_id.missing",
@@ -922,17 +923,18 @@
                                                                         and infores == ara_source:
                                                                     found_ara_knowledge_source = True
                                                                 elif kp_source and \
                                                                         attribute_type_id == kp_source_type and \
                                                                         infores == kp_source:
                                                                     found_kp_knowledge_source = True
 
-                                                # Check for 'support_graph'
-                                                if attribute_type_id == "biolink:support_graph":
-                                                    found_support_graph = False
+                                                # TODO: Defer tracking of the presence of 'biolink:support_graphs'
+                                                #       for specified predicates like 'treats' or its descendants
+                                                # if attribute_type_id == "biolink:support_graphs":
+                                                #     found_support_graphs = False
 
                                                 # We expect at this point that, if 'attribute_type_id' is a
                                                 # 'knowledge_level' or 'agent_type', then the value is a scalar
                                                 value = value[0]
 
                                                 # We won't likely care if 'knowledge_level' or 'agent_type'
                                                 # show up in graphs compliant with Biolink earlier than 4.2.0,
@@ -1004,21 +1006,22 @@
                         )
                     else:
                         self.report(
                             code="warning.knowledge_graph.edge.agent_type.missing",
                             identifier=edge_id
                         )
 
-                #
-                predicate = edge['predicate'] if 'predicate' in edge else None
-                if self.is_treats(predicate) and not found_support_graph:
-                    self.report(
-                        code="warning.knowledge_graph.edge.treats.support_graph.missing",
-                        identifier=edge_id
-                    )
+                # TODO: Defer tracking of the presence of 'biolink:support_graphs'
+                #       for specified predicates like 'treats' or its descendants
+                # predicate = edge['predicate'] if 'predicate' in edge else None
+                # if self.is_treats(predicate) and not found_support_graphs:
+                #     self.report(
+                #         code="warning.knowledge_graph.edge.treats.support_graph.missing",
+                #         identifier=edge_id
+                #     )
 
         return source_trail  # may be 'None' if the required attributes are missing
 
     def validate_attribute_constraints(self, edge_id: str, edge: Dict):
         """
         Validate Query Edge Attributes.
```

### Comparing `reasoner_validator-4.1.8/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.9/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/github.py` & `reasoner_validator-4.1.9/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/message.py` & `reasoner_validator-4.1.9/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/report.py` & `reasoner_validator-4.1.9/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.9/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.9/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.9/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.9/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/validator.py` & `reasoner_validator-4.1.9/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/versioning.py` & `reasoner_validator-4.1.9/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.9/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/__init__.py` & `reasoner_validator-4.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.9/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.9/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_response_validator.py` & `reasoner_validator-4.1.9/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_semver.py` & `reasoner_validator-4.1.9/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.9/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_validate.py` & `reasoner_validator-4.1.9/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_validation_report.py` & `reasoner_validator-4.1.9/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/tests/test_workflows.py` & `reasoner_validator-4.1.9/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.8/PKG-INFO` & `reasoner_validator-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.8
+Version: 4.1.9
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```


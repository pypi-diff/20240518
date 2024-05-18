# Comparing `tmp/graph_validation_test_runners-0.1.2.tar.gz` & `tmp/graph_validation_test_runners-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_validation_test_runners-0.1.2.tar", max compression
+gzip compressed data, was "graph_validation_test_runners-0.1.3.tar", max compression
```

## Comparing `graph_validation_test_runners-0.1.2.tar` & `graph_validation_test_runners-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,30 @@
--rw-r--r--   0        0        0     1070 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/LICENSE
--rw-r--r--   0        0        0    11042 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/README.md
--rw-r--r--   0        0        0    30316 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/translator/__init__.py
--rw-r--r--   0        0        0    36673 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/translator/registry/__init__.py
--rw-r--r--   0        0        0    10817 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/translator/trapi/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/utils/__init__.py
--rw-r--r--   0        0        0      722 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/utils/asyncio.py
--rw-r--r--   0        0        0      113 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/utils/constants.py
--rw-r--r--   0        0        0      886 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/utils/http.py
--rw-r--r--   0        0        0     4268 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/utils/ontology_kp.py
--rw-r--r--   0        0        0    19691 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/graph_validation_tests/utils/unit_test_templates.py
--rw-r--r--   0        0        0     7839 2024-05-10 20:29:36.641128 graph_validation_test_runners-0.1.2/one_hop_test_runner/__init__.py
--rw-r--r--   0        0        0     2610 2024-05-10 20:29:48.869178 graph_validation_test_runners-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4526 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/standards_validation_test_runner/__init__.py
--rw-r--r--   0        0        0     1933 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0    18172 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0     4960 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/__init__.py
--rw-r--r--   0        0        0     4776 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/test_graph_validation_test.py
--rw-r--r--   0        0        0     5765 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/test_unit_test_templates.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/biolink/__init__.py
--rw-r--r--   0        0        0     1066 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/biolink/test_ontology_kp.py
--rw-r--r--   0        0        0    18172 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/trapi/__init__.py
--rw-r--r--   0        0        0     5028 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/one_hop_test_runner/__init__.py
--rw-r--r--   0        0        0     3770 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/one_hop_test_runner/test_one_hop_test.py
--rw-r--r--   0        0        0       70 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/scripts/one_hop_test.cmd
--rw-r--r--   0        0        0        0 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/standards_validation_test_runner/__init__.py
--rw-r--r--   0        0        0     2573 2024-05-10 20:29:36.645128 graph_validation_test_runners-0.1.2/tests/standards_validation_test_runner/test_standards_validation_test.py
--rw-r--r--   0        0        0    12921 1970-01-01 00:00:00.000000 graph_validation_test_runners-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/LICENSE
+-rw-r--r--   0        0        0    11042 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/README.md
+-rw-r--r--   0        0        0    29260 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/translator/__init__.py
+-rw-r--r--   0        0        0    36789 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/translator/registry/__init__.py
+-rw-r--r--   0        0        0    11087 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/translator/trapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/utils/__init__.py
+-rw-r--r--   0        0        0      722 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/utils/asyncio.py
+-rw-r--r--   0        0        0      113 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/utils/constants.py
+-rw-r--r--   0        0        0    19683 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/graph_validation_tests/utils/unit_test_templates.py
+-rw-r--r--   0        0        0     7839 2024-05-18 09:22:32.477492 graph_validation_test_runners-0.1.3/one_hop_test_runner/__init__.py
+-rw-r--r--   0        0        0     2610 2024-05-18 09:22:47.221534 graph_validation_test_runners-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4526 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/standards_validation_test_runner/__init__.py
+-rw-r--r--   0        0        0     1933 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    18172 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0     2848 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/__init__.py
+-rw-r--r--   0        0        0     7096 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/test_graph_validation_test.py
+-rw-r--r--   0        0        0     5765 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/test_unit_test_templates.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/translator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/translator/biolink/__init__.py
+-rw-r--r--   0        0        0    18172 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/translator/trapi/__init__.py
+-rw-r--r--   0        0        0     2916 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/one_hop_test_runner/__init__.py
+-rw-r--r--   0        0        0     4320 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/one_hop_test_runner/test_one_hop_test.py
+-rw-r--r--   0        0        0       70 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/scripts/one_hop_test.cmd
+-rw-r--r--   0        0        0        0 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/standards_validation_test_runner/__init__.py
+-rw-r--r--   0        0        0     2894 2024-05-18 09:22:32.481492 graph_validation_test_runners-0.1.3/tests/standards_validation_test_runner/test_standards_validation_test.py
+-rw-r--r--   0        0        0    12921 1970-01-01 00:00:00.000000 graph_validation_test_runners-0.1.3/PKG-INFO
```

### Comparing `graph_validation_test_runners-0.1.2/LICENSE` & `graph_validation_test_runners-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/README.md` & `graph_validation_test_runners-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/graph_validation_tests/__init__.py` & `graph_validation_test_runners-0.1.3/graph_validation_tests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """
 Abstract base class for the GraphValidation TestRunners
 """
 from typing import Dict, List, Optional, Tuple
 
 from argparse import ArgumentParser
 
+from reasoner_validator.versioning import get_latest_version
 from reasoner_validator.biolink import BiolinkValidator
 from reasoner_validator.validator import TRAPIResponseValidator
 from reasoner_validator.message import MESSAGES_BY_TARGET, MESSAGE_CATALOG, MESSAGES_BY_TEST
 from translator_testing_model.datamodel.pydanticmodel import TestAsset, TestCaseResultEnum
 
 from graph_validation_tests.translator.registry import (
     get_the_registry_data,
     extract_component_test_metadata_from_registry
 )
 from graph_validation_tests.translator.trapi import get_available_components
 from graph_validation_tests.utils.asyncio import gather
 
+from bmt import Toolkit
+
 import logging
 logger = logging.getLogger(__name__)
 
+# as long as TRAPI has major version == "1", we should be OK here
+default_trapi_release: str = get_latest_version("1")
+default_biolink_model_version: str = Toolkit().get_model_version()
+
 
 class TestCaseRun(TRAPIResponseValidator):
     """
     TestCaseRun is a wrapper for BiolinkValidator, used to aggregate
     validation messages from the GraphValidationTest processing of a specific
     TestCase, derived from the TestAsset - bound to the 'test_run' - which is
     based on a TRAPI query against the test_run bound 'target' endpoint. Results
@@ -268,14 +275,15 @@
         raise NotImplementedError("Abstract method, implement in subclass!")
 
     @staticmethod
     async def run_test_cases(test_cases: List[TestCaseRun]):
         # TODO: unsure if one needs to limit concurrent requests here...
         await gather([test_case.run_test_case() for test_case in test_cases])  # , limit=num_concurrent_requests)
 
+    MESSAGE_PRECEDENCE = ("critical", "error", "warning", "skipped", "info")
     FAILURE_MODES = ("error", "critical")
 
     def compute_status(self, tcr: TestCaseRun) -> Tuple[str, TestCaseResultEnum, Dict]:
         """
         Method to construct components for a test case result based on the failure mode
         assessment of non-empty validation messages (which are also returned).
 
@@ -289,20 +297,24 @@
         messages_by_target: MESSAGES_BY_TARGET = tcr.get_all_messages()
         if target in messages_by_target:
             messages_by_test: MESSAGES_BY_TEST = messages_by_target[target]
             if test in messages_by_test:
                 message_catalog: MESSAGE_CATALOG = messages_by_test[test]
                 mtype: str
                 messages: Dict
-                non_empty_messages: MESSAGE_CATALOG = {
-                    mtype: messages for mtype, messages in message_catalog.items() if message_catalog[mtype]
-                }
+                # Load non-empty messages in order of message precedence
+                non_empty_messages: MESSAGE_CATALOG = dict()
+                for mtype in self.MESSAGE_PRECEDENCE:
+                    if mtype in message_catalog and message_catalog[mtype]:
+                        non_empty_messages[mtype] = message_catalog[mtype]
                 # TODO: this first iteration in which FAILURE_MODES are
-                #       immutable (not sensitive to TestRunner parameters)
-                if not non_empty_messages or not any([mtype in non_empty_messages for mtype in self.FAILURE_MODES]):
+                #       immutable (not sensitive to TestRunner parameters);
+                #       Maybe we need to treat "SKIPPED" tests differently here(?)
+                if not non_empty_messages or \
+                        not any([mtype in non_empty_messages for mtype in self.FAILURE_MODES]):
                     return target, TestCaseResultEnum.PASSED, non_empty_messages
                 else:
                     return target, TestCaseResultEnum.FAILED, non_empty_messages
         # TODO: seems sensible to assumed that if the target or test are
         #       missing in test results, then the test was skipped?
         return target, TestCaseResultEnum.SKIPPED, {}
 
@@ -530,70 +542,28 @@
                 environment=environment,
                 trapi_generators=trapi_generators,
                 trapi_version=trapi_version,
                 biolink_version=biolink_version,
                 runner_settings=runner_settings
             ) for target in components
         ]
-        #
-        # TODO: the following comment is plagiarized from 3rd party TestRunner comments simply as
-        #       a short term source of inspiration for the design of results from this TestRunner
-        # The ARS_test_Runner with the following command:
-        #
-        #       ARS_Test_Runner
-        #           --env 'ci'
-        #           --query_type 'treats_creative'
-        #           --expected_output '["TopAnswer","TopAnswer"]'
-        #           --input_curie 'MONDO:0005301'
-        #           --output_curie  '["PUBCHEM.COMPOUND:107970","UNII:3JB47N2Q2P"]'
-        #
-        # gives a Python dictionary report (serialized to JSON) similar as follows:
-        #
-        # {
-        #     "pks": {
-        #         "parent_pk": "e29c5051-d8d7-4e82-a1a1-b3cc9b8c9657",
-        #         "merged_pk": "56e3d5ac-66b4-4560-9f56-7a4d117e8003",
-        #         "aragorn": "14953570-7451-4d1b-a817-fc9e7879b477",
-        #         "arax": "8c88ead6-6cbf-4c9a-9570-ca76392ddb7a",
-        #         "unsecret": "bd084e27-2a0e-4df4-843c-417bfac6f8c7",
-        #         "bte": "d28a4146-9486-4e98-973d-8cdd33270595",
-        #         "improving": "d8d3c905-ec07-491f-a078-7ef0f489a409"
-        #     },
-        #     "results": [
-        #         {
-        #             "PUBCHEM.COMPOUND:107970": {
-        #                 "aragorn": "Fail",
-        #                 "arax": "Pass",
-        #                 "unsecret": "Fail",
-        #                 "bte": "Pass",
-        #                 "improving": "Pass",
-        #                 "ars": "Pass"
-        #             }
-        #         },
-        #         {
-        #             "UNII:3JB47N2Q2P": {
-        #                 "aragorn": "Fail",
-        #                 "arax": "Pass",
-        #                 "unsecret": "Fail",
-        #                 "bte": "Pass",
-        #                 "improving": "Pass",
-        #                 "ars": "Pass"
-        #             }
-        #         }
-        #     ]
-        # }
         results = {
             "pks": dict(),
             "results": dict()
         }
         for tr in test_runs:
             target: str = tr.default_target
             test_run_id: str = tr.get_run_id()
             results["pks"].update({target: test_run_id})
-            results["results"].update(await tr.process_test_run(**kwargs))
+            result: Dict = await tr.process_test_run(**kwargs)
+            for test_case_id, result in result.items():
+                if test_case_id not in results["results"]:
+                    results["results"][test_case_id] = dict()
+
+                results["results"][test_case_id].update(result)
 
         return results
 
 
 def get_parameters(tool_name: str):
     """Parse CLI args."""
 
@@ -672,24 +642,25 @@
         required=True,
         help="Statement object concept Biolink category (CURIE)",
     )
 
     parser.add_argument(
         "--trapi_version",
         type=str,
-        help="TRAPI version expected for knowledge graph access (Default: use latest TRAPI community release)",
-        default=None
+        help="TRAPI version expected for knowledge graph access" +
+             f" (Default: use latest TRAPI community release: '{default_trapi_release}')",
+        default=default_trapi_release
     )
 
     parser.add_argument(
         "--biolink_version",
         type=str,
         help="Biolink Model version expected for knowledge graph access " +
-             "(Default: use current default release of the Biolink Model Toolkit)",
-        default=None
+             f"(Default: use current default release of the Biolink Model Toolkit: '{default_biolink_model_version}')",
+        default=default_biolink_model_version
     )
 
     parser.add_argument(
         "--runner_settings",
         nargs='+',
         help="Scalar settings for the TestRunner, e.g. 'inferred'",
         default=None
```

### Comparing `graph_validation_test_runners-0.1.2/graph_validation_tests/translator/registry/__init__.py` & `graph_validation_test_runners-0.1.3/graph_validation_tests/translator/registry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,25 +244,26 @@
     testing_endpoints: List[str] = ["meta_knowledge_graph", "asyncquery_status/abcdefg"]
     for endpoint in testing_endpoints:
         test_url: str = f"{url}/{endpoint}"
         try:
             request = requests.get(test_url)
             if request.status_code == 200:
                 # Success! given url is deemed a 'live' TRAPI endpoint
-                # TODO: since we are accessing this endpoint now, perhaps we can
+                # TODO: since we are accessing this endpoint now, perhaps can we
                 #       harvest some of its metadata here, for validation purposes?
                 data: Optional[Dict] = request.json()
+                logger.info(f"live_trapi_endpoint(): TRAPI endpoint '{test_url}' successfully accessed!")
                 return data
             else:
                 logger.warning(
                     f"live_trapi_endpoint(): TRAPI endpoint '{test_url}' is inaccessible? " +
                     f"Status code: {request.status_code}?"
                 )
         except RequestException as re:
-            logger.warning(f"live_trapi_endpoint(): requests.get() exception {str(re)}?")
+            logger.warning(f"live_trapi_endpoint(): requests.get({test_url}) exception {str(re)}?")
     return None
 
 
 def capture_kg_metadata(endpoint: str, data: Dict):
     """
     Parses and caches useful metadata from a specified TRAPI endpoint.
     :param endpoint: str, TRAPI endpoint
```

### Comparing `graph_validation_test_runners-0.1.2/graph_validation_tests/translator/trapi/__init__.py` & `graph_validation_test_runners-0.1.3/graph_validation_tests/translator/trapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -219,53 +219,49 @@
                                             (default: None == 'ars')
     :param environment: Optional[str]: target Translator execution environment of the component to be accessed;
                                               One of ['dev', 'ci', 'test', 'prod'] (default: None == 'ci')
     :param target_trapi_version: Optional[str], target TRAPI version (default: latest public release)
     :param target_biolink_version: Optional[str], target Biolink Model version (default: Biolink toolkit release)
     :return: Optional[str], environment-specific endpoint for component to be queried. None if not available.
     """
+    endpoint: Optional[str] = None
     if not component:
         component = 'ars'
 
     if not environment:
         environment = 'ci'
 
-    elif environment not in DEPLOYMENT_TYPE_MAP.keys():
+    if environment not in DEPLOYMENT_TYPE_MAP.keys():
         logger.error(
             f"resolve_component_endpoint(): unexpected environment type: '{environment}', Cannot resolve endpoint!"
         )
-        return None
-
-    if component == 'ars':
+    elif component == 'ars':
         ars_env: str = ars_env_spec[environment]
         # TODO: how do I check if the given ARS service is online here?
         return f"https://{ars_env}.transltr.io/ars/api/"
-
     else:
-        endpoint: Optional[str] = None
         err_msg: str = \
-            f"Could not resolve endpoint of component '{component}' " + \
+            f"trapi::resolve_component_endpoint() - Could not resolve endpoint of component '{component}' " + \
             f"within specified environment '{environment}'?"
         try:
             registry_data: Dict = get_the_registry_data()
             endpoint: Optional[str] = \
                 get_component_endpoint_from_registry(
                     registry_data,
                     infores_id=get_component_infores_object_id(component),
                     environment=environment,
                     target_trapi_version=target_trapi_version,
                     target_biolink_version=target_biolink_version
                 )
         except AssertionError as ae:
-            err_msg = f"Exception occurred while resolving: {str(ae)}"
-
+            err_msg += f" Exception occurred while resolving: {str(ae)}"
         if not endpoint:
             logger.error(err_msg)
 
-        return endpoint
+    return endpoint
 
 
 async def run_trapi_query(
         trapi_request: Dict,
         component: str,
         environment: str,
         target_trapi_version: Optional[str],
@@ -279,25 +275,30 @@
                           'ars', ARA acronym (e.g. 'arax') or KP acronym (e.g. 'molepro')
     :param environment: Optional[str] = None, Target Translator execution environment for the test,
                                               one of 'dev', 'ci', 'test' or 'prod' (default: 'ci')
     :param target_trapi_version: Optional[str], target TRAPI version (default: latest public release)
     :param target_biolink_version: Optional[str], target Biolink Model version (default: Biolink toolkit release)
     :return:  Dict, TRAPI response JSON, as a Python data structure.
     """
+    trapi_response: Optional[Dict] = None
     endpoint: str = resolve_component_endpoint(
         component=component,
         environment=environment,
         target_trapi_version=target_trapi_version,
         target_biolink_version=target_biolink_version
     )
-    if not endpoint:
-        return None
-
-    if component == 'ars':
-        # TODO: make the (modified) TRAPI query to the ARS
-        raise NotImplementedError("Implement ARS TRAPI query processing!")
+    if endpoint:
+        if component == 'ars':
+            logger.error(
+                "trapi::run_trapi_query() - GraphValidationTest does not yet support ARS TRAPI query processing!"
+            )
+        else:
+            # Make the TRAPI call to the TestCase targeted ARS, KP or
+            # ARA resource, using the case-documented input test edge
+            trapi_response = await call_trapi(endpoint, trapi_request)
     else:
-        # Make the TRAPI call to the TestCase targeted ARS, KP or
-        # ARA resource, using the case-documented input test edge
-        trapi_response = await call_trapi(endpoint, trapi_request)
+        logger.error(
+            "trapi::run_trapi_query() - GraphValidationTest could not resolve endpoint " +
+            f"for component {component} in environment {environment}!"
+        )
 
     return trapi_response
```

### Comparing `graph_validation_test_runners-0.1.2/graph_validation_tests/utils/asyncio.py` & `graph_validation_test_runners-0.1.3/graph_validation_tests/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/graph_validation_tests/utils/unit_test_templates.py` & `graph_validation_test_runners-0.1.3/graph_validation_tests/utils/unit_test_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Set, Dict, List, Tuple, Optional
 from copy import deepcopy
 from dataclasses import asdict
 from functools import wraps
 
 from bmt import utils
 from reasoner_validator.biolink import get_biolink_model_toolkit, BMTWrapper
+from reasoner_validator.biolink.ontology import get_parent_concept
 from translator_testing_model.datamodel.pydanticmodel import TestCase
 
-from graph_validation_tests.utils.ontology_kp import get_parent_concept
-
 
 def create_one_hop_message(edge, look_up_subject: bool = False) -> Tuple[Optional[Dict], str]:
     """
     Given a complete edge, create a valid TRAPI message for "one hop" querying for the edge.
 
     If the look_up_subject is False (default) then the object id is not included, (lookup object
     by subject) and if the look_up_subject is True, then the subject id is not included (look up
@@ -234,15 +233,15 @@
     context: str = f"inverse_by_new_subject|predicate '{str(request['predicate_id'])}'"
 
     validator: BMTWrapper = BMTWrapper(biolink_version=request['biolink_version'])
     inverse_predicate = validator.get_inverse_predicate(predicate)
 
     # Not everything has an inverse (it should, and it will, but it doesn't right now)
     if inverse_predicate is None:
-        reason: str = "is an unknown or has no inverse?"
+        reason: str = "is unknown or has no inverse?"
         return None, context, reason
 
     # probably don't need to worry here but just-in-case
     # only work off a copy of the original request...
     transformed_request = request.copy()
     transformed_request.update({
         "subject_category": request['object_category'],
@@ -463,8 +462,8 @@
                f"Acceptable values are: {','.join(get_unit_test_list())}"
         return tuple(test.test_runner_settings)
     if test.test_case_objective == "StandardsValidationTest":
         return "by_subject", "by_object"
     elif test.test_case_objective == "OneHopTest":
         return tuple(get_unit_test_list())
     else:
-        raise NotImplementedError(f"Unexpected test_case_objective: {test.case_objective}?")
+        raise NotImplementedError(f"Unexpected test_case_objective: {test.case_objective}?")
```

### Comparing `graph_validation_test_runners-0.1.2/one_hop_test_runner/__init__.py` & `graph_validation_test_runners-0.1.3/one_hop_test_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/pyproject.toml` & `graph_validation_test_runners-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graph-validation-test-runners"
-version = "0.1.2"
+version = "0.1.3"
 description = "Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Chris Bizon <bizon.renci.org>",
     "Tim Putnam <tim@tislab>"
 ]
 maintainers = ["Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
@@ -50,15 +50,15 @@
 deepdiff = "^6.7.1"
 fastapi = "*"
 httpx = "^0.27.0"
 tqdm = "^4.66.2"
 requests = "^2.31.0"
 matplotlib = "^3.8.3"
 
-reasoner-validator = "^4.1.6"
+reasoner-validator = "^4.2.0"
 translator-testing-model = "^0.3.1"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "^69.5.1"
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.23.3"
```

### Comparing `graph_validation_test_runners-0.1.2/standards_validation_test_runner/__init__.py` & `graph_validation_test_runners-0.1.3/standards_validation_test_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/tests/__init__.py` & `graph_validation_test_runners-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/tests/graph_validation_test/translator/test_translator_smartapi_registry.py` & `graph_validation_test_runners-0.1.3/tests/graph_validation_test/translator/test_translator_smartapi_registry.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/tests/graph_validation_test/translator/trapi/test_trapi.py` & `graph_validation_test_runners-0.1.3/tests/one_hop_test_runner/test_one_hop_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,159 +1,168 @@
 """
-Unit tests of the low level TRAPI (ARS, KP & ARA) calling subsystem.
+Unit tests for One Hop Test code validation
 """
-from typing import Optional
+from sys import stdout, stderr
+from typing import List, Dict
+from json import dump
+import subprocess
 import pytest
 
-from graph_validation_tests.translator.trapi import (
-    get_component_infores_object_id,
-    resolve_component_endpoint
+from graph_validation_tests.utils.unit_test_templates import (
+    by_subject,
+    inverse_by_new_subject,
+    by_object,
+    raise_subject_entity,
+    raise_object_entity,
+    raise_object_by_subject,
+    raise_predicate_by_subject
+)
+from one_hop_test_runner import (
+    OneHopTest,
+    run_one_hop_tests
+)
+from tests import (
+    SCRIPTS_DIR,
+    SAMPLE_MOLEPRO_INPUT_DATA,
+    SAMPLE_ARAX_INPUT_DATA,
+    SAMPLE_ARAGORN_INPUT_DATA
 )
-from graph_validation_tests.utils.http import post_query
-from graph_validation_tests.utils.ontology_kp import (
-    ONTOLOGY_KP_TRAPI_SERVER,
-    NODE_NORMALIZER_SERVER
-)
-
-pytest_plugins = ('pytest_asyncio',)
 
 
-@pytest.mark.parametrize(
-    "component,infores",
-    [
-        ("arax", "arax"),
-        ("aragorn", "aragorn"),
-        ("bte", "biothings-explorer"),
-        ("improving", "improving-agent"),
-        ("molepro", "molepro")
+@pytest.mark.asyncio
+async def test_one_hop_test():
+    trapi_generators = [
+        by_subject,
+        inverse_by_new_subject,
+        by_object,
+        raise_subject_entity,
+        raise_object_entity,
+        raise_object_by_subject,
+        raise_predicate_by_subject
     ]
-)
-def test_get_get_component_infores_object_id(component: str, infores: str):
-    assert get_component_infores_object_id(component=component) == infores
+    results: Dict = await OneHopTest.run_tests(
+        **SAMPLE_MOLEPRO_INPUT_DATA,
+        trapi_generators=trapi_generators,
+        environment="ci",
+        components=["aragorn", "molepro"]
+    )
+    dump(results, stderr, indent=4)
 
 
-@pytest.mark.skip(
-    reason="These tests often work fine with fresh data, " +
-           "but fail later due to changes in online resources"
-)
-@pytest.mark.parametrize(
-    "component,environment,result",
-    [
-        (None, None, f"https://ars.ci.transltr.io/ars/api/"),
-        ("ars", None, f"https://ars.ci.transltr.io/ars/api/"),
-        ("ars", "non-environment", None),
-        ("ars", "test", f"https://ars.test.transltr.io/ars/api/"),
-        ("arax", "dev", "https://arax.ncats.io/beta/api/arax/v1.4"),
-        # ("aragorn", "prod", "https://aragorn.transltr.io/aragorn"),
-        ("bte", "test", "https://bte.test.transltr.io/v1"),
-        # ("improving", "test", "https://ia.test.transltr.io/api/v1.4/"),
-        ("molepro", "ci", "https://molepro-trapi.ci.transltr.io/molepro/trapi/v1.5"),
-        ("foobar", "ci", None),
-        ("arax", "non-environment", None),
+# ARS tests not yet supported so yes... results will
+# always be empty, with a logger message to inform why
+@pytest.mark.asyncio
+async def test_one_hop_test_of_ars():
+    trapi_generators = [
+        by_subject,
+        inverse_by_new_subject,
+        by_object,
+        raise_subject_entity,
+        raise_object_entity,
+        raise_object_by_subject,
+        raise_predicate_by_subject
     ]
-)
-def test_resolve_component_endpoint(
-        component: Optional[str],
-        environment: Optional[str],
-        result: Optional[str]
-):
-    endpoint: Optional[str] = \
-        resolve_component_endpoint(
-            component=component,
-            environment=environment,
-            target_trapi_version=None,
-            target_biolink_version=None
-        )
-    assert endpoint == result
+    results: Dict = await OneHopTest.run_tests(
+        **SAMPLE_MOLEPRO_INPUT_DATA,
+        trapi_generators=trapi_generators,
+        environment="ci"
+    )
+    assert not results
 
 
 @pytest.mark.parametrize(
-    "curie,category,result",
+    "data,environment,component,expected_result",
     [
-        (   # Query 0 - chemical compounds are NOT in ontology hierarchy
-            "CHEMBL.COMPOUND:CHEMBL2333026",
-            "biolink:SmallMolecule",
+        (
+            SAMPLE_MOLEPRO_INPUT_DATA,
+            "ci",
+            "molepro",
             None
         ),
-        (   # Query 1 - MONDO disease terms are in an ontology term hierarchy
-            "MONDO:0011027",
-            "biolink:Disease",
-            "MONDO:0015967"
+        (
+            SAMPLE_ARAX_INPUT_DATA,
+            "ci",
+            "arax",
+            None
         )
     ]
 )
 @pytest.mark.asyncio
-async def test_post_query_to_ontology_kp(curie: str, category: str, result: Optional[str]):
-    query = {
-        "message": {
-            "query_graph": {
-                "nodes": {
-                    "a": {
-                        "ids": [curie]
-                    },
-                    "b": {
-                        "categories": [category]
-                    }
-                },
-                "edges": {
-                    "ab": {
-                        "subject": "a",
-                        "object": "b",
-                        "predicates": ["biolink:subclass_of"]
-                    }
-                }
-            }
-        }
-    }
-    response = post_query(url=ONTOLOGY_KP_TRAPI_SERVER, query=query, server="Post Ontology KP Query")
-    assert response
+async def test_run_one_hop_tests(
+        data: Dict,
+        environment: str,
+        component: str,
+        expected_result
+):
+    results: Dict = await run_one_hop_tests(
+        **data,
+        environment=environment,
+        components=[component]
+    )
+    assert results
+    dump(results, stderr, indent=4)
 
 
 @pytest.mark.parametrize(
-    "curie,category",
+    "data,environment,components,expected_result",
     [
-        # Query 0 - HGNC id
-        ("HGNC:12791", "biolink:Gene"),
-
-        # Query 1 - MONDO term
-        ("MONDO:0011027", "biolink:Disease"),
-
-        # Query 2 - HP term
-        ("HP:0040068", "biolink:PhenotypicFeature")
+        (   # Query 0 - MolePro test
+            SAMPLE_MOLEPRO_INPUT_DATA,
+            "ci",
+            ["molepro"],
+            None
+        ),
+        (   # Query 1 - ARAX test
+            SAMPLE_ARAX_INPUT_DATA,
+            "ci",
+            ["arax"],
+            None
+        ),
+        (   # Query 2 - Aragorn test
+            SAMPLE_ARAGORN_INPUT_DATA,
+            "ci",
+            ["aragorn"],
+            None
+        ),
+        (   # Query 3 - Combined ARAX and MolePro test
+            SAMPLE_MOLEPRO_INPUT_DATA,
+            "ci",
+            ["molepro", "arax", "aragorn"],
+            None
+        )
     ]
 )
 @pytest.mark.asyncio
-async def test_post_query_to_node_normalization(curie: str, category: str):
-    j = {'curies': [curie]}
-    result = post_query(url=NODE_NORMALIZER_SERVER, query=j, server="Post Node Normalizer Query")
-    assert result
-    assert curie in result
-    assert "equivalent_identifiers" in result[curie]
-    assert len(result[curie]["equivalent_identifiers"])
-    assert category in result[curie]["type"]
-
-
-# @pytest.mark.asyncio
-# async def test_execute_trapi_lookup():
-#     url: str = TRAPI_TEST_ENDPOINT
-#     subject_id = 'MONDO:0005301'
-#     subject_category = "biolink:Disease"
-#     predicate_name = "treats"
-#     predicate_id = f"biolink:{predicate_name}"
-#     object_id = 'PUBCHEM.COMPOUND:107970'
-#     object_category = "biolink:SmallMolecule"
-#     oht: OneHopTest = OneHopTest(endpoints=[url])
-#     test_asset: TestAsset = oht.build_test_asset(
-#         subject_id=subject_id,
-#         subject_category=subject_category,
-#         predicate_id=predicate_id,
-#         object_id=object_id,
-#         object_category=object_category
-#     )
-#     report: UnitTestReport = await run_one_hop_unit_test(
-#         url=url,
-#         test_asset=test_asset,
-#         creator=by_subject,
-#         trapi_version="1.4.2",
-#         # biolink_version=None
-#     )
-#     assert report
+async def test_run_one_hop_tests_with_runner_parameters(
+        data: Dict,
+        environment: str,
+        components: List[str],
+        expected_result
+):
+    results: Dict = await run_one_hop_tests(
+        **data,
+        environment=environment,
+        components=components,
+        strict_validation=True
+    )
+    assert results
+    dump(results, stderr, indent=4)
+
+
+# subprocess.run(
+#     args, *, stdin=None, input=None, stdout=None, stderr=None,
+#     capture_output=False, shell=False, cwd=None, timeout=None,
+#     check=False, encoding=None, errors=None, text=None, env=None,
+#     universal_newlines=None, **other_popen_kwargs
+# )
+@pytest.mark.skip("Not yet fully implemented")
+def test_one_hop_cli():
+    # command: List = ["python", "-m", "one_hop_test_runner.__init__"]
+    # args: Dict = SAMPLE_TEST_INPUT_1.copy()
+    # args["components"] = "arax,molepro"
+    # [command.extend([f"--{flag}", value]) for flag, value in args.items()]
+    # results = check_output(["dir"])
+    # results = check_output([
+    #     "python", "-m", "venv", "--clear", "test_venv", ";",
+    #     ".", "test_venv/bin/activate"
+    # ])
+    subprocess.run("one_hop_test_runner", stdout=stdout, shell=True, cwd=SCRIPTS_DIR)
```

### Comparing `graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/test_unit_test_templates.py` & `graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/test_unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py` & `graph_validation_test_runners-0.1.3/tests/graph_validation_test_runner/translator/test_translator_smartapi_registry.py`

 * *Files identical despite different names*

### Comparing `graph_validation_test_runners-0.1.2/tests/standards_validation_test_runner/test_standards_validation_test.py` & `graph_validation_test_runners-0.1.3/tests/standards_validation_test_runner/test_standards_validation_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 """
 Unit tests for Standards Validation Test code validation
 """
 from sys import stderr
-from typing import Dict
+from typing import List, Dict
 from json import dump
 import pytest
 
-from graph_validation_tests.utils.unit_test_templates import by_subject, by_object
-from standards_validation_test_runner import StandardsValidationTest, run_standards_validation_tests
-from tests import SAMPLE_MOLEPRO_INPUT_DATA, SAMPLE_ARAX_INPUT_DATA, SAMPLE_ARAGORN_INPUT_DATA
+from graph_validation_tests.utils.unit_test_templates import (
+    by_subject,
+    by_object
+)
+from standards_validation_test_runner import (
+    StandardsValidationTest,
+    run_standards_validation_tests
+)
+from tests import (
+    SAMPLE_MOLEPRO_INPUT_DATA,
+    SAMPLE_ARAX_INPUT_DATA,
+    SAMPLE_ARAGORN_INPUT_DATA
+)
 
 
 @pytest.mark.parametrize(
     "data,environment,component,expected_result",
     [
         (
             SAMPLE_MOLEPRO_INPUT_DATA,
@@ -67,43 +77,49 @@
         trapi_generators=trapi_generators,
         environment="prod"
     )
     assert not results
 
 
 @pytest.mark.parametrize(
-    "data,environment,component,expected_result",
+    "data,environment,components,expected_result",
     [
-        (
+        (   # Query 0 - MolePro test
             SAMPLE_MOLEPRO_INPUT_DATA,
             "ci",
-            "molepro",
+            ["molepro"],
             None
         ),
-        (
+        (   # Query 1 - ARAX test
             SAMPLE_ARAX_INPUT_DATA,
             "ci",
-            "arax",
+            ["arax"],
             None
         ),
-        (
+        (   # Query 2 - Aragorn test
             SAMPLE_ARAGORN_INPUT_DATA,
             "ci",
-            "aragorn",
+            ["aragorn"],
+            None
+        ),
+        (   # Query 3 - Combined ARAX and MolePro test
+            SAMPLE_MOLEPRO_INPUT_DATA,
+            "ci",
+            ["molepro", "arax", "aragorn"],
             None
         )
     ]
 )
 @pytest.mark.asyncio
 async def test_run_standards_validation_tests(
         data: Dict,
         environment: str,
-        component: str,
+        components: List[str],
         expected_result
 ):
     results: Dict = await run_standards_validation_tests(
         **data,
         environment=environment,
-        components=[component]
+        components=components
     )
     assert results
     dump(results, stderr, indent=4)
```

### Comparing `graph_validation_test_runners-0.1.2/PKG-INFO` & `graph_validation_test_runners-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-validation-test-runners
-Version: 0.1.2
+Version: 0.1.3
 Summary: Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation
 Home-page: https://github.com/TranslatorSRI
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: deepdiff (>=6.7.1,<7.0.0)
 Requires-Dist: fastapi
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: reasoner-validator (>=4.1.6,<5.0.0)
+Requires-Dist: reasoner-validator (>=4.2.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: translator-testing-model (>=0.3.1,<0.4.0)
 Project-URL: Bug Tracker, https://github.com/TranslatorSRI/graph-validation-test-runners/issues
 Project-URL: Change Log, https://github.com/TranslatorSRI/graph-validation-test-runners/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/TranslatorSRI/graph-validation-test-runners/blob/main/README.md
 Project-URL: Repository, https://github.com/TranslatorSRI/graph-validation-test-runners
```


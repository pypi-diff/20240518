# Comparing `tmp/qgate_sln_mlrun-0.2.3-py3-none-any.whl.zip` & `tmp/qgate_sln_mlrun-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,47 +1,54 @@
-Zip file size: 50937 bytes, number of entries: 45
+Zip file size: 56254 bytes, number of entries: 52
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Nov-10 20:59 qgate_sln_mlrun/__init__.py
--rw-rw-rw-  2.0 fat     7261 b- defN 24-Apr-30 13:44 qgate_sln_mlrun/mysqlhelper.py
 -rw-rw-rw-  2.0 fat     9317 b- defN 24-Apr-20 16:47 qgate_sln_mlrun/output.py
--rw-rw-rw-  2.0 fat     9731 b- defN 24-May-02 14:36 qgate_sln_mlrun/qualityreport.py
--rw-rw-rw-  2.0 fat     4740 b- defN 24-Apr-19 16:05 qgate_sln_mlrun/setup.py
--rw-rw-rw-  2.0 fat       53 b- defN 24-May-03 05:13 qgate_sln_mlrun/version.py
+-rw-rw-rw-  2.0 fat    10021 b- defN 24-May-07 16:24 qgate_sln_mlrun/qualityreport.py
+-rw-rw-rw-  2.0 fat     4830 b- defN 24-May-07 18:55 qgate_sln_mlrun/setup.py
+-rw-rw-rw-  2.0 fat       53 b- defN 24-May-18 18:17 qgate_sln_mlrun/version.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-07 14:52 qgate_sln_mlrun/helper/__init__.py
+-rw-rw-rw-  2.0 fat      872 b- defN 24-May-12 13:16 qgate_sln_mlrun/helper/basehelper.py
+-rw-rw-rw-  2.0 fat     5488 b- defN 24-May-12 13:16 qgate_sln_mlrun/helper/kafkahelper.py
+-rw-rw-rw-  2.0 fat     6945 b- defN 24-May-12 13:16 qgate_sln_mlrun/helper/mysqlhelper.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 14:43 qgate_sln_mlrun/model_changes/__init__.py
 -rw-rw-rw-  2.0 fat      312 b- defN 24-Apr-04 17:53 qgate_sln_mlrun/model_changes/empty-template.json
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 14:43 qgate_sln_mlrun/templates/__init__.py
 -rw-rw-rw-  2.0 fat    10411 b- defN 24-Apr-30 20:00 qgate_sln_mlrun/templates/qgt-mlrun.html
 -rw-rw-rw-  2.0 fat     1468 b- defN 24-Apr-20 18:45 qgate_sln_mlrun/templates/qgt-mlrun.txt
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:59 qgate_sln_mlrun/ts/__init__.py
--rw-rw-rw-  2.0 fat     5702 b- defN 24-Apr-28 20:28 qgate_sln_mlrun/ts/tsbase.py
--rw-rw-rw-  2.0 fat     4199 b- defN 24-Apr-30 19:08 qgate_sln_mlrun/ts/tshelper.py
+-rw-rw-rw-  2.0 fat     5768 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/tsbase.py
+-rw-rw-rw-  2.0 fat     4121 b- defN 24-May-11 14:51 qgate_sln_mlrun/ts/tshelper.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:37 qgate_sln_mlrun/ts/ts01_project/__init__.py
--rw-rw-rw-  2.0 fat     1122 b- defN 24-Apr-10 13:54 qgate_sln_mlrun/ts/ts01_project/ts101.py
--rw-rw-rw-  2.0 fat     2474 b- defN 24-Apr-30 12:12 qgate_sln_mlrun/ts/ts01_project/ts102.py
+-rw-rw-rw-  2.0 fat     1100 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts01_project/ts101.py
+-rw-rw-rw-  2.0 fat     2620 b- defN 24-May-12 05:52 qgate_sln_mlrun/ts/ts01_project/ts102.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:37 qgate_sln_mlrun/ts/ts02_feature_set/__init__.py
--rw-rw-rw-  2.0 fat     9137 b- defN 24-Apr-26 19:24 qgate_sln_mlrun/ts/ts02_feature_set/ts201.py
--rw-rw-rw-  2.0 fat     3530 b- defN 24-May-02 14:36 qgate_sln_mlrun/ts/ts02_feature_set/ts202.py
--rw-rw-rw-  2.0 fat     3043 b- defN 24-May-02 14:36 qgate_sln_mlrun/ts/ts02_feature_set/ts203.py
--rw-rw-rw-  2.0 fat     3054 b- defN 24-May-02 14:36 qgate_sln_mlrun/ts/ts02_feature_set/ts204.py
--rw-rw-rw-  2.0 fat     3460 b- defN 24-May-02 14:36 qgate_sln_mlrun/ts/ts02_feature_set/ts205.py
--rw-rw-rw-  2.0 fat     3511 b- defN 24-May-02 14:36 qgate_sln_mlrun/ts/ts02_feature_set/ts206.py
+-rw-rw-rw-  2.0 fat     9200 b- defN 24-May-07 19:15 qgate_sln_mlrun/ts/ts02_feature_set/ts201.py
+-rw-rw-rw-  2.0 fat     3586 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts02_feature_set/ts202.py
+-rw-rw-rw-  2.0 fat     3047 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts02_feature_set/ts203.py
+-rw-rw-rw-  2.0 fat     3058 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts02_feature_set/ts204.py
+-rw-rw-rw-  2.0 fat     3517 b- defN 24-May-12 12:55 qgate_sln_mlrun/ts/ts02_feature_set/ts205.py
+-rw-rw-rw-  2.0 fat     3128 b- defN 24-May-13 17:24 qgate_sln_mlrun/ts/ts02_feature_set/ts206.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:39 qgate_sln_mlrun/ts/ts03_ingest_data/__init__.py
--rw-rw-rw-  2.0 fat     2697 b- defN 24-May-02 07:02 qgate_sln_mlrun/ts/ts03_ingest_data/ts302.py
--rw-rw-rw-  2.0 fat     2187 b- defN 24-May-02 07:02 qgate_sln_mlrun/ts/ts03_ingest_data/ts303.py
--rw-rw-rw-  2.0 fat     2229 b- defN 24-May-02 07:02 qgate_sln_mlrun/ts/ts03_ingest_data/ts304.py
--rw-rw-rw-  2.0 fat     3000 b- defN 24-May-02 07:02 qgate_sln_mlrun/ts/ts03_ingest_data/ts305.py
+-rw-rw-rw-  2.0 fat     2045 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts03_ingest_data/ts301.py
+-rw-rw-rw-  2.0 fat     2731 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts03_ingest_data/ts302.py
+-rw-rw-rw-  2.0 fat     2191 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts03_ingest_data/ts303.py
+-rw-rw-rw-  2.0 fat     2212 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts03_ingest_data/ts304.py
+-rw-rw-rw-  2.0 fat     3036 b- defN 24-May-12 12:55 qgate_sln_mlrun/ts/ts03_ingest_data/ts305.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:39 qgate_sln_mlrun/ts/ts04_feature_vector/__init__.py
--rw-rw-rw-  2.0 fat     2491 b- defN 24-Apr-10 13:56 qgate_sln_mlrun/ts/ts04_feature_vector/ts401.py
+-rw-rw-rw-  2.0 fat     2495 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts04_feature_vector/ts401.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:40 qgate_sln_mlrun/ts/ts05_get_data/__init__.py
--rw-rw-rw-  2.0 fat     1190 b- defN 24-Apr-10 13:56 qgate_sln_mlrun/ts/ts05_get_data/ts501.py
--rw-rw-rw-  2.0 fat     4234 b- defN 24-Apr-10 13:56 qgate_sln_mlrun/ts/ts05_get_data/ts502.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts05_get_data/ts501.py
+-rw-rw-rw-  2.0 fat     4238 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts05_get_data/ts502.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:41 qgate_sln_mlrun/ts/ts06_pipeline/__init__.py
--rw-rw-rw-  2.0 fat     2704 b- defN 24-Apr-23 14:11 qgate_sln_mlrun/ts/ts06_pipeline/ts601.py
+-rw-rw-rw-  2.0 fat     3249 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts06_pipeline/ts601.py
+-rw-rw-rw-  2.0 fat     1177 b- defN 24-May-06 11:29 qgate_sln_mlrun/ts/ts06_pipeline/ts601_ext_code.py
+-rw-rw-rw-  2.0 fat     2632 b- defN 24-May-18 16:57 qgate_sln_mlrun/ts/ts06_pipeline/ts602.py
+-rw-rw-rw-  2.0 fat     2451 b- defN 24-May-18 17:03 qgate_sln_mlrun/ts/ts06_pipeline/ts602_ext_code.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:42 qgate_sln_mlrun/ts/ts07_build_model/__init__.py
--rw-rw-rw-  2.0 fat     3568 b- defN 24-Apr-10 13:56 qgate_sln_mlrun/ts/ts07_build_model/ts701.py
+-rw-rw-rw-  2.0 fat     3522 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts07_build_model/ts701.py
 -rw-rw-rw-  2.0 fat       57 b- defN 24-May-02 13:43 qgate_sln_mlrun/ts/ts08_serve_model/__init__.py
--rw-rw-rw-  2.0 fat     3159 b- defN 24-Apr-10 13:56 qgate_sln_mlrun/ts/ts08_serve_model/ts801.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-May-03 05:22 qgate_sln_mlrun-0.2.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9221 b- defN 24-May-03 05:22 qgate_sln_mlrun-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-03 05:22 qgate_sln_mlrun-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 24-May-03 05:22 qgate_sln_mlrun-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4286 b- defN 24-May-03 05:22 qgate_sln_mlrun-0.2.3.dist-info/RECORD
-45 files, 135824 bytes uncompressed, 43887 bytes compressed:  67.7%
+-rw-rw-rw-  2.0 fat     2993 b- defN 24-May-06 20:49 qgate_sln_mlrun/ts/ts08_serve_model/ts801.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-May-18 18:18 qgate_sln_mlrun-0.2.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9140 b- defN 24-May-18 18:18 qgate_sln_mlrun-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 18:18 qgate_sln_mlrun-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-18 18:18 qgate_sln_mlrun-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     4981 b- defN 24-May-18 18:18 qgate_sln_mlrun-0.2.4.dist-info/RECORD
+52 files, 151482 bytes uncompressed, 48074 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -1,25 +1,34 @@
 Filename: qgate_sln_mlrun/__init__.py
 Comment: 
 
-Filename: qgate_sln_mlrun/mysqlhelper.py
-Comment: 
-
 Filename: qgate_sln_mlrun/output.py
 Comment: 
 
 Filename: qgate_sln_mlrun/qualityreport.py
 Comment: 
 
 Filename: qgate_sln_mlrun/setup.py
 Comment: 
 
 Filename: qgate_sln_mlrun/version.py
 Comment: 
 
+Filename: qgate_sln_mlrun/helper/__init__.py
+Comment: 
+
+Filename: qgate_sln_mlrun/helper/basehelper.py
+Comment: 
+
+Filename: qgate_sln_mlrun/helper/kafkahelper.py
+Comment: 
+
+Filename: qgate_sln_mlrun/helper/mysqlhelper.py
+Comment: 
+
 Filename: qgate_sln_mlrun/model_changes/__init__.py
 Comment: 
 
 Filename: qgate_sln_mlrun/model_changes/empty-template.json
 Comment: 
 
 Filename: qgate_sln_mlrun/templates/__init__.py
@@ -69,14 +78,17 @@
 
 Filename: qgate_sln_mlrun/ts/ts02_feature_set/ts206.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts03_ingest_data/__init__.py
 Comment: 
 
+Filename: qgate_sln_mlrun/ts/ts03_ingest_data/ts301.py
+Comment: 
+
 Filename: qgate_sln_mlrun/ts/ts03_ingest_data/ts302.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts03_ingest_data/ts303.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts03_ingest_data/ts304.py
@@ -102,35 +114,44 @@
 
 Filename: qgate_sln_mlrun/ts/ts06_pipeline/__init__.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts06_pipeline/ts601.py
 Comment: 
 
+Filename: qgate_sln_mlrun/ts/ts06_pipeline/ts601_ext_code.py
+Comment: 
+
+Filename: qgate_sln_mlrun/ts/ts06_pipeline/ts602.py
+Comment: 
+
+Filename: qgate_sln_mlrun/ts/ts06_pipeline/ts602_ext_code.py
+Comment: 
+
 Filename: qgate_sln_mlrun/ts/ts07_build_model/__init__.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts07_build_model/ts701.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts08_serve_model/__init__.py
 Comment: 
 
 Filename: qgate_sln_mlrun/ts/ts08_serve_model/ts801.py
 Comment: 
 
-Filename: qgate_sln_mlrun-0.2.3.dist-info/LICENSE
+Filename: qgate_sln_mlrun-0.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_sln_mlrun-0.2.3.dist-info/METADATA
+Filename: qgate_sln_mlrun-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: qgate_sln_mlrun-0.2.3.dist-info/WHEEL
+Filename: qgate_sln_mlrun-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_sln_mlrun-0.2.3.dist-info/top_level.txt
+Filename: qgate_sln_mlrun-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_sln_mlrun-0.2.3.dist-info/RECORD
+Filename: qgate_sln_mlrun-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_sln_mlrun/qualityreport.py

```diff
@@ -1,47 +1,52 @@
 import glob
 import json
 import os
 from qgate_sln_mlrun.setup import Setup, ProjectDelete
 from qgate_sln_mlrun.output import Output
 from qgate_sln_mlrun.ts.ts08_serve_model import ts801
 from qgate_sln_mlrun.ts.ts07_build_model import ts701
+from qgate_sln_mlrun.ts.ts06_pipeline import ts601, ts602
 from qgate_sln_mlrun.ts.ts05_get_data import ts501, ts502
 from qgate_sln_mlrun.ts.ts04_feature_vector import ts401
-from qgate_sln_mlrun.ts.ts03_ingest_data import ts305, ts302, ts304, ts303
-from qgate_sln_mlrun.ts.ts02_feature_set import ts201, ts203, ts205, ts204, ts202, ts206
-from qgate_sln_mlrun.ts.ts01_project import ts102, ts101
+from qgate_sln_mlrun.ts.ts03_ingest_data import ts301, ts302, ts303, ts304, ts305
+from qgate_sln_mlrun.ts.ts02_feature_set import ts201, ts202, ts203, ts204, ts205, ts206
+from qgate_sln_mlrun.ts.ts01_project import ts101, ts102
 from qgate_sln_mlrun.ts import tsbase
 import importlib.resources
 
 
 class QualityReport:
     """
     Quality report
     """
 
     TEST_SCENARIOS = [ts101.TS101,
                       ts201.TS201, ts202.TS202, ts203.TS203, ts204.TS204, ts205.TS205, ts206.TS206,
-                      ts302.TS302, ts303.TS303, ts304.TS304, ts305.TS305,
+                      ts301.TS301, ts302.TS302, ts303.TS303, ts304.TS304, ts305.TS305,
                       ts401.TS401,
-                      ts501.TS501, ts502.TS502]
+                      ts501.TS501, ts502.TS502,
+                      ts601.TS601, ts602.TS602]
     TEST_EXPERIMENTS = [ts701.TS701, ts801.TS801]
     TEST_SCENARIO_DELETE = ts102.TS102
 
 
     # Target vs On/Off-line
     TARGET_ONLINE = ["kafka", "redis", "mysql", "postgres"]
     TARGET_OFFLINE = ["parquet", "csv"]
 
     # Target vs invalid tests
     TARGET_NOT_VALID_TEST = {"kafka": ["TS501", "TS502"]}
 
     # Test vs Only On/Off-line
-    TEST_BOTH = ["TS101","TS102","TS201", "TS202", "TS203", "TS204", "TS205", "TS206",
-                 "TS301", "TS302", "TS303", "TS304", "TS305", "TS401"]
+    TEST_BOTH = ["TS101","TS102",
+                 "TS201", "TS202", "TS203", "TS204", "TS205", "TS206",
+                 "TS301", "TS302", "TS303", "TS304", "TS305",
+                 "TS401",
+                 "TS601", "TS602"]
     TEST_ONLY_OFFLINE = ["TS501","TS701","TS801"]
     TEST_ONLY_ONLINE = ["TS502"]
 
 
     def __init__(self, setup: Setup, output: Output):
         self._setup = setup
         self._output = output
@@ -108,17 +113,14 @@
         return projects_avoid_ts
 
     def execute(self, delete_scenario: ProjectDelete=ProjectDelete.FULL_DELETE, experiment_scenario=False, filter_projects: list=None):
 
         # define valid projects
         self._define_projects(filter_projects)
 
-        # TODO: Define, which test scenarios will be valid for specific project
-
-
         # define, which test scenarios will be executed
         test_scenarios = self.build_scenarios(delete_scenario, experiment_scenario)
 
         # define, which test scenarios will be valid for specific project based on target type, etc.
         projects_avoid_ts = self._projects_avoid_testscenarios()
 
         # setup filter test scenarios
@@ -126,31 +128,36 @@
 
         for test_scenario in test_scenarios:
             if test_scenario:
                 # create instance
                 ts = test_scenario(self)
                 try:
 
-                    # execution of test case
+                    # apply QGATE_FILTER_SCENARIOS, focus on only the specific test scenarios
+                    if filter_scenarios:
+                        if not ts.name in filter_scenarios:
+                            continue
+
+                    # write info about TS to the output
                     ts.testscenario_new()
+
+                    # BEFORE execution of TS
                     ts.before()
+                    # EXEC execute of TS
+                    ts.exec()
 
                     for project_name in self.projects:
-                        # avoid irrelevant scenarios for this project
                         if ts.name in projects_avoid_ts[project_name]:
+                            # avoid irrelevant scenarios for this project
                             continue
 
-                        # apply QGATE_FILTER_SCENARIOS, focus on only the specific test scenarios
-                        if filter_scenarios:
-                            if not ts.name in filter_scenarios:
-                                continue
-
-                        # execute TS for this project
-                        ts.exec(project_name)
+                        # PRJ_EXEC execute of TS for project
+                        ts.prj_exec(project_name)
 
+                    # AFTER execute of TS
                     ts.after()
                     ts.state = tsbase.TSState.DONE
                 except Exception as ex:
                     ts.state = tsbase.TSState.ERR
                     ts.testcase_detail(f"{type(ex).__name__}: {str(ex)}")
                     ts.testcase_state("ERR")
         self._output.render(self.projects, self.project_descs)
```

## qgate_sln_mlrun/setup.py

```diff
@@ -24,274 +24,279 @@
 00000170: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
 00000180: 732e 5f69 6e73 7461 6e63 6573 5b63 6c73  s._instances[cls
 00000190: 5d0d 0a0d 0a63 6c61 7373 2053 6574 7570  ]....class Setup
 000001a0: 286d 6574 6163 6c61 7373 3d53 696e 676c  (metaclass=Singl
 000001b0: 6574 6f6e 293a 0d0a 2020 2020 2222 220d  eton):..    """.
 000001c0: 0a20 2020 2053 6574 7570 2066 6f72 2073  .    Setup for s
 000001d0: 6f6c 7574 696f 6e0d 0a20 2020 2022 2222  olution..    """
-000001e0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
-000001f0: 6974 5f5f 2873 656c 662c 206d 6c72 756e  it__(self, mlrun
-00000200: 5f65 6e76 5f66 696c 653a 206c 6973 745b  _env_file: list[
-00000210: 7374 725d 2c20 6461 7461 7365 745f 6e61  str], dataset_na
-00000220: 6d65 203d 204e 6f6e 652c 2068 6172 645f  me = None, hard_
-00000230: 7661 7269 6162 6c65 733a 2064 6963 743d  variables: dict=
-00000240: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-00000250: 2222 2244 6566 696e 6520 7365 7474 696e  """Define settin
-00000260: 6720 666f 7220 7465 7374 696e 670d 0a0d  g for testing...
-00000270: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000280: 6d6c 7275 6e5f 656e 765f 6669 6c65 3a20  mlrun_env_file: 
-00000290: 206c 6973 7420 6f66 202a 2e65 6e76 2066   list of *.env f
-000002a0: 696c 6573 2c20 6669 7273 7420 7661 6c69  iles, first vali
-000002b0: 6420 6669 6c65 2077 696c 6c20 6265 0d0a  d file will be..
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000002e0: 7573 6564 2065 2e67 2e20 5b22 7167 6174  used e.g. ["qgat
-000002f0: 652d 736c 6e2d 6d6c 7275 6e2d 7072 6976  e-sln-mlrun-priv
-00000300: 6174 652e 656e 7622 2c20 2271 6761 7465  ate.env", "qgate
-00000310: 2d73 6c6e 2d6d 6c72 756e 2e65 6e76 225d  -sln-mlrun.env"]
-00000320: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00000330: 2064 6174 6173 6574 5f6e 616d 653a 2020   dataset_name:  
-00000340: 2020 6e61 6d65 206f 6620 6461 7461 2073    name of data s
-00000350: 6574 2065 2e67 2e20 2230 312d 7369 7a65  et e.g. "01-size
-00000360: 2d31 3030 220d 0a20 2020 2020 2020 203a  -100"..        :
-00000370: 7061 7261 6d20 6861 7264 5f76 6172 6961  param hard_varia
-00000380: 626c 6573 3a20 206e 6577 206f 7220 7265  bles:  new or re
-00000390: 706c 6163 656d 656e 7420 6f66 2076 6172  placement of var
-000003a0: 6961 626c 6573 2066 726f 6d20 2a2e 656e  iables from *.en
-000003b0: 7620 6669 6c65 0d0a 2020 2020 2020 2020  v file..        
-000003c0: 2222 220d 0a20 2020 2020 2020 2023 2073  """..        # s
-000003d0: 6574 2076 6172 6961 626c 6573 2062 6173  et variables bas
-000003e0: 6564 206f 6e20 656e 7669 726f 6e6d 656e  ed on environmen
-000003f0: 7420 6669 6c65 730d 0a20 2020 2020 2020  t files..       
-00000400: 2066 6f72 2065 6e76 5f66 696c 6520 696e   for env_file in
-00000410: 206d 6c72 756e 5f65 6e76 5f66 696c 653a   mlrun_env_file:
-00000420: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000430: 206f 732e 7061 7468 2e69 7366 696c 6528   os.path.isfile(
-00000440: 656e 765f 6669 6c65 293a 0d0a 2020 2020  env_file):..    
-00000450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000460: 2e5f 7661 7269 6162 6c65 733d 6d6c 7275  ._variables=mlru
-00000470: 6e2e 7365 745f 656e 765f 6672 6f6d 5f66  n.set_env_from_f
-00000480: 696c 6528 656e 765f 6669 6c65 2c20 7265  ile(env_file, re
-00000490: 7475 726e 5f64 6963 743d 5472 7565 290d  turn_dict=True).
-000004a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004b0: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
-000004c0: 2020 2320 7075 7368 2064 6174 6173 6574    # push dataset
-000004d0: 206e 616d 650d 0a20 2020 2020 2020 2069   name..        i
-000004e0: 6620 6461 7461 7365 745f 6e61 6d65 3a0d  f dataset_name:.
-000004f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00000500: 662e 5f76 6172 6961 626c 6573 5b22 5147  f._variables["QG
-00000510: 4154 455f 4441 5441 5345 5422 5d20 3d20  ATE_DATASET"] = 
-00000520: 6461 7461 7365 745f 6e61 6d65 0d0a 0d0a  dataset_name....
-00000530: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00000540: 206e 6577 206f 7220 7265 7772 6974 6520   new or rewrite 
-00000550: 7661 7269 6162 6c65 730d 0a20 2020 2020  variables..     
-00000560: 2020 2069 6620 6861 7264 5f76 6172 6961     if hard_varia
-00000570: 626c 6573 3a0d 0a20 2020 2020 2020 2020  bles:..         
-00000580: 2020 2066 6f72 206b 6579 2069 6e20 6861     for key in ha
-00000590: 7264 5f76 6172 6961 626c 6573 2e6b 6579  rd_variables.key
-000005a0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-000005b0: 2020 2020 2020 7365 6c66 2e5f 7661 7269        self._vari
-000005c0: 6162 6c65 735b 6b65 795d 3d68 6172 645f  ables[key]=hard_
-000005d0: 7661 7269 6162 6c65 735b 6b65 795d 0d0a  variables[key]..
-000005e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000005f0: 7661 7269 6162 6c65 735b 2244 4952 225d  variables["DIR"]
-00000600: 3d6f 732e 6765 7463 7764 2829 0d0a 0d0a  =os.getcwd()....
-00000610: 2020 2020 2020 2020 2320 6d6f 6465 6c20          # model 
-00000620: 6465 6669 6e69 7469 6f6e 2073 6574 7469  definition setti
-00000630: 6e67 0d0a 2020 2020 2020 2020 7365 6c66  ng..        self
-00000640: 2e5f 6d6f 6465 6c5f 6465 6669 6e69 7469  ._model_definiti
-00000650: 6f6e 5f73 6574 7469 6e67 3d7b 7d0d 0a20  on_setting={}.. 
-00000660: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00000670: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-00000680: 6c66 2e6d 6f64 656c 5f64 6566 696e 6974  lf.model_definit
-00000690: 696f 6e2c 2022 3031 2d6d 6f64 656c 222c  ion, "01-model",
-000006a0: 2022 6d6f 6465 6c2e 6a73 6f6e 2229 2c20   "model.json"), 
-000006b0: 2272 2229 2061 7320 6a73 6f6e 5f66 696c  "r") as json_fil
-000006c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000006d0: 7365 7474 696e 6720 3d20 6a73 6f6e 2e6c  setting = json.l
-000006e0: 6f61 6428 6a73 6f6e 5f66 696c 6529 0d0a  oad(json_file)..
-000006f0: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
-00000700: 6465 6c5f 6465 6669 6e69 7469 6f6e 5f73  del_definition_s
-00000710: 6574 7469 6e67 3d73 6574 7469 6e67 5b22  etting=setting["
-00000720: 7370 6563 225d 0d0a 0d0a 2020 2020 6465  spec"]....    de
-00000730: 6620 5f5f 7374 725f 5f28 7365 6c66 293a  f __str__(self):
-00000740: 0d0a 2020 2020 2020 2020 7265 743d 2222  ..        ret=""
-00000750: 0d0a 2020 2020 2020 2020 666f 7220 6b65  ..        for ke
-00000760: 7920 696e 2073 656c 662e 5f76 6172 6961  y in self._varia
-00000770: 626c 6573 2e6b 6579 7328 293a 0d0a 2020  bles.keys():..  
-00000780: 2020 2020 2020 2020 2020 7265 742b 3d6b            ret+=k
-00000790: 6579 2b20 223a 2022 2b20 2227 2220 2b20  ey+ ": "+ "'" + 
-000007a0: 7374 7228 7365 6c66 2e5f 7661 7269 6162  str(self._variab
-000007b0: 6c65 735b 6b65 795d 2920 2b20 2227 5c6e  les[key]) + "'\n
-000007c0: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-000007d0: 6e20 7265 745b 3a2d 315d 0d0a 0d0a 2020  n ret[:-1]....  
-000007e0: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-000007f0: 2064 6566 2076 6172 6961 626c 6573 2873   def variables(s
-00000800: 656c 6629 3a0d 0a20 2020 2020 2020 2076  elf):..        v
-00000810: 6172 6961 626c 655f 6c69 7374 3d5b 5d0d  ariable_list=[].
-00000820: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-00000830: 2069 6e20 7365 6c66 2e5f 7661 7269 6162   in self._variab
-00000840: 6c65 732e 6b65 7973 2829 3a0d 0a20 2020  les.keys():..   
-00000850: 2020 2020 2020 2020 2069 746d 203d 207b           itm = {
-00000860: 7d0d 0a20 2020 2020 2020 2020 2020 2069  }..            i
-00000870: 746d 5b27 6b65 7927 5d3d 6b65 790d 0a20  tm['key']=key.. 
-00000880: 2020 2020 2020 2020 2020 2069 746d 5b27             itm['
-00000890: 7661 6c75 6527 5d3d 7365 6c66 2e5f 7661  value']=self._va
-000008a0: 7269 6162 6c65 735b 6b65 795d 0d0a 2020  riables[key]..  
-000008b0: 2020 2020 2020 2020 2020 7661 7269 6162            variab
-000008c0: 6c65 5f6c 6973 742e 6170 7065 6e64 2869  le_list.append(i
-000008d0: 746d 290d 0a20 2020 2020 2020 2072 6574  tm)..        ret
-000008e0: 7572 6e20 7661 7269 6162 6c65 5f6c 6973  urn variable_lis
-000008f0: 740d 0a0d 0a20 2020 2040 7072 6f70 6572  t....    @proper
-00000900: 7479 0d0a 2020 2020 6465 6620 7573 6564  ty..    def used
-00000910: 5f66 696c 7465 7273 2873 656c 6629 3a0d  _filters(self):.
-00000920: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
-00000930: 6b2c 2069 6620 736f 6d65 2066 696c 7465  k, if some filte
-00000940: 7220 6973 2075 7365 6422 2222 0d0a 2020  r is used"""..  
-00000950: 2020 2020 2020 6966 2073 656c 662e 6669        if self.fi
-00000960: 6c74 6572 5f73 6365 6e61 7269 6f73 3a0d  lter_scenarios:.
-00000970: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000980: 6c65 6e28 7365 6c66 2e66 696c 7465 725f  len(self.filter_
-00000990: 7363 656e 6172 696f 7329 3e30 3a0d 0a20  scenarios)>0:.. 
-000009a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000009b0: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-000009c0: 2020 2020 6966 2073 656c 662e 6669 6c74      if self.filt
-000009d0: 6572 5f70 726f 6a65 6374 733a 0d0a 2020  er_projects:..  
-000009e0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000009f0: 2873 656c 662e 6669 6c74 6572 5f70 726f  (self.filter_pro
-00000a00: 6a65 6374 7329 3e30 3a0d 0a20 2020 2020  jects)>0:..     
-00000a10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000a20: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
-00000a30: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-00000a40: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00000a50: 2020 2064 6566 206d 6f64 656c 5f6f 7574     def model_out
-00000a60: 7075 7428 7365 6c66 293a 0d0a 2020 2020  put(self):..    
-00000a70: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-00000a80: 6520 6d6f 6465 6c20 6f75 7470 7574 2070  e model output p
-00000a90: 6174 6822 2222 0d0a 2020 2020 2020 2020  ath"""..        
-00000aa0: 7265 7475 726e 2073 656c 662e 5f76 6172  return self._var
-00000ab0: 6961 626c 6573 2e67 6574 2827 5147 4154  iables.get('QGAT
-00000ac0: 455f 4f55 5450 5554 272c 2027 2e2f 6f75  E_OUTPUT', './ou
-00000ad0: 7470 7574 2729 0d0a 0d0a 2020 2020 4070  tput')....    @p
-00000ae0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00000af0: 206d 6f64 656c 5f64 6566 696e 6974 696f   model_definitio
-00000b00: 6e28 7365 6c66 293a 0d0a 2020 2020 2020  n(self):..      
-00000b10: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
-00000b20: 7061 7468 2074 6f20 6d6f 6465 6c20 6465  path to model de
-00000b30: 6669 6e69 7469 6f6e 2222 220d 0a20 2020  finition"""..   
-00000b40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000b50: 2e5f 7661 7269 6162 6c65 735b 2751 4741  ._variables['QGA
-00000b60: 5445 5f44 4546 494e 4954 494f 4e27 5d0d  TE_DEFINITION'].
-00000b70: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00000b80: 0d0a 2020 2020 6465 6620 6461 7461 7365  ..    def datase
-00000b90: 745f 6e61 6d65 2873 656c 6629 3a0d 0a20  t_name(self):.. 
-00000ba0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00000bb0: 2074 6865 2064 6174 6173 6574 2073 6574   the dataset set
-00000bc0: 7469 6e67 2222 220d 0a20 2020 2020 2020  ting"""..       
-00000bd0: 2072 6574 7572 6e20 7365 6c66 2e5f 7661   return self._va
-00000be0: 7269 6162 6c65 732e 6765 7428 2251 4741  riables.get("QGA
-00000bf0: 5445 5f44 4154 4153 4554 222c 2022 3031  TE_DATASET", "01
-00000c00: 2d73 697a 652d 3130 3022 290d 0a0d 0a20  -size-100").... 
-00000c10: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00000c20: 2020 6465 6620 6669 6c74 6572 5f70 726f    def filter_pro
-00000c30: 6a65 6374 7328 7365 6c66 293a 0d0a 2020  jects(self):..  
-00000c40: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00000c50: 7468 6520 7072 6f6a 6563 7420 6669 6c74  the project filt
-00000c60: 6572 2073 6574 7469 6e67 2222 220d 0a20  er setting""".. 
-00000c70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00000c80: 6c66 2e5f 7661 7269 6162 6c65 732e 6765  lf._variables.ge
-00000c90: 7428 2251 4741 5445 5f46 494c 5445 525f  t("QGATE_FILTER_
-00000ca0: 5052 4f4a 4543 5453 222c 204e 6f6e 6529  PROJECTS", None)
-00000cb0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-00000cc0: 790d 0a20 2020 2064 6566 2066 696c 7465  y..    def filte
-00000cd0: 725f 7363 656e 6172 696f 7328 7365 6c66  r_scenarios(self
-00000ce0: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
-00000cf0: 6574 7572 6e20 7468 6520 7465 7374 2073  eturn the test s
-00000d00: 6365 6e61 7269 6f20 6669 6c74 6572 2073  cenario filter s
-00000d10: 6574 7469 6e67 2222 220d 0a20 2020 2020  etting"""..     
-00000d20: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00000d30: 7661 7269 6162 6c65 732e 6765 7428 2251  variables.get("Q
-00000d40: 4741 5445 5f46 494c 5445 525f 5343 454e  GATE_FILTER_SCEN
-00000d50: 4152 494f 5322 2c20 4e6f 6e65 290d 0a0d  ARIOS", None)...
-00000d60: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00000d70: 2020 2020 6465 6620 7265 6469 7328 7365      def redis(se
-00000d80: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
-00000d90: 2252 6574 7572 6e20 7468 6520 636f 6e6e  "Return the conn
-00000da0: 6563 7469 6f6e 2074 6f20 5265 6469 7322  ection to Redis"
-00000db0: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00000dc0: 726e 2073 656c 662e 5f76 6172 6961 626c  rn self._variabl
-00000dd0: 6573 2e67 6574 2827 5147 4154 455f 5245  es.get('QGATE_RE
-00000de0: 4449 5327 2c20 4e6f 6e65 290d 0a0d 0a20  DIS', None).... 
-00000df0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00000e00: 2020 6465 6620 6d79 7371 6c28 7365 6c66    def mysql(self
-00000e10: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
-00000e20: 6574 7572 6e20 7468 6520 636f 6e6e 6563  eturn the connec
-00000e30: 7469 6f6e 2074 6f20 4d79 5371 6c22 2222  tion to MySql"""
-00000e40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000e50: 2073 656c 662e 5f76 6172 6961 626c 6573   self._variables
-00000e60: 2e67 6574 2827 5147 4154 455f 4d59 5351  .get('QGATE_MYSQ
-00000e70: 4c27 2c20 4e6f 6e65 290d 0a0d 0a20 2020  L', None)....   
-00000e80: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00000e90: 6465 6620 706f 7374 6772 6573 2873 656c  def postgres(sel
-00000ea0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00000eb0: 5265 7475 726e 2074 6865 2063 6f6e 6e65  Return the conne
-00000ec0: 6374 696f 6e20 746f 2050 6f73 7467 7265  ction to Postgre
-00000ed0: 7322 2222 0d0a 2020 2020 2020 2020 7265  s"""..        re
-00000ee0: 7475 726e 2073 656c 662e 5f76 6172 6961  turn self._varia
-00000ef0: 626c 6573 2e67 6574 2827 5147 4154 455f  bles.get('QGATE_
-00000f00: 504f 5354 4752 4553 272c 204e 6f6e 6529  POSTGRES', None)
-00000f10: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-00000f20: 790d 0a20 2020 2064 6566 206b 6166 6b61  y..    def kafka
-00000f30: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00000f40: 2022 2222 5265 7475 726e 2074 6865 2063   """Return the c
-00000f50: 6f6e 6e65 6374 696f 6e20 746f 204b 6166  onnection to Kaf
-00000f60: 6b61 2222 220d 0a20 2020 2020 2020 2072  ka"""..        r
-00000f70: 6574 7572 6e20 7365 6c66 2e5f 7661 7269  eturn self._vari
-00000f80: 6162 6c65 732e 6765 7428 2751 4741 5445  ables.get('QGATE
-00000f90: 5f4b 4146 4b41 272c 204e 6f6e 6529 0d0a  _KAFKA', None)..
-00000fa0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00000fb0: 0a20 2020 2064 6566 2061 6e6f 6e79 6d5f  .    def anonym_
-00000fc0: 6d6f 6465 2873 656c 6629 202d 3e20 626f  mode(self) -> bo
-00000fd0: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
-00000fe0: 5265 7475 726e 2074 6865 2061 6e6f 6e79  Return the anony
-00000ff0: 6d6f 7573 206d 6f64 6522 2222 0d0a 2020  mous mode"""..  
-00001000: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00001010: 6520 6966 2073 656c 662e 5f76 6172 6961  e if self._varia
-00001020: 626c 6573 2e67 6574 2827 5147 4154 455f  bles.get('QGATE_
-00001030: 414e 4f4e 594d 5f4d 4f44 4527 2c20 224f  ANONYM_MODE', "O
-00001040: 6666 2229 2e6c 6f77 6572 2829 203d 3d20  ff").lower() == 
-00001050: 226f 6e22 2065 6c73 6520 4661 6c73 650d  "on" else False.
-00001060: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00001070: 0d0a 2020 2020 6465 6620 6373 765f 7365  ..    def csv_se
-00001080: 7061 7261 746f 7228 7365 6c66 293a 0d0a  parator(self):..
-00001090: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000010a0: 656c 662e 5f6d 6f64 656c 5f64 6566 696e  elf._model_defin
-000010b0: 6974 696f 6e5f 7365 7474 696e 675b 2243  ition_setting["C
-000010c0: 5356 5f53 4550 4152 4154 4f52 225d 0d0a  SV_SEPARATOR"]..
-000010d0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-000010e0: 0a20 2020 2064 6566 2063 7376 5f64 6563  .    def csv_dec
-000010f0: 696d 616c 2873 656c 6629 3a0d 0a20 2020  imal(self):..   
-00001100: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00001110: 2e5f 6d6f 6465 6c5f 6465 6669 6e69 7469  ._model_definiti
-00001120: 6f6e 5f73 6574 7469 6e67 5b22 4353 565f  on_setting["CSV_
-00001130: 4445 4349 4d41 4c22 5d0d 0a0d 0a20 2020  DECIMAL"]....   
-00001140: 2064 6566 2067 6574 5f73 6365 6e61 7269   def get_scenari
-00001150: 6f5f 7365 7474 696e 6728 7365 6c66 2c20  o_setting(self, 
-00001160: 6e61 6d65 293a 0d0a 2020 2020 2020 2020  name):..        
-00001170: 7265 7475 726e 2073 656c 662e 5f76 6172  return self._var
-00001180: 6961 626c 6573 2e67 6574 286e 616d 652c  iables.get(name,
-00001190: 204e 6f6e 6529 0d0a 0d0a 2020 2020 6465   None)....    de
-000011a0: 6620 7365 745f 7363 656e 6172 696f 5f73  f set_scenario_s
-000011b0: 6574 7469 6e67 2873 656c 662c 206e 616d  etting(self, nam
-000011c0: 652c 2076 616c 293a 0d0a 2020 2020 2020  e, val):..      
-000011d0: 2020 7365 6c66 2e5f 7661 7269 6162 6c65    self._variable
-000011e0: 735b 6e61 6d65 5d20 3d20 7661 6c0d 0a0d  s[name] = val...
-000011f0: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-00001200: 2020 2020 6465 6620 7363 656e 6172 696f      def scenario
-00001210: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001220: 2022 2222 5265 7475 726e 2074 6865 2063   """Return the c
-00001230: 6f6e 6e65 6374 696f 6e20 746f 204b 6166  onnection to Kaf
-00001240: 6b61 2222 220d 0a20 2020 2020 2020 2072  ka"""..        r
-00001250: 6574 7572 6e20 7365 6c66 2e5f 7661 7269  eturn self._vari
-00001260: 6162 6c65 732e 6765 7428 2751 4741 5445  ables.get('QGATE
-00001270: 5f4b 4146 4b41 272c 204e 6f6e 6529 0d0a  _KAFKA', None)..
-00001280: 0d0a 0d0a                                ....
+000001e0: 0d0a 0d0a 2020 2020 2320 6d61 7820 6275  ....    # max bu
+000001f0: 6e64 6c65 2073 697a 6520 666f 7220 6461  ndle size for da
+00000200: 7461 2069 6e67 6573 7469 6f6e 0d0a 2020  ta ingestion..  
+00000210: 2020 4d41 585f 4255 4e44 4c45 203d 2031    MAX_BUNDLE = 1
+00000220: 3030 3030 0d0a 2020 2020 4d49 4e5f 4255  0000..    MIN_BU
+00000230: 4e44 4c45 203d 2031 3030 0d0a 0d0a 2020  NDLE = 100....  
+00000240: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00000250: 656c 662c 206d 6c72 756e 5f65 6e76 5f66  elf, mlrun_env_f
+00000260: 696c 653a 206c 6973 745b 7374 725d 2c20  ile: list[str], 
+00000270: 6461 7461 7365 745f 6e61 6d65 203d 204e  dataset_name = N
+00000280: 6f6e 652c 2068 6172 645f 7661 7269 6162  one, hard_variab
+00000290: 6c65 733a 2064 6963 743d 4e6f 6e65 293a  les: dict=None):
+000002a0: 0d0a 2020 2020 2020 2020 2222 2244 6566  ..        """Def
+000002b0: 696e 6520 7365 7474 696e 6720 666f 7220  ine setting for 
+000002c0: 7465 7374 696e 670d 0a0d 0a20 2020 2020  testing....     
+000002d0: 2020 203a 7061 7261 6d20 6d6c 7275 6e5f     :param mlrun_
+000002e0: 656e 765f 6669 6c65 3a20 206c 6973 7420  env_file:  list 
+000002f0: 6f66 202a 2e65 6e76 2066 696c 6573 2c20  of *.env files, 
+00000300: 6669 7273 7420 7661 6c69 6420 6669 6c65  first valid file
+00000310: 2077 696c 6c20 6265 0d0a 2020 2020 2020   will be..      
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2020 2020 2020 7573 6564 2065            used e
+00000340: 2e67 2e20 5b22 7167 6174 652d 736c 6e2d  .g. ["qgate-sln-
+00000350: 6d6c 7275 6e2d 7072 6976 6174 652e 656e  mlrun-private.en
+00000360: 7622 2c20 2271 6761 7465 2d73 6c6e 2d6d  v", "qgate-sln-m
+00000370: 6c72 756e 2e65 6e76 225d 0d0a 2020 2020  lrun.env"]..    
+00000380: 2020 2020 3a70 6172 616d 2064 6174 6173      :param datas
+00000390: 6574 5f6e 616d 653a 2020 2020 6e61 6d65  et_name:    name
+000003a0: 206f 6620 6461 7461 2073 6574 2065 2e67   of data set e.g
+000003b0: 2e20 2230 312d 7369 7a65 2d31 3030 220d  . "01-size-100".
+000003c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000003d0: 6861 7264 5f76 6172 6961 626c 6573 3a20  hard_variables: 
+000003e0: 206e 6577 206f 7220 7265 706c 6163 656d   new or replacem
+000003f0: 656e 7420 6f66 2076 6172 6961 626c 6573  ent of variables
+00000400: 2066 726f 6d20 2a2e 656e 7620 6669 6c65   from *.env file
+00000410: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00000420: 2020 2020 2020 2023 2073 6574 2076 6172         # set var
+00000430: 6961 626c 6573 2062 6173 6564 206f 6e20  iables based on 
+00000440: 656e 7669 726f 6e6d 656e 7420 6669 6c65  environment file
+00000450: 730d 0a20 2020 2020 2020 2066 6f72 2065  s..        for e
+00000460: 6e76 5f66 696c 6520 696e 206d 6c72 756e  nv_file in mlrun
+00000470: 5f65 6e76 5f66 696c 653a 0d0a 2020 2020  _env_file:..    
+00000480: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+00000490: 7468 2e69 7366 696c 6528 656e 765f 6669  th.isfile(env_fi
+000004a0: 6c65 293a 0d0a 2020 2020 2020 2020 2020  le):..          
+000004b0: 2020 2020 2020 7365 6c66 2e5f 7661 7269        self._vari
+000004c0: 6162 6c65 733d 6d6c 7275 6e2e 7365 745f  ables=mlrun.set_
+000004d0: 656e 765f 6672 6f6d 5f66 696c 6528 656e  env_from_file(en
+000004e0: 765f 6669 6c65 2c20 7265 7475 726e 5f64  v_file, return_d
+000004f0: 6963 743d 5472 7565 290d 0a20 2020 2020  ict=True)..     
+00000500: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00000510: 0d0a 0d0a 2020 2020 2020 2020 2320 7075  ....        # pu
+00000520: 7368 2064 6174 6173 6574 206e 616d 650d  sh dataset name.
+00000530: 0a20 2020 2020 2020 2069 6620 6461 7461  .        if data
+00000540: 7365 745f 6e61 6d65 3a0d 0a20 2020 2020  set_name:..     
+00000550: 2020 2020 2020 2073 656c 662e 5f76 6172         self._var
+00000560: 6961 626c 6573 5b22 5147 4154 455f 4441  iables["QGATE_DA
+00000570: 5441 5345 5422 5d20 3d20 6461 7461 7365  TASET"] = datase
+00000580: 745f 6e61 6d65 0d0a 0d0a 2020 2020 2020  t_name....      
+00000590: 2020 2320 6372 6561 7465 206e 6577 206f    # create new o
+000005a0: 7220 7265 7772 6974 6520 7661 7269 6162  r rewrite variab
+000005b0: 6c65 730d 0a20 2020 2020 2020 2069 6620  les..        if 
+000005c0: 6861 7264 5f76 6172 6961 626c 6573 3a0d  hard_variables:.
+000005d0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000005e0: 206b 6579 2069 6e20 6861 7264 5f76 6172   key in hard_var
+000005f0: 6961 626c 6573 2e6b 6579 7328 293a 0d0a  iables.keys():..
+00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000610: 7365 6c66 2e5f 7661 7269 6162 6c65 735b  self._variables[
+00000620: 6b65 795d 3d68 6172 645f 7661 7269 6162  key]=hard_variab
+00000630: 6c65 735b 6b65 795d 0d0a 0d0a 2020 2020  les[key]....    
+00000640: 2020 2020 7365 6c66 2e5f 7661 7269 6162      self._variab
+00000650: 6c65 735b 2244 4952 225d 3d6f 732e 6765  les["DIR"]=os.ge
+00000660: 7463 7764 2829 0d0a 0d0a 2020 2020 2020  tcwd()....      
+00000670: 2020 2320 6d6f 6465 6c20 6465 6669 6e69    # model defini
+00000680: 7469 6f6e 2073 6574 7469 6e67 0d0a 2020  tion setting..  
+00000690: 2020 2020 2020 7365 6c66 2e5f 6d6f 6465        self._mode
+000006a0: 6c5f 6465 6669 6e69 7469 6f6e 5f73 6574  l_definition_set
+000006b0: 7469 6e67 3d7b 7d0d 0a20 2020 2020 2020  ting={}..       
+000006c0: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
+000006d0: 7468 2e6a 6f69 6e28 7365 6c66 2e6d 6f64  th.join(self.mod
+000006e0: 656c 5f64 6566 696e 6974 696f 6e2c 2022  el_definition, "
+000006f0: 3031 2d6d 6f64 656c 222c 2022 6d6f 6465  01-model", "mode
+00000700: 6c2e 6a73 6f6e 2229 2c20 2272 2229 2061  l.json"), "r") a
+00000710: 7320 6a73 6f6e 5f66 696c 653a 0d0a 2020  s json_file:..  
+00000720: 2020 2020 2020 2020 2020 7365 7474 696e            settin
+00000730: 6720 3d20 6a73 6f6e 2e6c 6f61 6428 6a73  g = json.load(js
+00000740: 6f6e 5f66 696c 6529 0d0a 2020 2020 2020  on_file)..      
+00000750: 2020 7365 6c66 2e5f 6d6f 6465 6c5f 6465    self._model_de
+00000760: 6669 6e69 7469 6f6e 5f73 6574 7469 6e67  finition_setting
+00000770: 3d73 6574 7469 6e67 5b22 7370 6563 225d  =setting["spec"]
+00000780: 0d0a 0d0a 2020 2020 6465 6620 5f5f 7374  ....    def __st
+00000790: 725f 5f28 7365 6c66 293a 0d0a 2020 2020  r__(self):..    
+000007a0: 2020 2020 7265 743d 2222 0d0a 2020 2020      ret=""..    
+000007b0: 2020 2020 666f 7220 6b65 7920 696e 2073      for key in s
+000007c0: 656c 662e 5f76 6172 6961 626c 6573 2e6b  elf._variables.k
+000007d0: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+000007e0: 2020 2020 7265 742b 3d6b 6579 2b20 223a      ret+=key+ ":
+000007f0: 2022 2b20 2227 2220 2b20 7374 7228 7365   "+ "'" + str(se
+00000800: 6c66 2e5f 7661 7269 6162 6c65 735b 6b65  lf._variables[ke
+00000810: 795d 2920 2b20 2227 5c6e 220d 0a20 2020  y]) + "'\n"..   
+00000820: 2020 2020 2072 6574 7572 6e20 7265 745b       return ret[
+00000830: 3a2d 315d 0d0a 0d0a 2020 2020 4070 726f  :-1]....    @pro
+00000840: 7065 7274 790d 0a20 2020 2064 6566 2076  perty..    def v
+00000850: 6172 6961 626c 6573 2873 656c 6629 3a0d  ariables(self):.
+00000860: 0a20 2020 2020 2020 2076 6172 6961 626c  .        variabl
+00000870: 655f 6c69 7374 3d5b 5d0d 0a20 2020 2020  e_list=[]..     
+00000880: 2020 2066 6f72 206b 6579 2069 6e20 7365     for key in se
+00000890: 6c66 2e5f 7661 7269 6162 6c65 732e 6b65  lf._variables.ke
+000008a0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+000008b0: 2020 2069 746d 203d 207b 7d0d 0a20 2020     itm = {}..   
+000008c0: 2020 2020 2020 2020 2069 746d 5b27 6b65           itm['ke
+000008d0: 7927 5d3d 6b65 790d 0a20 2020 2020 2020  y']=key..       
+000008e0: 2020 2020 2069 746d 5b27 7661 6c75 6527       itm['value'
+000008f0: 5d3d 7365 6c66 2e5f 7661 7269 6162 6c65  ]=self._variable
+00000900: 735b 6b65 795d 0d0a 2020 2020 2020 2020  s[key]..        
+00000910: 2020 2020 7661 7269 6162 6c65 5f6c 6973      variable_lis
+00000920: 742e 6170 7065 6e64 2869 746d 290d 0a20  t.append(itm).. 
+00000930: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
+00000940: 7269 6162 6c65 5f6c 6973 740d 0a0d 0a20  riable_list.... 
+00000950: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00000960: 2020 6465 6620 7573 6564 5f66 696c 7465    def used_filte
+00000970: 7273 2873 656c 6629 3a0d 0a20 2020 2020  rs(self):..     
+00000980: 2020 2022 2222 4368 6563 6b2c 2069 6620     """Check, if 
+00000990: 736f 6d65 2066 696c 7465 7220 6973 2075  some filter is u
+000009a0: 7365 6422 2222 0d0a 2020 2020 2020 2020  sed"""..        
+000009b0: 6966 2073 656c 662e 6669 6c74 6572 5f73  if self.filter_s
+000009c0: 6365 6e61 7269 6f73 3a0d 0a20 2020 2020  cenarios:..     
+000009d0: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
+000009e0: 6c66 2e66 696c 7465 725f 7363 656e 6172  lf.filter_scenar
+000009f0: 696f 7329 3e30 3a0d 0a20 2020 2020 2020  ios)>0:..       
+00000a00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000a10: 5472 7565 0d0a 2020 2020 2020 2020 6966  True..        if
+00000a20: 2073 656c 662e 6669 6c74 6572 5f70 726f   self.filter_pro
+00000a30: 6a65 6374 733a 0d0a 2020 2020 2020 2020  jects:..        
+00000a40: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00000a50: 6669 6c74 6572 5f70 726f 6a65 6374 7329  filter_projects)
+00000a60: 3e30 3a0d 0a20 2020 2020 2020 2020 2020  >0:..           
+00000a70: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00000a80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000a90: 2046 616c 7365 0d0a 0d0a 2020 2020 4070   False....    @p
+00000aa0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00000ab0: 206d 6f64 656c 5f6f 7574 7075 7428 7365   model_output(se
+00000ac0: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
+00000ad0: 2252 6574 7572 6e20 7468 6520 6d6f 6465  "Return the mode
+00000ae0: 6c20 6f75 7470 7574 2070 6174 6822 2222  l output path"""
+00000af0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000b00: 2073 656c 662e 5f76 6172 6961 626c 6573   self._variables
+00000b10: 2e67 6574 2827 5147 4154 455f 4f55 5450  .get('QGATE_OUTP
+00000b20: 5554 272c 2027 2e2f 6f75 7470 7574 2729  UT', './output')
+00000b30: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+00000b40: 790d 0a20 2020 2064 6566 206d 6f64 656c  y..    def model
+00000b50: 5f64 6566 696e 6974 696f 6e28 7365 6c66  _definition(self
+00000b60: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000b70: 6574 7572 6e20 7468 6520 7061 7468 2074  eturn the path t
+00000b80: 6f20 6d6f 6465 6c20 6465 6669 6e69 7469  o model definiti
+00000b90: 6f6e 2222 220d 0a20 2020 2020 2020 2072  on"""..        r
+00000ba0: 6574 7572 6e20 7365 6c66 2e5f 7661 7269  eturn self._vari
+00000bb0: 6162 6c65 735b 2751 4741 5445 5f44 4546  ables['QGATE_DEF
+00000bc0: 494e 4954 494f 4e27 5d0d 0a0d 0a20 2020  INITION']....   
+00000bd0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00000be0: 6465 6620 6461 7461 7365 745f 6e61 6d65  def dataset_name
+00000bf0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000c00: 2022 2222 5265 7475 726e 2074 6865 2064   """Return the d
+00000c10: 6174 6173 6574 2073 6574 7469 6e67 2222  ataset setting""
+00000c20: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+00000c30: 6e20 7365 6c66 2e5f 7661 7269 6162 6c65  n self._variable
+00000c40: 732e 6765 7428 2251 4741 5445 5f44 4154  s.get("QGATE_DAT
+00000c50: 4153 4554 222c 2022 3031 2d73 697a 652d  ASET", "01-size-
+00000c60: 3130 3022 290d 0a0d 0a20 2020 2040 7072  100")....    @pr
+00000c70: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00000c80: 6669 6c74 6572 5f70 726f 6a65 6374 7328  filter_projects(
+00000c90: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000ca0: 2222 2252 6574 7572 6e20 7468 6520 7072  """Return the pr
+00000cb0: 6f6a 6563 7420 6669 6c74 6572 2073 6574  oject filter set
+00000cc0: 7469 6e67 2222 220d 0a20 2020 2020 2020  ting"""..       
+00000cd0: 2072 6574 7572 6e20 7365 6c66 2e5f 7661   return self._va
+00000ce0: 7269 6162 6c65 732e 6765 7428 2251 4741  riables.get("QGA
+00000cf0: 5445 5f46 494c 5445 525f 5052 4f4a 4543  TE_FILTER_PROJEC
+00000d00: 5453 222c 204e 6f6e 6529 0d0a 0d0a 2020  TS", None)....  
+00000d10: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00000d20: 2064 6566 2066 696c 7465 725f 7363 656e   def filter_scen
+00000d30: 6172 696f 7328 7365 6c66 293a 0d0a 2020  arios(self):..  
+00000d40: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000d50: 7468 6520 7465 7374 2073 6365 6e61 7269  the test scenari
+00000d60: 6f20 6669 6c74 6572 2073 6574 7469 6e67  o filter setting
+00000d70: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00000d80: 7572 6e20 7365 6c66 2e5f 7661 7269 6162  urn self._variab
+00000d90: 6c65 732e 6765 7428 2251 4741 5445 5f46  les.get("QGATE_F
+00000da0: 494c 5445 525f 5343 454e 4152 494f 5322  ILTER_SCENARIOS"
+00000db0: 2c20 4e6f 6e65 290d 0a0d 0a20 2020 2040  , None)....    @
+00000dc0: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00000dd0: 6620 7265 6469 7328 7365 6c66 293a 0d0a  f redis(self):..
+00000de0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00000df0: 6e20 7468 6520 636f 6e6e 6563 7469 6f6e  n the connection
+00000e00: 2074 6f20 5265 6469 7322 2222 0d0a 2020   to Redis"""..  
+00000e10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000e20: 662e 5f76 6172 6961 626c 6573 2e67 6574  f._variables.get
+00000e30: 2827 5147 4154 455f 5245 4449 5327 2c20  ('QGATE_REDIS', 
+00000e40: 4e6f 6e65 290d 0a0d 0a20 2020 2040 7072  None)....    @pr
+00000e50: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00000e60: 6d79 7371 6c28 7365 6c66 293a 0d0a 2020  mysql(self):..  
+00000e70: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000e80: 7468 6520 636f 6e6e 6563 7469 6f6e 2074  the connection t
+00000e90: 6f20 4d79 5371 6c22 2222 0d0a 2020 2020  o MySql"""..    
+00000ea0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00000eb0: 5f76 6172 6961 626c 6573 2e67 6574 2827  _variables.get('
+00000ec0: 5147 4154 455f 4d59 5351 4c27 2c20 4e6f  QGATE_MYSQL', No
+00000ed0: 6e65 290d 0a0d 0a20 2020 2040 7072 6f70  ne)....    @prop
+00000ee0: 6572 7479 0d0a 2020 2020 6465 6620 706f  erty..    def po
+00000ef0: 7374 6772 6573 2873 656c 6629 3a0d 0a20  stgres(self):.. 
+00000f00: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00000f10: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
+00000f20: 746f 2050 6f73 7467 7265 7322 2222 0d0a  to Postgres"""..
+00000f30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000f40: 656c 662e 5f76 6172 6961 626c 6573 2e67  elf._variables.g
+00000f50: 6574 2827 5147 4154 455f 504f 5354 4752  et('QGATE_POSTGR
+00000f60: 4553 272c 204e 6f6e 6529 0d0a 0d0a 2020  ES', None)....  
+00000f70: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
+00000f80: 2064 6566 206b 6166 6b61 2873 656c 6629   def kafka(self)
+00000f90: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+00000fa0: 7475 726e 2074 6865 2063 6f6e 6e65 6374  turn the connect
+00000fb0: 696f 6e20 746f 204b 6166 6b61 2222 220d  ion to Kafka""".
+00000fc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000fd0: 7365 6c66 2e5f 7661 7269 6162 6c65 732e  self._variables.
+00000fe0: 6765 7428 2751 4741 5445 5f4b 4146 4b41  get('QGATE_KAFKA
+00000ff0: 272c 204e 6f6e 6529 0d0a 0d0a 2020 2020  ', None)....    
+00001000: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00001010: 6566 2061 6e6f 6e79 6d5f 6d6f 6465 2873  ef anonym_mode(s
+00001020: 656c 6629 202d 3e20 626f 6f6c 3a0d 0a20  elf) -> bool:.. 
+00001030: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00001040: 2074 6865 2061 6e6f 6e79 6d6f 7573 206d   the anonymous m
+00001050: 6f64 6522 2222 0d0a 2020 2020 2020 2020  ode"""..        
+00001060: 7265 7475 726e 2054 7275 6520 6966 2073  return True if s
+00001070: 656c 662e 5f76 6172 6961 626c 6573 2e67  elf._variables.g
+00001080: 6574 2827 5147 4154 455f 414e 4f4e 594d  et('QGATE_ANONYM
+00001090: 5f4d 4f44 4527 2c20 224f 6666 2229 2e6c  _MODE', "Off").l
+000010a0: 6f77 6572 2829 203d 3d20 226f 6e22 2065  ower() == "on" e
+000010b0: 6c73 6520 4661 6c73 650d 0a0d 0a20 2020  lse False....   
+000010c0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+000010d0: 6465 6620 6373 765f 7365 7061 7261 746f  def csv_separato
+000010e0: 7228 7365 6c66 293a 0d0a 2020 2020 2020  r(self):..      
+000010f0: 2020 7265 7475 726e 2073 656c 662e 5f6d    return self._m
+00001100: 6f64 656c 5f64 6566 696e 6974 696f 6e5f  odel_definition_
+00001110: 7365 7474 696e 675b 2243 5356 5f53 4550  setting["CSV_SEP
+00001120: 4152 4154 4f52 225d 0d0a 0d0a 2020 2020  ARATOR"]....    
+00001130: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00001140: 6566 2063 7376 5f64 6563 696d 616c 2873  ef csv_decimal(s
+00001150: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00001160: 6574 7572 6e20 7365 6c66 2e5f 6d6f 6465  eturn self._mode
+00001170: 6c5f 6465 6669 6e69 7469 6f6e 5f73 6574  l_definition_set
+00001180: 7469 6e67 5b22 4353 565f 4445 4349 4d41  ting["CSV_DECIMA
+00001190: 4c22 5d0d 0a0d 0a20 2020 2064 6566 2067  L"]....    def g
+000011a0: 6574 5f73 6365 6e61 7269 6f5f 7365 7474  et_scenario_sett
+000011b0: 696e 6728 7365 6c66 2c20 6e61 6d65 293a  ing(self, name):
+000011c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000011d0: 2073 656c 662e 5f76 6172 6961 626c 6573   self._variables
+000011e0: 2e67 6574 286e 616d 652c 204e 6f6e 6529  .get(name, None)
+000011f0: 0d0a 0d0a 2020 2020 6465 6620 7365 745f  ....    def set_
+00001200: 7363 656e 6172 696f 5f73 6574 7469 6e67  scenario_setting
+00001210: 2873 656c 662c 206e 616d 652c 2076 616c  (self, name, val
+00001220: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00001230: 2e5f 7661 7269 6162 6c65 735b 6e61 6d65  ._variables[name
+00001240: 5d20 3d20 7661 6c0d 0a0d 0a20 2020 2040  ] = val....    @
+00001250: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00001260: 6620 7363 656e 6172 696f 2873 656c 6629  f scenario(self)
+00001270: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+00001280: 7475 726e 2074 6865 2063 6f6e 6e65 6374  turn the connect
+00001290: 696f 6e20 746f 204b 6166 6b61 2222 220d  ion to Kafka""".
+000012a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000012b0: 7365 6c66 2e5f 7661 7269 6162 6c65 732e  self._variables.
+000012c0: 6765 7428 2751 4741 5445 5f4b 4146 4b41  get('QGATE_KAFKA
+000012d0: 272c 204e 6f6e 6529 0d0a 0d0a 0d0a       ', None)......
```

## qgate_sln_mlrun/version.py

```diff
@@ -1,3 +1,3 @@
 # Store the version here so:
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
```

## qgate_sln_mlrun/ts/tsbase.py

```diff
@@ -160,17 +160,21 @@
     def name(self):
         return self._name
 
     def before(self):
         """One call BEFORE exec all projects for specific TS. It is relevant for data preparation, etc."""
         pass
 
-    def exec(self, project_name):
-        """Execution of test case"""
-        raise NotImplemented()
+    def prj_exec(self, project_name):
+        """Execution of TS for each project."""
+        pass
+
+    def exec(self):
+        """Execution of TS."""
+        pass
 
     def after(self):
         """One call AFTER execute all projects for specific TS. It is relevant for data cleaning, etc."""
         pass
 
     # region TEST_SCENARIOS
     def testscenario_new(self):
```

## qgate_sln_mlrun/ts/tshelper.py

```diff
@@ -15,15 +15,14 @@
         :return:                    None value or collection of items user name, password, host, port and db name
         """
         user_name = host = db = None
         password=""
         port=0
 
         if connection_string:
-            # re.findall(r'\/\/(.*):(.*)@(.*):(.*)/(.*)', connection_string)
             configs = re.findall(r'//(.*):(.*)@(.*):(.*)/(.*)', connection_string)
             if configs and len(configs)>0:
                 config=configs[0]
                 if len(config)>=5:
                     user_name = config[0]
                     password = config[1]
                     host = config[2]
```

## qgate_sln_mlrun/ts/ts01_project/ts101.py

```diff
@@ -1,15 +1,13 @@
 """
   TS101: Create project(s)
 """
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun
 import os
-import json
-import glob
 
 
 class TS101(TSBase):
 
     def __init__(self, solution):
         super().__init__(solution, self.__class__.__name__)
 
@@ -17,15 +15,15 @@
     def desc(self) -> str:
         return "Create project(s)"
 
     @property
     def long_desc(self):
         return "Create project with setting name, description and tags"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create projects based on json definition"""
         desc = self.project_descs[project_name]
         self._create_project(f"{project_name}/*: '{desc[0]}'", project_name, desc[0], desc[1], desc[2])
 
     @TSBase.handler_testcase
     def _create_project(self, testcase_name, name, desc, lbls, kind):
         """Create project"""
```

## qgate_sln_mlrun/ts/ts01_project/ts102.py

```diff
@@ -4,15 +4,15 @@
 
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun
 import os
 import glob
 import shutil
 from qgate_sln_mlrun.setup import ProjectDelete
-from qgate_sln_mlrun.mysqlhelper import MySQLHelper
+from qgate_sln_mlrun.helper.mysqlhelper import MySQLHelper
 
 
 class TS102(TSBase):
 
     def __init__(self, solution):
         super().__init__(solution, self.__class__.__name__)
 
@@ -20,35 +20,39 @@
     def desc(self) -> str:
         return "Delete project(s)"
 
     @property
     def long_desc(self):
         return "Delete project include all contents and targets (such as Parquet/CSV files, etc.)"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """Delete project"""
         self._delete_project(f"{project_name}/*:", project_name)
 
     def after(self):
-        """Delete addition content of project (include output directory, DB content etc.)"""
+        """Delete addition content without relation to one project (include output directory, DB content etc.)"""
 
         # remove data from MySQL
         self._clean_mysql()
 
         # remove files
         self._clean_file()
 
     def _clean_mysql(self):
         # remove content of mysql
 
-        mysql= MySQLHelper(self.setup)
-        mysql.remove_table(MySQLHelper.TABLE_SOURCE_PREFIX)
+        try:
+            mysql = MySQLHelper(self.setup)
+            if mysql.configured:
+                mysql.remove_helper(MySQLHelper.TABLE_SOURCE_PREFIX)
+        except Exception:
+            pass
 
     def _clean_file(self):
-        # remove files (not remove files from today)
+        # remove files from output dir (but not from today)
 
         # (this line generate file prefix for today)
         not_remove = f"qgt-mlrun-{str.replace(self.output.datetime, ':', '-')}".split(" ")[0]
 
         # cleaning/delete other directories in output directory (generated from e.g. CSVTargets)
         dir = os.path.join(os.getcwd(), self.setup.model_output, "*")
         for file in glob.glob(dir):
```

## qgate_sln_mlrun/ts/ts02_feature_set/ts201.py

```diff
@@ -2,15 +2,14 @@
   TS201: Create feature set(s)
 """
 import datetime
 import sqlalchemy
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun.feature_store as fstore
 from mlrun.features import Feature
-from mlrun.data_types.data_types import ValueType
 from mlrun.datastore.targets import RedisNoSqlTarget, ParquetTarget, CSVTarget, SQLTarget, KafkaTarget
 import os
 import json
 import glob
 from qgate_sln_mlrun.ts.tshelper import TSHelper
 
 
@@ -24,15 +23,15 @@
         return "Create feature set(s)"
 
     @property
     def long_desc(self):
         return ("Create feature set with name, description, entities, features and targets. "
                 "Supported these targets off-line 'parquet', 'csv' and the on-line 'redis'.")
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Get or create featuresets"""
 
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
@@ -171,18 +170,18 @@
                                             if_exists="replace",
                                             create_table=True,
                                             primary_key_column=primary_key)
             else:
                 raise ValueError("Missing value for mysql connection, see 'QGATE_POSTGRES'.")
         elif target == "kafka":
             if self.setup.kafka:
-                params=self.setup.kafka.split(',')
-
-                # NOTE: The path contains the Topic name
-                target_provider = KafkaTarget(name=target_name, bootstrap_servers=params[0].strip(), path=params[1].strip())
+                # NOTE: The topic name is combination of project name , feature name and target
+                target_provider = KafkaTarget(name=target_name,
+                                              bootstrap_servers=self.setup.kafka,
+                                              path=f"{project_name}_{featureset_name}_{target_name}")
             else:
                 raise ValueError("Missing value for kafka connection, see 'QGATE_KAFKA'.")
         else:
             # TODO: Add support for other targets
             raise NotImplementedError()
         return target_provider
```

## qgate_sln_mlrun/ts/ts02_feature_set/ts202.py

```diff
@@ -1,11 +1,12 @@
 """
   TS202: Create feature set(s) & Ingest from DataFrame source (one step)
 """
 from qgate_sln_mlrun.ts.tsbase import TSBase
+from qgate_sln_mlrun.setup import Setup
 import mlrun
 from mlrun.data_types.data_types import ValueType
 from qgate_sln_mlrun.ts.ts02_feature_set import ts201
 import os
 import json
 import glob
 import pandas as pd
@@ -20,15 +21,15 @@
     def desc(self) -> str:
         return "Create feature set(s) & Ingest from DataFrame source (in one step)"
 
     @property
     def long_desc(self):
         return ("Create feature set(s) & Ingest from DataFrame source (in one step, without save and load featureset)")
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create featuresets and ingest"""
 
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
@@ -61,15 +62,15 @@
                 for data_frm in pd.read_csv(file,
                                             sep=self.setup.csv_separator,
                                             header="infer",
                                             decimal=self.setup.csv_decimal,
                                             na_filter=False,
                                             compression="gzip",
                                             encoding="utf-8",
-                                            chunksize=10000):
+                                            chunksize=Setup.MAX_BUNDLE):
                     featureset.ingest(data_frm,
                                   # overwrite=False,
                                   return_df=False,
                                   #infer_options=mlrun.data_types.data_types.InferOptions.Null)
                                   infer_options=mlrun.data_types.data_types.InferOptions.default())
                     # TODO: use InferOptions.Null with python 3.10 or focus on WSL
                     # NOTE: option default, change types
```

## qgate_sln_mlrun/ts/ts02_feature_set/ts203.py

```diff
@@ -21,15 +21,15 @@
     def desc(self) -> str:
         return "Create feature set(s) & Ingest from from CSV source (one step)"
 
     @property
     def long_desc(self):
         return ("Create feature set(s) & Ingest from from CSV source (one step, without save and load featureset)")
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create featuresets and ingest"""
 
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
```

## qgate_sln_mlrun/ts/ts02_feature_set/ts204.py

```diff
@@ -21,15 +21,15 @@
     def desc(self) -> str:
         return "Create feature set(s) & Ingest from Parquet source (one step)"
 
     @property
     def long_desc(self):
         return ("Create feature set(s) & Ingest from Parquet source (one step, without save and load featureset)")
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create featuresets and ingest"""
 
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
```

## qgate_sln_mlrun/ts/ts02_feature_set/ts205.py

```diff
@@ -6,15 +6,15 @@
 import mlrun.feature_store as fstore
 from mlrun.data_types.data_types import ValueType
 from mlrun.datastore.sources import SQLSource
 from qgate_sln_mlrun.ts.ts02_feature_set import ts201
 import os
 import json
 import glob
-from qgate_sln_mlrun.mysqlhelper import MySQLHelper
+from qgate_sln_mlrun.helper.mysqlhelper import MySQLHelper
 
 
 class TS205(TSBase):
 
     def __init__(self, solution):
         super().__init__(solution, self.__class__.__name__)
         self._mysql = MySQLHelper(self.setup)
@@ -23,25 +23,25 @@
     def desc(self) -> str:
         return "Create feature set(s) & Ingest from SQL source (one step)"
 
     @property
     def long_desc(self):
         return ("Create feature set(s) & Ingest from SQL (MySQL) source (one step, without save and load featureset)")
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create featuresets & ingest"""
 
         # It can be executed only in case that configuration is fine
         if not self._mysql.configured:
             return
 
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # Create table only in case, that table does not exist
-            if not self._mysql.table_exist(featureset_name):
-                self._mysql.create_table(featureset_name)
+            #if not self._mysql.helper_exist(None, project_name, featureset_name):
+            self._mysql.create_insert_data(project_name, featureset_name, True)
 
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
                                        "02-feature-set",
                                        f"*-{featureset_name}.json")
@@ -64,15 +64,15 @@
 
             keys = ""
             for entity in featureset.spec.entities:
                 keys+=f"{entity.name},"
 
             fstore.ingest(featureset,
                           SQLSource(name="tst",
-                                    table_name=self._mysql.convert_feature_tablename(featureset_name),
+                                    table_name=self._mysql.create_helper(project_name, featureset_name),
                                     db_url=self.setup.mysql,
                                     key_field=keys[:-1].replace('-','_')),
                           # overwrite=False,
                           return_df=False,
                           # infer_options=mlrun.data_types.data_types.InferOptions.Null)
                           infer_options=mlrun.data_types.data_types.InferOptions.default())
             # TODO: use InferOptions.Null with python 3.10 or focus on WSL
```

## qgate_sln_mlrun/ts/ts02_feature_set/ts206.py

```diff
@@ -1,80 +1,73 @@
 """
   TS206: Create feature set(s) & Ingest from Kafka source (one step)
 """
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun
 import mlrun.feature_store as fstore
 from mlrun.data_types.data_types import ValueType
-from mlrun.datastore.sources import SQLSource
+from mlrun.datastore.sources import KafkaSource
 from qgate_sln_mlrun.ts.ts02_feature_set import ts201
 import json
-from qgate_sln_mlrun.mysqlhelper import MySQLHelper
+from qgate_sln_mlrun.helper.kafkahelper import KafkaHelper
+import os
+import glob
 
 
 class TS206(TSBase):
 
     def __init__(self, solution):
         super().__init__(solution, self.__class__.__name__)
-        self._mysql = MySQLHelper(self.setup)
+        self._kafka = KafkaHelper(self.setup)
 
     @property
     def desc(self) -> str:
         return "Create feature set(s) & Ingest from Kafka source (one step)"
 
     @property
     def long_desc(self):
         return ("Create feature set(s) & Ingest from Kafka source (one step, without save and load featureset)")
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create featuresets & ingest"""
-        return
 
-        # # It can be executed only in case that configuration is fine
-        # if not self._mysql.configured:
-        #     return
-        #
-        # for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
-        #     # Create table only in case, that table does not exist
-        #     if not self._mysql.table_exist(featureset_name):
-        #         self._mysql.create_table(featureset_name)
-        #
-        #     # create file with definition of vector
-        #     source_file = os.path.join(os.getcwd(),
-        #                                self.setup.model_definition,
-        #                                "01-model",
-        #                                "02-feature-set",
-        #                                f"*-{featureset_name}.json")
-        #
-        #     for file in glob.glob(source_file):
-        #         # iterate cross all featureset definitions
-        #         with open(file, "r") as json_file:
-        #             self._create_featureset_ingest(f'{project_name}/{featureset_name}', project_name, featureset_name, json_file)
+        # It can be executed only in case that configuration is fine
+        if not self._kafka.configured:
+            return
+
+        for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
+            # Create topic only in case, that topic does not exist
+            helper= self._kafka.create_helper(project_name, featureset_name)
+            #if not self._kafka.helper_exist(helper):
+            self._kafka.create_insert_data(helper, featureset_name,True)
+
+            # create file with definition of vector
+            source_file = os.path.join(os.getcwd(),
+                                       self.setup.model_definition,
+                                       "01-model",
+                                       "02-feature-set",
+                                       f"*-{featureset_name}.json")
+
+            for file in glob.glob(source_file):
+                # iterate cross all featureset definitions
+                with open(file, "r") as json_file:
+                    self._create_featureset_ingest(f'{project_name}/{featureset_name}', project_name, featureset_name, json_file)
 
     @TSBase.handler_testcase
     def _create_featureset_ingest(self, testcase_name, project_name, featureset_name, json_file):
         json_content = json.load(json_file)
         name, desc, lbls, kind = TSBase.get_json_header(json_content)
 
         if kind == "feature-set":
 
             # create feature set based on the logic in TS201
             ts= ts201.TS201(self._solution)
             featureset=ts.create_featureset_content(project_name, f"{self.name}-{name}", desc, json_content['spec'])
 
-            keys = ""
-            for entity in featureset.spec.entities:
-                keys+=f"{entity.name},"
-
-            fstore.ingest(featureset,
-                          SQLSource(name="tst",
-                                    table_name=self._mysql.convert_feature_tablename(featureset_name),
-                                    db_url=self.setup.mysql,
-                                    key_field=keys[:-1].replace('-','_')),
-                          # overwrite=False,
-                          return_df=False,
-                          # infer_options=mlrun.data_types.data_types.InferOptions.Null)
-                          infer_options=mlrun.data_types.data_types.InferOptions.default())
-            # TODO: use InferOptions.Null with python 3.10 or focus on WSL
-            # NOTE: option default, change types
-            # NOTE: option Null, generate error with datetime in python 3.9
 
+            # fstore.ingest(featureset,
+            #               KafkaSource(brokers=self.setup.kafka,
+            #                         topics=[self._kafka.create_helper(project_name, featureset_name)]),
+            #               # overwrite=False,
+            #               return_df=False,
+            #               # infer_options=mlrun.data_types.data_types.InferOptions.Null)
+            #               infer_options=mlrun.data_types.data_types.InferOptions.default())
```

## qgate_sln_mlrun/ts/ts03_ingest_data/ts302.py

```diff
@@ -1,12 +1,13 @@
 """
   TS302: Ingest data to feature set(s) from DataFrame Source
 """
 
 from qgate_sln_mlrun.ts.tsbase import TSBase
+from qgate_sln_mlrun.setup import Setup
 import mlrun
 import mlrun.feature_store as fstore
 from mlrun.data_types.data_types import spark_to_value_type
 import pandas as pd
 import glob
 import os
 
@@ -24,15 +25,15 @@
     def long_desc(self):
         return "Ingest data to feature set(s) from Pandas DataFrame source"
 
     def prepare(self):
         """Prepare data for ingestion"""
         pass
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """Data ingest"""
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create possible file for load
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "02-data",
                                        self.setup.dataset_name,
@@ -45,20 +46,20 @@
     @TSBase.handler_testcase
     def _ingest_data(self, testcase_name, project_name, featureset_name, file):
         # get existing feature set (feature set have to be created in previous test scenario)
         featureset = fstore.get_feature_set(f"{project_name}/{featureset_name}")
 
         # ingest data with bundl/chunk
         for data_frm in pd.read_csv(file,
-                                    sep=self.setup.csv_separator,       #";",
+                                    sep=self.setup.csv_separator,
                                     header="infer",
-                                    decimal=self.setup.csv_decimal,     #",",
+                                    decimal=self.setup.csv_decimal,
                                     compression="gzip",
                                     encoding="utf-8",
-                                    chunksize=10000):
+                                    chunksize=Setup.MAX_BUNDLE):
             featureset.ingest(data_frm,
                           # overwrite=False,
                           return_df=False,
                           #infer_options=mlrun.data_types.data_types.InferOptions.Null)
                           infer_options=mlrun.data_types.data_types.InferOptions.default())
             # TODO: use InferOptions.Null with python 3.10 or focus on WSL
             # NOTE: option default, change types
```

## qgate_sln_mlrun/ts/ts03_ingest_data/ts303.py

```diff
@@ -20,15 +20,15 @@
     def desc(self) -> str:
         return "Ingest data to feature set(s) from CSV source "
 
     @property
     def long_desc(self):
         return "Ingest data to feature set(s) from CSV source"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """Data ingest"""
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create possible file for load
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "02-data",
                                        self.setup.dataset_name,
```

## qgate_sln_mlrun/ts/ts03_ingest_data/ts304.py

```diff
@@ -3,15 +3,14 @@
 """
 
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun
 import mlrun.feature_store as fstore
 from mlrun.data_types.data_types import spark_to_value_type
 from mlrun.datastore.sources import ParquetSource
-import pandas as pd
 import glob
 import os
 
 
 class TS304(TSBase):
 
     def __init__(self, solution):
@@ -21,15 +20,15 @@
     def desc(self) -> str:
         return "Ingest data to feature set(s) from Parquet source "
 
     @property
     def long_desc(self):
         return "Ingest data to feature set(s) from Parquet source"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """Data ingest"""
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # create possible file for load
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "02-data",
                                        self.setup.dataset_name,
```

## qgate_sln_mlrun/ts/ts03_ingest_data/ts305.py

```diff
@@ -4,18 +4,17 @@
 
 
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun
 import mlrun.feature_store as fstore
 from mlrun.data_types.data_types import spark_to_value_type
 from mlrun.datastore.sources import SQLSource
-import pandas as pd
 import glob
 import os
-from qgate_sln_mlrun.mysqlhelper import MySQLHelper
+from qgate_sln_mlrun.helper.mysqlhelper import MySQLHelper
 
 
 class TS305(TSBase):
 
     def __init__(self, solution):
         super().__init__(solution, self.__class__.__name__)
         self._mysql = MySQLHelper(self.setup)
@@ -24,25 +23,25 @@
     def desc(self) -> str:
         return "Ingest data to feature set(s) from SQL source"
 
     @property
     def long_desc(self):
         return "Create feature set(s) & Ingest from SQL (MySQL) source"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """ Create featuresets & ingest"""
 
         # It can be executed only in case that configuration is fine
         if not self._mysql.configured:
             return
 
         for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
             # Create table only in case, that table does not exist
-            if not self._mysql.table_exist(featureset_name):
-                self._mysql.create_table(featureset_name)
+            #if not self._mysql.helper_exist(None, project_name, featureset_name):
+            self._mysql.create_insert_data(project_name, featureset_name, True)
 
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
                                        "02-feature-set",
                                        f"*-{featureset_name}.json")
@@ -59,15 +58,15 @@
 
         keys = ""
         for entity in featureset.spec.entities:
             keys+=f"{entity.name},"
 
         fstore.ingest(featureset,
                       SQLSource(name="tst",
-                                table_name=self._mysql.convert_feature_tablename(featureset_name),
+                                table_name=self._mysql.create_helper(project_name, featureset_name),
                                 db_url=self.setup.mysql,
                                 key_field=keys[:-1].replace('-','_')),
                       # overwrite=False,
                       return_df=False,
                       # infer_options=mlrun.data_types.data_types.InferOptions.Null)
                       infer_options=mlrun.data_types.data_types.InferOptions.default())
         # TODO: use InferOptions.Null with python 3.10 or focus on WSL
```

## qgate_sln_mlrun/ts/ts04_feature_vector/ts401.py

```diff
@@ -18,15 +18,15 @@
     def desc(self) -> str:
         return "Create feature vector(s)"
 
     @property
     def long_desc(self):
         return "Create feature vectors as join of relevant feature sets"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """Create feature vectors"""
         # https://docs.mlrun.org/en/latest/api/mlrun.feature_store.html#mlrun.feature_store.FeatureVector
 
         for featurevector_name in self.get_featurevectors(self.project_specs.get(project_name)):
             # create file with definition of vector
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
```

## qgate_sln_mlrun/ts/ts05_get_data/ts501.py

```diff
@@ -15,15 +15,15 @@
     def desc(self) -> str:
         return "Get data from off-line feature vector(s)"
 
     @property
     def long_desc(self):
         return "Get data from off-line feature vector"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """
         Get data from off-line feature vector
         """
         for featurevector_name in self.get_featurevectors(self.project_specs.get(project_name)):
             self._get_data_offline(f"{project_name}/{featurevector_name}", project_name, featurevector_name)
```

## qgate_sln_mlrun/ts/ts05_get_data/ts502.py

```diff
@@ -17,15 +17,15 @@
     def desc(self) -> str:
         return "Get data from on-line feature vector(s)"
 
     @property
     def long_desc(self):
         return "Get data from on-line feature vector(s), focus on target Redis"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """
         Get data from on-line feature vector
         """
         # get information, about list of on-line vectors
         vectors = None
         if self.test_setting.get('vector'):
             if self.test_setting['vector'].get('online'):
```

## qgate_sln_mlrun/ts/ts06_pipeline/ts601.py

```diff
@@ -1,67 +1,87 @@
 """
-  TS601: Simple pipeline(s) (HTTP call)
+  TS601: Simple pipeline(s)
 """
 
 from qgate_sln_mlrun.ts.tsbase import TSBase
+from qgate_sln_mlrun.setup import Setup
 import mlrun.feature_store as fstore
 import mlrun
 import pandas as pd
 import glob
 import os
 
 
 class TS601(TSBase):
 
     def __init__(self, solution):
         super().__init__(solution, self.__class__.__name__)
 
     @property
     def desc(self) -> str:
-        return "Simple pipeline(s) (HTTP call)"
+        return "Simple pipeline(s)"
 
     @property
     def long_desc(self):
-        return "Simple pipeline(s) in project (access via HTTP call)"
+        return "Simple pipeline(s), focus on full/partial event and tests under the Mock"
 
-    def exec(self, project_name):
+    def exec(self):
         """Simple pipeline during ingest"""
-        return
-
-        for featureset_name in self.get_featuresets(self.project_specs.get(project_name)):
-            # create possible file for load
-            source_file = os.path.join(os.getcwd(),
-                                       self.setup.model_definition,
-                                       "02-data",
-                                       self.setup.dataset_name,
-                                       f"*-{featureset_name}.csv.gz")
-
-            # check existing data set
-            for file in glob.glob(source_file):
-                self._ingest_data(f"{project_name}/{featureset_name}", project_name, featureset_name, file)
+        self._class_plus(f"*/class_plus (event)", True)
+        self._class_plus(f"*/class_plus", False)
+        self._class_multipl(f"*/class_multipl (event)", True)
+        self._class_multipl(f"*/class_multipl", False)
+        self._minus(f"*/minus (event)", True)
+        self._minus(f"*/minus", False)
 
     @TSBase.handler_testcase
-    def _ingest_data(self, testcase_name, project_name, featureset_name, file):
-        # get existing feature set (feature set have to be created in previous test scenario)
-        featureset = fstore.get_feature_set(f"{project_name}/{featureset_name}")
-
-        #quotes_set.graph.to("storey.Filter", "filter", _fn="(event['bid'] > 50)")
-        #https://docs.mlrun.org/en/latest/serving/getting-started.html
+    def _class_plus(self, testcase_name, full_event):
+
+        func = mlrun.code_to_function(f"ts601_fn",
+                                      kind="serving",
+                                      filename="./qgate_sln_mlrun/ts/ts06_pipeline/ts601_ext_code.py")
+        graph_echo = func.set_topology("flow")
+        graph_echo.to(class_name="TS601Pipeline", full_event=full_event, name="plus", default=True).respond()
+
+        # tests
+        echo_server = func.to_mock_server(current_function="*")
+        result = echo_server.test("", {"a": 5, "b": 7})
+        echo_server.wait_for_completion()
+
+        # value check
+        if result['calc']!=12:
+            raise ValueError("Invalid calculation, expected value 12")
 
+    @TSBase.handler_testcase
+    def _class_multipl(self, testcase_name, full_event):
 
+        func = mlrun.code_to_function(f"ts601_fn",
+                                      kind="serving",
+                                      filename="./qgate_sln_mlrun/ts/ts06_pipeline/ts601_ext_code.py")
+        graph_echo = func.set_topology("flow")
+        graph_echo.to(class_name="TS601Pipeline", full_event=full_event, name="multipl", default=True).respond()
+
+        # tests
+        echo_server = func.to_mock_server(current_function="*")
+        result = echo_server.test("", {"a": 5, "b": 7})
+        echo_server.wait_for_completion()
+
+        # value check
+        if result['calc']!=35:
+            raise ValueError("Invalid calculation, expected value 35")
 
-        # ingest data with bundl/chunk
-        for data_frm in pd.read_csv(file,
-                                    sep=self.setup.csv_separator,       #";",
-                                    header="infer",
-                                    decimal=self.setup.csv_decimal,     #",",
-                                    compression="gzip",
-                                    encoding="utf-8",
-                                    chunksize=10000):
-            featureset.ingest(data_frm,
-                          # overwrite=False,
-                          return_df=False,
-                          #infer_options=mlrun.data_types.data_types.InferOptions.Null)
-                          infer_options=mlrun.data_types.data_types.InferOptions.default())
-            # TODO: use InferOptions.Null with python 3.10 or focus on WSL
-            # NOTE: option default, change types
-            # NOTE: option Null, generate error with datetime in python 3.9
+    @TSBase.handler_testcase
+    def _minus(self, testcase_name, full_event):
+        func = mlrun.code_to_function(f"ts601_fn",
+                                      kind="serving",
+                                      filename="./qgate_sln_mlrun/ts/ts06_pipeline/ts601_ext_code.py")
+        graph_echo = func.set_topology("flow")
+        graph_echo.to(handler="minus" , full_event=full_event, name="minus", default=True).respond()
+
+        # tests
+        echo_server = func.to_mock_server(current_function="*")
+        result = echo_server.test("", {"a": 10, "b": 7})
+        echo_server.wait_for_completion()
+
+        # value check
+        if result['calc']!=3:
+            raise ValueError("Invalid calculation, expected value 3")
```

## qgate_sln_mlrun/ts/ts07_build_model/ts701.py

```diff
@@ -1,18 +1,16 @@
 """
   TS701: Build CART model (based on off-line feature vector)
 """
 from sklearn.preprocessing import LabelEncoder
 from qgate_sln_mlrun.ts.tsbase import TSBase
 import mlrun.feature_store as fstore
 import mlrun
-import pandas as pd
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.model_selection import train_test_split
-from sklearn import metrics
 import os
 import glob
 import json
 from pickle import dumps
 
 
 class TS701(TSBase):
@@ -29,15 +27,15 @@
         """
         Long description, more information see these sources:
          - https://www.datacamp.com/tutorial/decision-tree-classification-python
          - https://scikit-learn.org/stable/modules/tree.html
         """
         return "Build CART model (Classification and Regression Tree) from Scikit-Learn"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
 
         # Get list of ml models
         for mlmodel_name in self.get_mlmodel(self.project_specs.get(project_name)):
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
                                        "04-ml-model",
```

## qgate_sln_mlrun/ts/ts08_serve_model/ts801.py

```diff
@@ -1,19 +1,15 @@
 """
   TS801: Serving score from CART (with usage of off-line feature vector)
 """
 
 from qgate_sln_mlrun.ts.tsbase import TSBase
 from pickle import load
-from mlrun.datastore import DataItem
 from mlrun.artifacts import get_model, update_model
 import mlrun
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.model_selection import train_test_split
-from sklearn import metrics
 import mlrun.feature_store as fstore
 from sklearn.preprocessing import LabelEncoder
 import os
 import glob
 import json
 
 class TS801(TSBase):
@@ -30,15 +26,15 @@
         """
         Long description, more information see these sources:
          - https://www.datacamp.com/tutorial/decision-tree-classification-python
          - https://scikit-learn.org/stable/modules/tree.html
         """
         return "Serving score from CART (Classification and Regression Tree) from Scikit-Learn"
 
-    def exec(self, project_name):
+    def prj_exec(self, project_name):
         """
         Serve score
         """
         for mlmodel_name in self.get_mlmodel(self.project_specs.get(project_name)):
             source_file = os.path.join(os.getcwd(),
                                        self.setup.model_definition,
                                        "01-model",
```

## Comparing `qgate_sln_mlrun/mysqlhelper.py` & `qgate_sln_mlrun/helper/mysqlhelper.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import os
 import glob
 import json
 import pandas as pd
 from qgate_sln_mlrun.ts.tsbase import TSBase
 from qgate_sln_mlrun.ts.tshelper import TSHelper
 from qgate_sln_mlrun.setup import Setup
+from qgate_sln_mlrun.helper.basehelper import BaseHelper
 
 
-class MySQLHelper():
+class MySQLHelper(BaseHelper):
 
     # Prefix of table with sources
     TABLE_SOURCE_PREFIX = "tmp_"
 
     def __init__(self,setup: Setup):
         self._setup = setup
 
@@ -21,16 +22,20 @@
         return self._setup
 
     @property
     def configured(self):
         """Return None if not configured or connection string (based on setting QGATE_MYSQL in *.env file)."""
         return self.setup.mysql
 
-    def create_table(self, featureset_name, drop_table_if_exist = False):
-        """Create table"""
+    @property
+    def prefix(self):
+        return MySQLHelper.TABLE_SOURCE_PREFIX
+
+    def create_insert_data(self, helper, featureset_name, drop_if_exist = False):
+        """Create table and insert data"""
         primary_keys=""
         column_types= ""
         columns = ""
 
         source_file = os.path.join(os.getcwd(),
                                    self.setup.model_definition,
                                    "01-model",
@@ -54,15 +59,14 @@
                     primary_keys += f"{item['name']},"
 
                 # columns
                 for item in json_spec['features']:
                     columns += f"{item['name']},"
                     column_types+= f"{item['name']} {TSHelper.type_to_mysql_type(item['type'])},"
 
-        table_name = self.convert_feature_tablename(featureset_name)
         column_types = column_types[:-1].replace('-', '_')
         primary_keys = primary_keys[:-1].replace('-','_')
         columns = columns[:-1].replace('-', '_')
 
         # connect
         user_name, password, host, port, db = TSHelper.split_sqlalchemy_connection(self.setup.mysql)
         connection = pymysql.connect(host=host,
@@ -71,27 +75,27 @@
                                      password=password,
                                      database=db,
                                      cursorclass=pymysql.cursors.DictCursor)
 
         with connection:
             with connection.cursor() as cursor:
 
-                if drop_table_if_exist:
+                if drop_if_exist:
                     # drop table
-                    cursor.execute(f"DROP TABLE IF EXISTS {table_name};")
+                    cursor.execute(f"DROP TABLE IF EXISTS {helper};")
                     connection.commit()
 
                 # create table
-                cursor.execute(f"CREATE TABLE {table_name} ({column_types});")
+                cursor.execute(f"CREATE TABLE {helper} ({column_types});")
                 connection.commit()
 
                 # insert data
-                self._insert_into(connection, cursor, table_name, featureset_name, columns)
+                self._insert_into(connection, cursor, helper, featureset_name, columns)
 
-    def _insert_into(self, connection, cursor, table_name, featureset_name, columns):
+    def _insert_into(self, connection, cursor, helper, featureset_name, columns):
         """Insert data into the table"""
 
         # create possible file for load
         source_file = os.path.join(os.getcwd(),
                                    self.setup.model_definition,
                                    "02-data",
                                    self.setup.dataset_name,
@@ -101,55 +105,47 @@
             # ingest data with bundl/chunk
             for data_frm in pd.read_csv(file,
                                         sep=self.setup.csv_separator,  # ";",
                                         header="infer",
                                         decimal=self.setup.csv_decimal,  # ",",
                                         compression="gzip",
                                         encoding="utf-8",
-                                        chunksize=10000):
+                                        chunksize=Setup.MAX_BUNDLE):
                 for row in data_frm.to_numpy().tolist():
                     values=f"\",\"".join(str(e) for e in row)
 
-                    cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES(\"{values}\");")
+                    cursor.execute(f"INSERT INTO {helper} ({columns}) VALUES(\"{values}\");")
                 connection.commit()
 
-    def convert_feature_tablename(self, featureset_name):
-        """Convert featureset name to the name of table.
-
-        :param featureset_name:     Feature set name
-        :return:                    The name of db table with relevant prefix
-        """
-        return f"{MySQLHelper.TABLE_SOURCE_PREFIX}{featureset_name}".replace('-', '_')
-
-    def table_exist(self, featureset_name):
-        """Check, if table exists
+    def helper_exist(self, helper):
+        """Check, if helper exists
 
-        :param table_name:      name of the table for check
-        :return:                True - table exist, False - table does not exist
+        :param helper:              topic name
+        :return:                    True - table exist, False - table does not exist
         """
         user_name, password, host, port, db = TSHelper.split_sqlalchemy_connection(self.setup.mysql)
         connection = pymysql.connect(host=host,
                                      port=port,
                                      user=user_name,
                                      password=password,
                                      database=db,
                                      cursorclass=pymysql.cursors.DictCursor)
 
         with connection:
             with connection.cursor() as cursor:
                 cursor.execute(f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{db}'"
-                               f" AND table_name = '{self.convert_feature_tablename(featureset_name)}' LIMIT 1;")
+                               f" AND table_name = '{helper}' LIMIT 1;")
                 myresult = cursor.fetchone()
                 if myresult:
                     if len(myresult)>0:
                         return True
         return False
 
-    def remove_table(self, start_with):
-        """Remove tables with specific prefix
+    def remove_helper(self, start_with):
+        """Remove helper with specific prefix
 
         :param start_with:      prefix of tables for remove
         """
         if start_with:
             user_name, password, host, port, db = TSHelper.split_sqlalchemy_connection(self.setup.mysql)
             connection = pymysql.connect(host=host,
                                          port=port,
```

## Comparing `qgate_sln_mlrun-0.2.3.dist-info/LICENSE` & `qgate_sln_mlrun-0.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_sln_mlrun-0.2.3.dist-info/METADATA` & `qgate_sln_mlrun-0.2.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate_sln_mlrun
-Version: 0.2.3
+Version: 0.2.4
 Summary: The quality gate for testing MLRun/Iguazio solution.
 Author-email: Jiri Steuer <steuer.jiri@gmail.com>
 Maintainer-email: Jiri Steuer <steuer.jiri@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/george0st/qgate-sln-mlrun/
 Project-URL: repository, https://pypi.org/project/qgate-sln-mlrun/
 Keywords: testing,data-science,machine-learning,quality-assurance,quality-assessment,iguazio,mlrun,mlops,quality-gate,feature-store
@@ -79,31 +79,30 @@
    - ✅ TS202: Create feature set(s) & Ingest from DataFrame source (one step)
    - ✅ TS203: Create feature set(s) & Ingest from CSV source (one step) 
    - ✅ TS204: Create feature set(s) & Ingest from Parquet source (one step)
    - ✅ TS205: Create feature set(s) & Ingest from SQL source (one step)
    - ✔  TS206: Create feature set(s) & Ingest from Kafka source (one step)
    - ❌ TS207: Create feature set(s) & Ingest from HTTP source (one step)
  - **03 - Ingest data**
-   - ✔  TS301: Ingest data (Preview)
+   - ✅ TS301: Ingest data (Preview mode)
    - ✅ TS302: Ingest data to feature set(s) from DataFrame source
    - ✅ TS303: Ingest data to feature set(s) from CSV source 
    - ✅ TS304: Ingest data to feature set(s) from Parquet source
    - ✅ TS305: Ingest data to feature set(s) from SQL source
    - ✔  TS306: Ingest data to feature set(s) from Kafka source
    - ❌ TS307: Ingest data to feature set(s) from HTTP source
  - **04 - Feature vector**
    - ✅ TS401: Create feature vector(s)
  - **05 - Get data from vector**
    - ✅ TS501: Get data from off-line feature vector(s)
    - ✅ TS502: Get data from on-line feature vector(s)
  - **06 - Pipeline**
-   - ✔ TS601: Simple pipeline(s) (HTTP call)
-   - ❌ TS602: Simple pipeline for CSV source
-   - ❌ TS603: Complex pipeline for DataFrame source
-   - ❌ TS604: Complex pipeline for CSV source
+   - ✅ TS601: Simple pipeline(s)
+   - ✅ TS602: Complex pipeline(s)
+   - ✔ TS602: Complex mass pipeline(s)
  - **07 - Build model**
    - ✅ TS701: Build CART model
    - ❌ TS702: Build XGBoost model
    - ❌ TS703: Build DNN model
  - **08 - Serve model**
    - ✅ TS801: Serving score from CART
    - ❌ TS802: Serving score from XGBoost
```

## Comparing `qgate_sln_mlrun-0.2.3.dist-info/RECORD` & `qgate_sln_mlrun-0.2.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 qgate_sln_mlrun/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
-qgate_sln_mlrun/mysqlhelper.py,sha256=UFEZoi_vyTM63Fqm0CyvDN0-nZal72nmObYqmkKmlv8,7261
 qgate_sln_mlrun/output.py,sha256=aHBr5-1yfoxe25Wi5gusUROpnQRPx92l0IeYRVscKk0,9317
-qgate_sln_mlrun/qualityreport.py,sha256=MmPIzdzN904xlphmvaTpRoUanPTPB69gumJk_-foRhw,9731
-qgate_sln_mlrun/setup.py,sha256=eCMK533ZhQ8h974UtDr1Yoh-I6K5nR6Ryd6dZOYC1wg,4740
-qgate_sln_mlrun/version.py,sha256=DQTxpor0VJd5ua1riFIi1Oxym5B2ZPM4o31joBSO0cU,53
+qgate_sln_mlrun/qualityreport.py,sha256=cs6go9WFBTlkVI7f3kqXXGKghbDMZuklnOiHFIwJM1k,10021
+qgate_sln_mlrun/setup.py,sha256=46edxA8_OkBEGFnCPkjMoasZgMJdMJkR6KhvIOxNgjc,4830
+qgate_sln_mlrun/version.py,sha256=pjmpJFFkVHN9jckxLO3VN_4z6rnl_zDt1sGe481npgo,53
+qgate_sln_mlrun/helper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+qgate_sln_mlrun/helper/basehelper.py,sha256=Wask9vAiyqRy1OVkJmd7Ggr-njMvfQ4qNC39nZV-WDs,872
+qgate_sln_mlrun/helper/kafkahelper.py,sha256=iQWRk-yXM8JIEoEvAtKlIvHhek9G4eKrHowqblxmIRw,5488
+qgate_sln_mlrun/helper/mysqlhelper.py,sha256=ZZPQ5vjcOZvY78L9HSM-dxISzhqOeA1pOTyU18dgvwU,6945
 qgate_sln_mlrun/model_changes/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
 qgate_sln_mlrun/model_changes/empty-template.json,sha256=tOp6llKrzwGv-rlSvaaNjaXYGY96JlJ_V3p8sD2igpw,312
 qgate_sln_mlrun/templates/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
 qgate_sln_mlrun/templates/qgt-mlrun.html,sha256=2UFIfZG3SQQ1DKofSw42EuVeB5m30R_4Y-4yOC9td4M,10411
 qgate_sln_mlrun/templates/qgt-mlrun.txt,sha256=AFIR9XATOAunaROKLD2o8hXYYgSkJ0pHBetHzt1uQaY,1468
 qgate_sln_mlrun/ts/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/tsbase.py,sha256=KOl-5HoDCbTF090eLm-TyO7JBiKEDe1wUWWuMU9x8OY,5702
-qgate_sln_mlrun/ts/tshelper.py,sha256=VwM6USYzLIocdK4wMCc1stF0xuDE5VBRQ-Kh_kC0afA,4199
+qgate_sln_mlrun/ts/tsbase.py,sha256=_3NnF2BjSVQVIpAn9tlDaGwFghbSQH9kOODTolgCXMk,5768
+qgate_sln_mlrun/ts/tshelper.py,sha256=UMnMLvsZ4PH4CSjN0171sUwrqYb9orzUhoX-XaI_uMM,4121
 qgate_sln_mlrun/ts/ts01_project/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts01_project/ts101.py,sha256=ezfjK-5phcB7UAsbCuZRvtHA_bGnq1DacNKAACE5T6E,1122
-qgate_sln_mlrun/ts/ts01_project/ts102.py,sha256=obxhe5md8293-cmfTLMqRUr30hHtazwcdAtRHG-_aLY,2474
+qgate_sln_mlrun/ts/ts01_project/ts101.py,sha256=axfwD7RQ7l7_MygiQJDDzuRGP0sd1wzXOqsnh4Ispf8,1100
+qgate_sln_mlrun/ts/ts01_project/ts102.py,sha256=y8cGkaX_j_n2lNzkQPP6ColmNDyCRN85YnouqesYo90,2620
 qgate_sln_mlrun/ts/ts02_feature_set/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts02_feature_set/ts201.py,sha256=S-mOd_QWCJQww_WZGZFoRWySi9Ogb3viEV1UdQKezDI,9137
-qgate_sln_mlrun/ts/ts02_feature_set/ts202.py,sha256=GttCHgb1XeoW2sTi-2agqslS_02dHjHM4U2guW-d6UA,3530
-qgate_sln_mlrun/ts/ts02_feature_set/ts203.py,sha256=P3kux4vG9cxYjdbdo1Hj-FEX-BFjtbuaDkZhAHtaFmM,3043
-qgate_sln_mlrun/ts/ts02_feature_set/ts204.py,sha256=apZWdYycEUTVkJvBG57Nfw9vUvN35FaB6ZJF271Xkho,3054
-qgate_sln_mlrun/ts/ts02_feature_set/ts205.py,sha256=nj4Hz0pYe816tIqmrozCBcI0XEt32smnASCLFE8XdmQ,3460
-qgate_sln_mlrun/ts/ts02_feature_set/ts206.py,sha256=IH4ovJZxbUJXT0d8jXMPLZgDq4rCKpAnVUxdGBGT8nM,3511
+qgate_sln_mlrun/ts/ts02_feature_set/ts201.py,sha256=qF25f1_LJm1OKLg78u6trdLKwVZ_qIy2e6sa9XhUajA,9200
+qgate_sln_mlrun/ts/ts02_feature_set/ts202.py,sha256=pOgxgK6e_KnP7RVF8WsZA_Zt9uZRh0qYhojW3Zjg3VY,3586
+qgate_sln_mlrun/ts/ts02_feature_set/ts203.py,sha256=alpBxPEZB27SgI-udvoe_6BRM6k6kWfNE5bwzuRKZVM,3047
+qgate_sln_mlrun/ts/ts02_feature_set/ts204.py,sha256=hpmZrpOoTLRBCLmeUDYI25pgWkty0jGg0znvy_diPdE,3058
+qgate_sln_mlrun/ts/ts02_feature_set/ts205.py,sha256=AWtkLQfzXUIBOtEFDD_GG0mt2R5ZZxFp6ZMYvO9PRG8,3517
+qgate_sln_mlrun/ts/ts02_feature_set/ts206.py,sha256=sFy2CshVZH4Ql0tDPMP3j3TFKSBGQ6o6WwUwMpleR6Y,3128
 qgate_sln_mlrun/ts/ts03_ingest_data/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts03_ingest_data/ts302.py,sha256=5GBVlygvJRcdSfRurGwCFKVbZy4DTAKg-eIde2SJ8Yo,2697
-qgate_sln_mlrun/ts/ts03_ingest_data/ts303.py,sha256=WZSWEXjTr6SVHidwKBaBg2bkmxYu79PibvgcI5fanS8,2187
-qgate_sln_mlrun/ts/ts03_ingest_data/ts304.py,sha256=189vwa7UuiE-PjMBygoH8djZ9djjBr8CSv9mm_JPXyk,2229
-qgate_sln_mlrun/ts/ts03_ingest_data/ts305.py,sha256=wLeJh_Vl_6fMHz1NbXaiJV06Mt2CbeP_g0YFJZr8roA,3000
+qgate_sln_mlrun/ts/ts03_ingest_data/ts301.py,sha256=5uyWcD37fPodfPbVQws9081D0QRebR1PcQkiLsEAR28,2045
+qgate_sln_mlrun/ts/ts03_ingest_data/ts302.py,sha256=auJDKQglA57PSjQhyHx67A1yQDhgi2q3GWuw73LyLIo,2731
+qgate_sln_mlrun/ts/ts03_ingest_data/ts303.py,sha256=xNqXpVJfy6Cq8ZP0SvOix5yEB6NiMY3lRVxXtY8U8nw,2191
+qgate_sln_mlrun/ts/ts03_ingest_data/ts304.py,sha256=OPmtgs3dGltQE52vcfhLi3RXFdqPPc6rxb9n2v-z4Bk,2212
+qgate_sln_mlrun/ts/ts03_ingest_data/ts305.py,sha256=_JKcnwf4GvCTRN3mggxHm0spm3gogFMV5D1k0MOCA0E,3036
 qgate_sln_mlrun/ts/ts04_feature_vector/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts04_feature_vector/ts401.py,sha256=VpS4yL7yx9yVF2k8x74jfJGEapssgPKUOHN3zCTCEX0,2491
+qgate_sln_mlrun/ts/ts04_feature_vector/ts401.py,sha256=zKSKFHb26rwP3sPDLXWU6E0l8dsINbFN7-ftMiD7Bbo,2495
 qgate_sln_mlrun/ts/ts05_get_data/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts05_get_data/ts501.py,sha256=lrs7YYbGlbw0DIDF8qJeMxG9LvFS0dbrV9QGcH23UiY,1190
-qgate_sln_mlrun/ts/ts05_get_data/ts502.py,sha256=1Y0uuY1smafQi3A6swRLqRZd0tHAR-euqEN7K5WAaEY,4234
+qgate_sln_mlrun/ts/ts05_get_data/ts501.py,sha256=qM9dkSIgoxzwoGiAPRLhEDPCTjcCDLRxWsOddIC9e7g,1194
+qgate_sln_mlrun/ts/ts05_get_data/ts502.py,sha256=ZKeWBcc0e67Jmx6rvEEJbjSnqDQEcHaeC9XkaLosv8s,4238
 qgate_sln_mlrun/ts/ts06_pipeline/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts06_pipeline/ts601.py,sha256=cAshiy6dKByGPBz3pjPoKFAiURDf4mY92wmDmNNC-xo,2704
+qgate_sln_mlrun/ts/ts06_pipeline/ts601.py,sha256=XBv9B_rTwCkN5oniWbA5wbRg-jBnQn3jDWfGjJjtFxQ,3249
+qgate_sln_mlrun/ts/ts06_pipeline/ts601_ext_code.py,sha256=pTKgm_qb1SKy8lwwDZiWNoZkUR6OWcFULPJ-aqObDwU,1177
+qgate_sln_mlrun/ts/ts06_pipeline/ts602.py,sha256=0SA3TgQR-9ekNiNrTC9CW1dN6V8kHoUTiSV-7W5RQd0,2632
+qgate_sln_mlrun/ts/ts06_pipeline/ts602_ext_code.py,sha256=V99VNv8pSHTuarXTl3FD9BMlD8_NrLPUwnH7SZfwF3E,2451
 qgate_sln_mlrun/ts/ts07_build_model/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts07_build_model/ts701.py,sha256=w2cvRvWBK0sj9Ph3XvgEp1Qt5eHH8Mj-pHUwW2oCI90,3568
+qgate_sln_mlrun/ts/ts07_build_model/ts701.py,sha256=WEhapZyfRFsnxYpiAHPdYDyauwvBA6X_uT42l0hH19c,3522
 qgate_sln_mlrun/ts/ts08_serve_model/__init__.py,sha256=qxChQ26lwgN7TtSLp0GwRnaT6z-5h2BLeeJthUNTUOc,57
-qgate_sln_mlrun/ts/ts08_serve_model/ts801.py,sha256=24DbeoEUS2IZ_N3IqGd9iexTVys4LJ0Zc5Vajs5TZsY,3159
-qgate_sln_mlrun-0.2.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_sln_mlrun-0.2.3.dist-info/METADATA,sha256=oQsIYlOx6YUkfLtIan8ehuK4kPxNJHbSczj0JGG7ro8,9221
-qgate_sln_mlrun-0.2.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-qgate_sln_mlrun-0.2.3.dist-info/top_level.txt,sha256=dsHeqkGGTaYET0hq5NgEUTlhPGrzBqdwzq942Ar-a74,16
-qgate_sln_mlrun-0.2.3.dist-info/RECORD,,
+qgate_sln_mlrun/ts/ts08_serve_model/ts801.py,sha256=FXQLezyOxyJYcWSoeUVH-43m86bxCx-oat59EyMNc9A,2993
+qgate_sln_mlrun-0.2.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_sln_mlrun-0.2.4.dist-info/METADATA,sha256=H9ysh-zuNXd9JeAjPYT9ibL1PoJKJ0MYCd59DapyrkY,9140
+qgate_sln_mlrun-0.2.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+qgate_sln_mlrun-0.2.4.dist-info/top_level.txt,sha256=dsHeqkGGTaYET0hq5NgEUTlhPGrzBqdwzq942Ar-a74,16
+qgate_sln_mlrun-0.2.4.dist-info/RECORD,,
```


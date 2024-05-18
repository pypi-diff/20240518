# Comparing `tmp/cnb_tools-0.2.0.tar.gz` & `tmp/cnb_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnb_tools-0.2.0.tar", max compression
+gzip compressed data, was "cnb_tools-0.3.0.tar", max compression
```

## Comparing `cnb_tools-0.2.0.tar` & `cnb_tools-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-22 21:14:14.440131 cnb_tools-0.2.0/LICENSE
--rw-r--r--   0        0        0     3419 2024-03-22 21:14:14.440280 cnb_tools-0.2.0/README.md
--rw-r--r--   0        0        0       81 2024-03-22 21:14:14.440477 cnb_tools-0.2.0/cnb_tools/__init__.py
--rw-r--r--   0        0        0       54 2024-03-22 21:14:14.440603 cnb_tools-0.2.0/cnb_tools/__main__.py
--rw-r--r--   0        0        0     2359 2024-04-01 19:58:34.033172 cnb_tools-0.2.0/cnb_tools/classes/annotation.py
--rw-r--r--   0        0        0     1350 2024-04-01 19:58:34.033515 cnb_tools-0.2.0/cnb_tools/classes/base.py
--rw-r--r--   0        0        0     1003 2024-04-01 19:58:34.033747 cnb_tools-0.2.0/cnb_tools/classes/participant.py
--rw-r--r--   0        0        0      988 2024-04-01 19:58:34.034075 cnb_tools-0.2.0/cnb_tools/classes/queue.py
--rw-r--r--   0        0        0     2123 2024-04-01 22:53:45.728542 cnb_tools-0.2.0/cnb_tools/classes/submission.py
--rw-r--r--   0        0        0     3535 2024-04-04 16:24:02.597596 cnb_tools-0.2.0/cnb_tools/commands/submission_cli.py
--rw-r--r--   0        0        0     1183 2024-04-04 16:17:12.393627 cnb_tools-0.2.0/cnb_tools/main_cli.py
--rw-r--r--   0        0        0     1688 2024-04-04 19:43:53.397715 cnb_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 cnb_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 21:14:14.440131 cnb_tools-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3419 2024-03-22 21:14:14.440280 cnb_tools-0.3.0/README.md
+-rw-r--r--   0        0        0       81 2024-05-02 23:43:17.720382 cnb_tools-0.3.0/cnb_tools/__init__.py
+-rw-r--r--   0        0        0       54 2024-03-22 21:14:14.440603 cnb_tools-0.3.0/cnb_tools/__main__.py
+-rw-r--r--   0        0        0     2586 2024-05-16 23:29:46.060950 cnb_tools-0.3.0/cnb_tools/classes/annotation.py
+-rw-r--r--   0        0        0     1366 2024-05-16 23:29:46.061910 cnb_tools-0.3.0/cnb_tools/classes/base.py
+-rw-r--r--   0        0        0     1119 2024-05-16 23:29:46.063286 cnb_tools-0.3.0/cnb_tools/classes/participant.py
+-rw-r--r--   0        0        0      994 2024-05-16 23:29:46.064287 cnb_tools-0.3.0/cnb_tools/classes/queue.py
+-rw-r--r--   0        0        0     2341 2024-05-16 23:29:46.065040 cnb_tools-0.3.0/cnb_tools/classes/submission.py
+-rw-r--r--   0        0        0     4753 2024-05-16 23:29:46.067072 cnb_tools-0.3.0/cnb_tools/commands/submission_cli.py
+-rw-r--r--   0        0        0     1183 2024-04-04 22:34:42.552921 cnb_tools-0.3.0/cnb_tools/main_cli.py
+-rw-r--r--   0        0        0     4055 2024-05-18 00:02:25.655870 cnb_tools-0.3.0/cnb_tools/validation_toolkit.py
+-rw-r--r--   0        0        0     1688 2024-05-17 23:32:45.644846 cnb_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 cnb_tools-0.3.0/PKG-INFO
```

### Comparing `cnb_tools-0.2.0/LICENSE` & `cnb_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.2.0/README.md` & `cnb_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.2.0/cnb_tools/classes/annotation.py` & `cnb_tools-0.3.0/cnb_tools/classes/annotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 """Class representing annotations of a challenge submission."""
 
 import json
 
+from synapseclient import SubmissionStatus
 from synapseclient.core.exceptions import SynapseHTTPError
 from synapseclient.core.retry import with_retry
 
 from cnb_tools.classes.base import SynapseBase, UnknownSynapseID
 
 
 class SubmissionAnnotation(SynapseBase):
-    def __init__(self, sub_id):
+    def __init__(self, sub_id: int):
         super().__init__(sub_id)
         try:
             self._curr_annotations = self.syn.getSubmissionStatus(sub_id)
         except SynapseHTTPError as err:
             raise UnknownSynapseID(
                 f"⛔ {err.response.json().get('reason')}. "
                 "Check the ID and try again."
             ) from err
 
     @property
-    def curr_annotations(self) -> list[str]:
+    def curr_annotations(self) -> SubmissionStatus:
         """Submission's current list of annotations."""
         return self._curr_annotations
 
     @curr_annotations.setter
-    def curr_annotations(self, value: list[str]):
+    def curr_annotations(self, value: SubmissionStatus):
         self._curr_annotations = value
 
     def __str__(self) -> str:
         to_print = f"     Status: {self.curr_annotations.status}\n"
         to_print += "Annotations:\n"
         to_print += json.dumps(self.curr_annotations.submissionAnnotations, indent=2)
         return to_print
 
-    def update(self, new_annots, verbose) -> None:
+    # pylint: disable=unsupported-binary-operation
+    def update(
+            self,
+            new_annots: dict[str, str | int | float | bool],
+            verbose: bool
+        ) -> None:
         self.curr_annotations.submissionAnnotations.update(new_annots)
-        curr_annotations = self.syn.store(self.curr_annotations)
+        self.curr_annotations = self.syn.store(self.curr_annotations)
         print(f"Submission ID {self.uid} annotations updated.")
 
         if verbose:
             print("Annotations:")
-            print(json.dumps(curr_annotations.submissionAnnotations, indent=2))
+            print(json.dumps(self.curr_annotations.submissionAnnotations, indent=2))
 
-    def update_with_file(self, annots_file, verbose) -> None:
+    def update_with_file(self, annots_file: str, verbose: bool) -> None:
         with open(annots_file, encoding="utf-8") as f:
             new_annots = json.load(f)
 
         # Filter annotations with null and empty-list values
         new_annots = {
             key: value
             for key, value in new_annots.items()
@@ -57,11 +63,11 @@
             lambda: self.update(new_annots, verbose),
             wait=3,
             retries=10,
             retry_status_codes=[412, 429, 500, 502, 503, 504],
             verbose=True,
         )
 
-    def update_status(self, new_status) -> None:
+    def update_status(self, new_status: str) -> None:
         self.curr_annotations.status = new_status
         self.syn.store(self.curr_annotations)
-        print(f"Updated saubmission ID {self.uid} to status: {new_status}")
+        print(f"Updated submission ID {self.uid} to status: {new_status}")
```

### Comparing `cnb_tools-0.2.0/cnb_tools/classes/base.py` & `cnb_tools-0.3.0/cnb_tools/classes/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 
     @property
     def syn(self) -> str:
         """Synapse object with authentication."""
         return self._syn
 
     @syn.setter
-    def syn(self, _: str):
+    def syn(self, _: str) -> None:
         raise SynapseInternalError("syn object is read-only")
 
     @property
     def uid(self) -> str:
         """Synapse entity's unique ID."""
         return self._uid
 
     @uid.setter
-    def uid(self, value: str):
+    def uid(self, value: str) -> None:
         self._uid = value
 
     # pylint: disable=unsupported-binary-operation
     @staticmethod
     def _check_login() -> synapseclient.Synapse | None:
         try:
             return synapseclient.login(silent=True)
```

### Comparing `cnb_tools-0.2.0/cnb_tools/classes/participant.py` & `cnb_tools-0.3.0/cnb_tools/classes/participant.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,21 @@
 class Participant(SynapseBase):
     def __str__(self) -> str:
         try:
             return self.syn.getTeam(self.uid).get("name")
         except SynapseHTTPError:
             return self.syn.getUserProfile(self.uid).get("userName")
 
-    def create_team(self, name, description=None, can_public_join=False) -> Team:
+    # pylint: disable=unsupported-binary-operation
+    def create_team(
+        self,
+        name: str,
+        description: str | None = None,
+        can_public_join: bool = False
+    ) -> Team:
         try:
             team = self.syn.getTeam(name)
             use_team = typer.confirm(f"Team '{name}' already exists. Use this team?")
             if not use_team:
                 sys.exit("OK. Try again with a new challenge name.")
         except ValueError:
             team = Team(
```

### Comparing `cnb_tools-0.2.0/cnb_tools/classes/queue.py` & `cnb_tools-0.3.0/cnb_tools/classes/queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,19 +15,19 @@
             raise UnknownSynapseID(
                 f"⛔ {err.response.json().get('reason')}. "
                 "Check the ID and try again."
             ) from err
 
     @property
     def queue(self) -> Evaluation:
-        """Synapse entity's unique ID."""
+        """Synapse evaluation queue."""
         return self._queue
 
     @queue.setter
-    def queue(self, value: Evaluation):
+    def queue(self, value: Evaluation) -> None:
         self._queue = value
 
     def __str__(self) -> str:
         return self.queue.name
 
     def get_challenge_name(self) -> str:
         parent_id = self.queue.contentSource
```

### Comparing `cnb_tools-0.2.0/cnb_tools/commands/submission_cli.py` & `cnb_tools-0.3.0/cnb_tools/commands/submission_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 Manage submissions.
 
 Example:
     $ cnb-tools submission --help
 """
 
+import sys
 from pathlib import Path
 
 from enum import Enum
 from typing_extensions import Annotated
 import typer
 
+from cnb_tools.classes.base import UnknownSynapseID
 from cnb_tools.classes.annotation import SubmissionAnnotation
 from cnb_tools.classes.submission import Submission
 
 
 class Status(str, Enum):
     received = "RECEIVED"
     validated = "VALIDATED"
@@ -53,19 +55,32 @@
 
 @app.command()
 def change_status(
     submission_ids: Annotated[
         list[int], typer.Argument(help="One or more submission ID(s)")
     ],
     new_status: Annotated[Status, typer.Argument()],
+    skip_errors: Annotated[
+        bool,
+        typer.Option(
+            "--skip_errors",
+            help="Continue update even if unknown ID error is encountered (default: False)",
+        ),
+    ] = False,
 ):
     """Update one or more submission statuses."""
     for submission_id in submission_ids:
-        submission_annots = SubmissionAnnotation(submission_id)
-        submission_annots.update_status(new_status)
+        try:
+            submission_annots = SubmissionAnnotation(submission_id)
+            submission_annots.update_status(new_status)
+        except UnknownSynapseID as err:
+            if skip_errors:
+                print(f"Unknown submission ID: {submission_id} - skipping...")
+                continue
+            sys.exit(err)
 
 
 @app.command()
 def delete(
     submission_ids: Annotated[
         list[int],
         typer.Argument(help="One or more submission ID(s)"),
@@ -78,21 +93,34 @@
             prompt=(
                 "❗Are you sure you want to delete the submission(s)?\n\n"
                 "Once deleted, submission(s) CANNOT be recovered."
             ),
             help="Force [red]deletion[/red] without confirmation.",
         ),
     ] = False,
+    skip_errors: Annotated[
+        bool,
+        typer.Option(
+            "--skip_errors",
+            help="Continue deletion even if unknown ID error is encountered (default: False)",
+        ),
+    ] = False,
 ):
     """Delete one or more submissions."""
     print()
     if force:
         for submission_id in submission_ids:
-            submission = Submission(submission_id)
-            submission.delete()
+            try:
+                submission = Submission(submission_id)
+                submission.delete()
+            except UnknownSynapseID as err:
+                if skip_errors:
+                    print(f"Unknown submission ID: {submission_id} - skipping...")
+                    continue
+                sys.exit(err)
     else:
         print("No deletion was done.")
 
 
 @app.command()
 def download(
     submission_id: Annotated[int, typer.Argument(help="Submission ID")],
@@ -131,10 +159,21 @@
 
 
 @app.command()
 def reset(
     submission_ids: Annotated[
         list[int], typer.Argument(help="One or more submission ID(s)")
     ],
+    skip_errors: Annotated[
+        bool,
+        typer.Option(
+            "--skip_errors",
+            help="Continue update even if unknown ID error is encountered (default: False)",
+        ),
+    ] = False,
 ):
     """Reset one or more submission to RECEIVED."""
-    change_status(submission_ids=submission_ids, new_status="RECEIVED")
+    change_status(
+        submission_ids=submission_ids,
+        new_status="RECEIVED",
+        skip_errors=skip_errors
+    )
```

### Comparing `cnb_tools-0.2.0/cnb_tools/main_cli.py` & `cnb_tools-0.3.0/cnb_tools/main_cli.py`

 * *Files identical despite different names*

### Comparing `cnb_tools-0.2.0/pyproject.toml` & `cnb_tools-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cnb-tools"
-version = "0.2.0"
+version = "0.3.0"
 description = "Convenience tools/functions for challenges and benchmarking on Synapse.org"
 license = "Apache-2.0"
 authors = ["Sage CNB Team <cnb@sagebase.org>"]
 maintainers = [
     "Verena Chung <verena.chung@sagebase.org>",
 ]
 readme = "README.md"
@@ -26,15 +26,15 @@
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9.0"}
-synapseclient = "4.1.1"
+synapseclient = "4.2.0"
 
 [tool.poetry.scripts]
 cnb-tools = "cnb_tools.main_cli:app"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Sage-Bionetworks-Challenges/cnb-tools/issues"
```

### Comparing `cnb_tools-0.2.0/PKG-INFO` & `cnb_tools-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnb-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convenience tools/functions for challenges and benchmarking on Synapse.org
 Home-page: https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 License: Apache-2.0
 Author: Sage CNB Team
 Author-email: cnb@sagebase.org
 Maintainer: Verena Chung
 Maintainer-email: verena.chung@sagebase.org
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: synapseclient (==4.1.1)
+Requires-Dist: synapseclient (==4.2.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/Sage-Bionetworks-Challenges/cnb-tools/issues
 Project-URL: Documentation, https://sage-bionetworks-challenges.github.io/cnb-tools
 Project-URL: Repository, https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: cnb-tools Version: 0.2.0 Summary: Convenience
+Metadata-Version: 2.1 Name: cnb-tools Version: 0.3.0 Summary: Convenience
 tools/functions for challenges and benchmarking on Synapse.org Home-page:
 https://github.com/Sage-Bionetworks-Challenges/cnb-tools License: Apache-2.0
 Author: Sage CNB Team Author-email: cnb@sagebase.org Maintainer: Verena Chung
 Maintainer-email: verena.chung@sagebase.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Dist: synapseclient (==4.1.1) Requires-
+Libraries :: Python Modules Requires-Dist: synapseclient (==4.2.0) Requires-
 Dist: typer[all] (>=0.9.0,<0.10.0) Project-URL: Bug Tracker, https://
 github.com/Sage-Bionetworks-Challenges/cnb-tools/issues Project-URL:
 Documentation, https://sage-bionetworks-challenges.github.io/cnb-tools Project-
 URL: Repository, https://github.com/Sage-Bionetworks-Challenges/cnb-tools
 Description-Content-Type: text/markdown
 ![cnb-tools](https://raw.githubusercontent.com/Sage-Bionetworks-Challenges/cnb-
                      tools/main/docs/assets/cnb-tools.png)
```


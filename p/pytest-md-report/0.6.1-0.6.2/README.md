# Comparing `tmp/pytest_md_report-0.6.1.tar.gz` & `tmp/pytest_md_report-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_md_report-0.6.1.tar", last modified: Sat May 11 12:15:11 2024, max compression
+gzip compressed data, was "pytest_md_report-0.6.2.tar", last modified: Sat May 18 15:28:30 2024, max compression
```

## Comparing `pytest_md_report-0.6.1.tar` & `pytest_md_report-0.6.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/gfm_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/report.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_skipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_xfailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_xpassed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/pytest_md_report/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/_style_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/pytest_md_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:14:59.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/requirements/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/ss/
--rw-r--r--   0 runner    (1001) docker     (127)    75738 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/md-report_exclude_outcomes_verbose_output.png
--rw-r--r--   0 runner    (1001) docker     (127)    61742 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/md-report_gha.png
--rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/pytest_md_report_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    41954 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/pytest_md_report_example_verbose.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tests/test_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.479770 pytest_md_report-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.479770 pytest_md_report-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.483770 pytest_md_report-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/gfm_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/test_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/test_xfailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/examples/test_xpassed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.483770 pytest_md_report-0.6.2/pytest_md_report/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pytest_md_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pytest_md_report/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pytest_md_report/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pytest_md_report/_style_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18638 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pytest_md_report/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/pytest_md_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/pytest_md_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-18 15:28:30.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-18 15:28:30.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:28:30.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 15:28:30.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:28:19.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-18 15:28:30.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 15:28:30.000000 pytest_md_report-0.6.2/pytest_md_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/ss/
+-rw-r--r--   0 runner    (1001) docker     (127)    75738 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/ss/md-report_exclude_outcomes_verbose_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61742 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/ss/md-report_gha.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86154 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/ss/md-report_job-summary_full.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/ss/pytest_md_report_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41954 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/ss/pytest_md_report_example_verbose.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:28:30.487770 pytest_md_report-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/tests/test_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-18 15:28:07.000000 pytest_md_report-0.6.2/tox.ini
```

### Comparing `pytest_md_report-0.6.1/.github/workflows/ci.yml` & `pytest_md_report-0.6.2/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
       - uses: actions/download-artifact@v4
         with:
           name: dist
           path: ./dist
 
       - name: Publish package to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
+        if: github.event_name == 'push' && github.ref == 'refs/heads/master'
         with:
           repository-url: https://test.pypi.org/legacy/
           skip-existing: true
 
   sign-package:
     needs: publish-package
     runs-on: ubuntu-latest
```

### Comparing `pytest_md_report-0.6.1/.github/workflows/release.yml` & `pytest_md_report-0.6.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/.gitignore` & `pytest_md_report-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/LICENSE` & `pytest_md_report-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/PKG-INFO` & `pytest_md_report-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.6.1
+Version: 0.6.2
 Summary: A pytest plugin to generate test outcomes reports with markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
@@ -155,15 +155,15 @@
 
 Add report to pull requests
 -----------------------------------------------
 You can add test reports to pull requests by GitHub actions workflow like the below:
 
 .. code-block:: yaml
 
-    name: md-report
+    name: md-report - pull request example
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
@@ -179,28 +179,28 @@
               python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
+            env:
+              REPORT_OUTPUT: md_report.md
+            shell: bash
             run: |
-              report_file=md_report.md
-              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
-              pytest --md-report --md-report-flavor gfm --md-report-output "$report_file"
+              echo "REPORT_FILE=${REPORT_OUTPUT}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$REPORT_OUTPUT"
 
-          - name: Render reports to the PR when tests fail
+          - name: Render the report to the PR when tests fail
+            uses: marocchino/sticky-pull-request-comment@v2
             if: failure()
-            env:
-              GH_TOKEN: ${{ github.token }}
-              PR_NUMBER: ${{ github.event.number }}
-            run: |
-              if [ -f "$REPORT_FILE" ]; then
-                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
-              fi
+            with:
+              header: test-report
+              recreate: true
+              path: ${{ env.REPORT_FILE }}
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_gha.png
     :scale: 80%
     :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_gha.png
 
     Rendering result
 
@@ -208,15 +208,15 @@
 Add report to pull requests: only failed tests
 -----------------------------------------------
 You can exclude specific test outcomes from the report by using the ``--md-report-exclude-outcomes`` option.
 The below example excludes ``passed``, ``skipped``, and ``xpassed`` test outcomes from the report and posts the report to the pull request when tests fail with verbose output.
 
 .. code-block:: yaml
 
-    name: md-report
+    name: md-report - pull request example
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
@@ -232,32 +232,89 @@
               python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
+            env:
+              REPORT_OUTPUT: md_report.md
+            shell: bash
             run: |
-              report_file=md_report.md
               echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
               pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$report_file"
 
-          - name: Render reports to the PR when tests fail
+          - name: Render the report to the PR when tests fail
+            uses: marocchino/sticky-pull-request-comment@v2
             if: failure()
+            with:
+              header: test-report
+              recreate: true
+              path: ${{ env.REPORT_FILE }}
+
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+    :scale: 80%
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+
+    Rendering result
+
+
+Add reports to the job summary of the GitHub action workflow runs
+-----------------------------------------------------------------------------
+The below example adds test reports to the job summary of the GitHub action workflow runs when tests fail.
+
+.. code-block:: yaml
+
+    name: md-report - job summary example
+
+    on:
+      pull_request:
+
+    jobs:
+      run-tests:
+        runs-on: ${{ matrix.os }}
+        strategy:
+          fail-fast: false
+          matrix:
+            os: [ubuntu-latest, windows-latest]
+
+        steps:
+          - uses: actions/checkout@v4
+
+          - uses: actions/setup-python@v5
+            with:
+              python-version: '3.12'
+              cache: pip
+
+          - name: Install dependencies
+            run: pip install --upgrade pytest-md-report
+
+          - name: Run tests
             env:
-              GH_TOKEN: ${{ github.token }}
-              PR_NUMBER: ${{ github.event.number }}
+              REPORT_OUTPUT: md_report.md
+            shell: bash
+            run: |
+              echo "REPORT_FILE=${REPORT_OUTPUT}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$REPORT_OUTPUT"
+
+          - name: Output reports to the job summary when tests fail
+            if: failure()
+            shell: bash
             run: |
               if [ -f "$REPORT_FILE" ]; then
-                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+                echo "<details><summary>Failed Test Report</summary>" >> $GITHUB_STEP_SUMMARY
+                echo "" >> $GITHUB_STEP_SUMMARY
+                cat "$REPORT_FILE" >> $GITHUB_STEP_SUMMARY
+                echo "" >> $GITHUB_STEP_SUMMARY
+                echo "</details>" >> $GITHUB_STEP_SUMMARY
               fi
 
-.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_job-summary_full.png
     :scale: 80%
-    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_job-summary_full.png
 
     Rendering result
 
 
 Options
 ============================================
```

### Comparing `pytest_md_report-0.6.1/README.rst` & `pytest_md_report-0.6.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 Add report to pull requests
 -----------------------------------------------
 You can add test reports to pull requests by GitHub actions workflow like the below:
 
 .. code-block:: yaml
 
-    name: md-report
+    name: md-report - pull request example
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
@@ -137,28 +137,28 @@
               python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
+            env:
+              REPORT_OUTPUT: md_report.md
+            shell: bash
             run: |
-              report_file=md_report.md
-              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
-              pytest --md-report --md-report-flavor gfm --md-report-output "$report_file"
+              echo "REPORT_FILE=${REPORT_OUTPUT}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$REPORT_OUTPUT"
 
-          - name: Render reports to the PR when tests fail
+          - name: Render the report to the PR when tests fail
+            uses: marocchino/sticky-pull-request-comment@v2
             if: failure()
-            env:
-              GH_TOKEN: ${{ github.token }}
-              PR_NUMBER: ${{ github.event.number }}
-            run: |
-              if [ -f "$REPORT_FILE" ]; then
-                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
-              fi
+            with:
+              header: test-report
+              recreate: true
+              path: ${{ env.REPORT_FILE }}
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_gha.png
     :scale: 80%
     :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_gha.png
 
     Rendering result
 
@@ -166,15 +166,15 @@
 Add report to pull requests: only failed tests
 -----------------------------------------------
 You can exclude specific test outcomes from the report by using the ``--md-report-exclude-outcomes`` option.
 The below example excludes ``passed``, ``skipped``, and ``xpassed`` test outcomes from the report and posts the report to the pull request when tests fail with verbose output.
 
 .. code-block:: yaml
 
-    name: md-report
+    name: md-report - pull request example
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
@@ -190,32 +190,89 @@
               python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
+            env:
+              REPORT_OUTPUT: md_report.md
+            shell: bash
             run: |
-              report_file=md_report.md
               echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
               pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$report_file"
 
-          - name: Render reports to the PR when tests fail
+          - name: Render the report to the PR when tests fail
+            uses: marocchino/sticky-pull-request-comment@v2
             if: failure()
+            with:
+              header: test-report
+              recreate: true
+              path: ${{ env.REPORT_FILE }}
+
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+    :scale: 80%
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+
+    Rendering result
+
+
+Add reports to the job summary of the GitHub action workflow runs
+-----------------------------------------------------------------------------
+The below example adds test reports to the job summary of the GitHub action workflow runs when tests fail.
+
+.. code-block:: yaml
+
+    name: md-report - job summary example
+
+    on:
+      pull_request:
+
+    jobs:
+      run-tests:
+        runs-on: ${{ matrix.os }}
+        strategy:
+          fail-fast: false
+          matrix:
+            os: [ubuntu-latest, windows-latest]
+
+        steps:
+          - uses: actions/checkout@v4
+
+          - uses: actions/setup-python@v5
+            with:
+              python-version: '3.12'
+              cache: pip
+
+          - name: Install dependencies
+            run: pip install --upgrade pytest-md-report
+
+          - name: Run tests
             env:
-              GH_TOKEN: ${{ github.token }}
-              PR_NUMBER: ${{ github.event.number }}
+              REPORT_OUTPUT: md_report.md
+            shell: bash
+            run: |
+              echo "REPORT_FILE=${REPORT_OUTPUT}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$REPORT_OUTPUT"
+
+          - name: Output reports to the job summary when tests fail
+            if: failure()
+            shell: bash
             run: |
               if [ -f "$REPORT_FILE" ]; then
-                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+                echo "<details><summary>Failed Test Report</summary>" >> $GITHUB_STEP_SUMMARY
+                echo "" >> $GITHUB_STEP_SUMMARY
+                cat "$REPORT_FILE" >> $GITHUB_STEP_SUMMARY
+                echo "" >> $GITHUB_STEP_SUMMARY
+                echo "</details>" >> $GITHUB_STEP_SUMMARY
               fi
 
-.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_job-summary_full.png
     :scale: 80%
-    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_job-summary_full.png
 
     Rendering result
 
 
 Options
 ============================================
```

### Comparing `pytest_md_report-0.6.1/examples/gfm_report.md` & `pytest_md_report-0.6.2/examples/gfm_report.md`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/examples/report.md` & `pytest_md_report-0.6.2/examples/report.md`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/pyproject.toml` & `pytest_md_report-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/pytest_md_report/_const.py` & `pytest_md_report-0.6.2/pytest_md_report/_const.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/pytest_md_report/_style_filter.py` & `pytest_md_report-0.6.2/pytest_md_report/_style_filter.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/pytest_md_report/plugin.py` & `pytest_md_report-0.6.2/pytest_md_report/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,15 @@
 
         for value in values:
             try:
                 filesystempath, lineno, domaininfo = value.location
             except AttributeError:
                 continue
 
+            filesystempath = os.path.normpath(filesystempath).replace("\\", "/")
             testfunc = value.head_line.split("[")[0]
 
             if verbosity_level == 0:
                 key: Tuple = (filesystempath,)
             elif verbosity_level >= 1:
                 key = (filesystempath, testfunc)
             else:
```

### Comparing `pytest_md_report-0.6.1/pytest_md_report.egg-info/PKG-INFO` & `pytest_md_report-0.6.2/pytest_md_report.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.6.1
+Version: 0.6.2
 Summary: A pytest plugin to generate test outcomes reports with markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
@@ -155,15 +155,15 @@
 
 Add report to pull requests
 -----------------------------------------------
 You can add test reports to pull requests by GitHub actions workflow like the below:
 
 .. code-block:: yaml
 
-    name: md-report
+    name: md-report - pull request example
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
@@ -179,28 +179,28 @@
               python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
+            env:
+              REPORT_OUTPUT: md_report.md
+            shell: bash
             run: |
-              report_file=md_report.md
-              echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
-              pytest --md-report --md-report-flavor gfm --md-report-output "$report_file"
+              echo "REPORT_FILE=${REPORT_OUTPUT}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$REPORT_OUTPUT"
 
-          - name: Render reports to the PR when tests fail
+          - name: Render the report to the PR when tests fail
+            uses: marocchino/sticky-pull-request-comment@v2
             if: failure()
-            env:
-              GH_TOKEN: ${{ github.token }}
-              PR_NUMBER: ${{ github.event.number }}
-            run: |
-              if [ -f "$REPORT_FILE" ]; then
-                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
-              fi
+            with:
+              header: test-report
+              recreate: true
+              path: ${{ env.REPORT_FILE }}
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_gha.png
     :scale: 80%
     :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_gha.png
 
     Rendering result
 
@@ -208,15 +208,15 @@
 Add report to pull requests: only failed tests
 -----------------------------------------------
 You can exclude specific test outcomes from the report by using the ``--md-report-exclude-outcomes`` option.
 The below example excludes ``passed``, ``skipped``, and ``xpassed`` test outcomes from the report and posts the report to the pull request when tests fail with verbose output.
 
 .. code-block:: yaml
 
-    name: md-report
+    name: md-report - pull request example
 
     on:
       pull_request:
 
     jobs:
       run-tests:
         runs-on: ubuntu-latest
@@ -232,32 +232,89 @@
               python-version: '3.12'
               cache: pip
 
           - name: Install dependencies
             run: pip install --upgrade pytest-md-report
 
           - name: Run tests
+            env:
+              REPORT_OUTPUT: md_report.md
+            shell: bash
             run: |
-              report_file=md_report.md
               echo "REPORT_FILE=${report_file}" >> "$GITHUB_ENV"
               pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$report_file"
 
-          - name: Render reports to the PR when tests fail
+          - name: Render the report to the PR when tests fail
+            uses: marocchino/sticky-pull-request-comment@v2
             if: failure()
+            with:
+              header: test-report
+              recreate: true
+              path: ${{ env.REPORT_FILE }}
+
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+    :scale: 80%
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+
+    Rendering result
+
+
+Add reports to the job summary of the GitHub action workflow runs
+-----------------------------------------------------------------------------
+The below example adds test reports to the job summary of the GitHub action workflow runs when tests fail.
+
+.. code-block:: yaml
+
+    name: md-report - job summary example
+
+    on:
+      pull_request:
+
+    jobs:
+      run-tests:
+        runs-on: ${{ matrix.os }}
+        strategy:
+          fail-fast: false
+          matrix:
+            os: [ubuntu-latest, windows-latest]
+
+        steps:
+          - uses: actions/checkout@v4
+
+          - uses: actions/setup-python@v5
+            with:
+              python-version: '3.12'
+              cache: pip
+
+          - name: Install dependencies
+            run: pip install --upgrade pytest-md-report
+
+          - name: Run tests
             env:
-              GH_TOKEN: ${{ github.token }}
-              PR_NUMBER: ${{ github.event.number }}
+              REPORT_OUTPUT: md_report.md
+            shell: bash
+            run: |
+              echo "REPORT_FILE=${REPORT_OUTPUT}" >> "$GITHUB_ENV"
+              pytest -v --md-report --md-report-flavor gfm --md-report-exclude-outcomes passed skipped xpassed --md-report-output "$REPORT_OUTPUT"
+
+          - name: Output reports to the job summary when tests fail
+            if: failure()
+            shell: bash
             run: |
               if [ -f "$REPORT_FILE" ]; then
-                gh pr comment $PR_NUMBER --body-file "$REPORT_FILE"
+                echo "<details><summary>Failed Test Report</summary>" >> $GITHUB_STEP_SUMMARY
+                echo "" >> $GITHUB_STEP_SUMMARY
+                cat "$REPORT_FILE" >> $GITHUB_STEP_SUMMARY
+                echo "" >> $GITHUB_STEP_SUMMARY
+                echo "</details>" >> $GITHUB_STEP_SUMMARY
               fi
 
-.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_exclude_outcomes_verbose_output.png
+.. figure:: https://cdn.jsdelivr.net/gh/thombashi/pytest-md-report@master/ss/md-report_job-summary_full.png
     :scale: 80%
-    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_exclude_outcomes_verbose_output.png
+    :alt: https://github.com/thombashi/pytest-md-report/blob/master/ss/md-report_job-summary_full.png
 
     Rendering result
 
 
 Options
 ============================================
```

### Comparing `pytest_md_report-0.6.1/pytest_md_report.egg-info/SOURCES.txt` & `pytest_md_report-0.6.2/pytest_md_report.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,12 +31,13 @@
 pytest_md_report.egg-info/not-zip-safe
 pytest_md_report.egg-info/requires.txt
 pytest_md_report.egg-info/top_level.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
 ss/md-report_exclude_outcomes_verbose_output.png
 ss/md-report_gha.png
+ss/md-report_job-summary_full.png
 ss/pytest_md_report_example.png
 ss/pytest_md_report_example_verbose.png
 tests/conftest.py
 tests/test_option.py
 tests/test_plugin.py
```

### Comparing `pytest_md_report-0.6.1/setup.py` & `pytest_md_report-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/ss/md-report_exclude_outcomes_verbose_output.png` & `pytest_md_report-0.6.2/ss/md-report_exclude_outcomes_verbose_output.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/ss/md-report_gha.png` & `pytest_md_report-0.6.2/ss/md-report_gha.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/ss/pytest_md_report_example.png` & `pytest_md_report-0.6.2/ss/pytest_md_report_example.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/ss/pytest_md_report_example_verbose.png` & `pytest_md_report-0.6.2/ss/pytest_md_report_example_verbose.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/tests/test_option.py` & `pytest_md_report-0.6.2/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/tests/test_plugin.py` & `pytest_md_report-0.6.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.1/tox.ini` & `pytest_md_report-0.6.2/tox.ini`

 * *Files identical despite different names*


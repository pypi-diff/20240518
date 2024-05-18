# Comparing `tmp/packaging_demo_avr-0.0.4.tar.gz` & `tmp/packaging_demo_avr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging_demo_avr-0.0.4.tar", last modified: Sat May 18 01:57:11 2024, max compression
+gzip compressed data, was "packaging_demo_avr-0.0.7.tar", last modified: Sat May 18 15:48:50 2024, max compression
```

## Comparing `packaging_demo_avr-0.0.4.tar` & `packaging_demo_avr-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.189787 packaging_demo_avr-0.0.4/
--rw-r--r--   0 avr27     (1000) avr27     (1000)    27488 2024-05-18 01:57:11.189787 packaging_demo_avr-0.0.4/PKG-INFO
--rw-r--r--   0 avr27     (1000) avr27     (1000)    26457 2024-05-18 01:55:36.000000 packaging_demo_avr-0.0.4/README.md
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo/
--rw-r--r--   0 avr27     (1000) avr27     (1000)       18 2024-05-18 01:55:57.000000 packaging_demo_avr-0.0.4/packaging_demo/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.4/packaging_demo/cities.json
--rw-r--r--   0 avr27     (1000) avr27     (1000)      134 2024-05-16 02:51:30.000000 packaging_demo_avr-0.0.4/packaging_demo/colorized_demo.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      281 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.4/packaging_demo/my_file.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo/my_folder/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-11 02:32:35.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2282 2024-05-17 04:24:28.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/another-cities.json
--rw-r--r--   0 avr27     (1000) avr27     (1000)      196 2024-05-12 11:42:54.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_sub_package/
--rw-r--r--   0 avr27     (1000) avr27     (1000)        0 2024-05-11 06:29:23.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_sub_package/__init__.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      198 2024-05-11 04:27:59.000000 packaging_demo_avr-0.0.4/packaging_demo/my_folder/my_sub_package/nested_module.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)       37 2024-05-11 06:56:11.000000 packaging_demo_avr-0.0.4/packaging_demo/my_other_file.py
--rw-r--r--   0 avr27     (1000) avr27     (1000)      864 2024-05-15 04:07:16.000000 packaging_demo_avr-0.0.4/packaging_demo/states_info.py
-drwxr-xr-x   0 avr27     (1000) avr27     (1000)        0 2024-05-18 01:57:11.179787 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/
--rw-r--r--   0 avr27     (1000) avr27     (1000)    27488 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/PKG-INFO
--rw-r--r--   0 avr27     (1000) avr27     (1000)      654 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/SOURCES.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)        1 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/dependency_links.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)      255 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/requires.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)       15 2024-05-18 01:57:11.000000 packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/top_level.txt
--rw-r--r--   0 avr27     (1000) avr27     (1000)     2992 2024-05-18 01:54:48.000000 packaging_demo_avr-0.0.4/pyproject.toml
--rw-r--r--   0 avr27     (1000) avr27     (1000)       38 2024-05-18 01:57:11.189787 packaging_demo_avr-0.0.4/setup.cfg
--rw-r--r--   0 avr27     (1000) avr27     (1000)        6 2024-05-18 01:56:05.000000 packaging_demo_avr-0.0.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:48:50.167830 packaging_demo_avr-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    32643 2024-05-18 15:48:50.167830 packaging_demo_avr-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31246 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:48:50.163830 packaging_demo_avr-0.0.7/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/cities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:48:50.163830 packaging_demo_avr-0.0.7/packaging_demo/my_folder/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_folder/another-cities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_folder/my_nested_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:48:50.163830 packaging_demo_avr-0.0.7/packaging_demo/my_folder/my_sub_package/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_folder/my_sub_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_folder/my_sub_package/nested_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:48:50.167830 packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32643 2024-05-18 15:48:50.000000 packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-18 15:48:50.000000 packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:48:50.000000 packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-18 15:48:50.000000 packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:48:50.000000 packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:48:50.167830 packaging_demo_avr-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 15:48:40.000000 packaging_demo_avr-0.0.7/version.txt
```

### Comparing `packaging_demo_avr-0.0.4/PKG-INFO` & `packaging_demo_avr-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.4
+Version: 0.0.7
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
-Keywords: one,two
+Project-URL: Repository, https://github.com/avr2002/python-packaging
+Project-URL: Documentation, https://github.com/avr2002/python-packaging/blob/main/README.md
+Keywords: python,bash,makefile,pypi,ci-cd,setuptools,wheels,package-development,github-actions,pypi-package,pre-commit-hooks,pyproject-toml,gitactions-workflow,github-actions-enabled,pre-commit-ci,pre-commit-config
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: fastapi
 Requires-Dist: importlib-metadata; python_version < "3.10"
 Provides-Extra: test
@@ -19,19 +21,19 @@
 Requires-Dist: twine; extra == "release"
 Provides-Extra: static-code-qa
 Requires-Dist: pre-commit; extra == "static-code-qa"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black; extra == "dev"
-Requires-Dist: packaging-demo[release,static-code-qa,test]; extra == "dev"
+Requires-Dist: packaging-demo-avr[release,static-code-qa,test]; extra == "dev"
 Provides-Extra: colors
 Requires-Dist: rich; extra == "colors"
 Provides-Extra: all
-Requires-Dist: packaging-demo[colors,dev]; extra == "all"
+Requires-Dist: packaging-demo-avr[colors,dev]; extra == "all"
 
 ## Why package your Python code?
 
 1. Distributing your code
 2. Non-painful import statements
 3. Reproduciblity
 
@@ -768,7 +770,176 @@
 
 
 - [Taskfile](https://github.com/adriancooney/Taskfile)
 
 
 - [`justfile`](https://github.com/casey/just)
 - [pyinvoke](https://www.pyinvoke.org/)
+
+* **
+
+# Continuous Delivery using GitHub Actions
+
+## Goals
+1. Understand Continuous Delivery
+2. Know the parts of a CI/CD pipeline for Python Packages
+3. Have an advanced understanding of GitHub Actions
+
+
+
+## Delivery "Environments"
+
+>Dev $\rightarrow$ QA/Staging $\rightarrow$ Prod
+
+
+- Pre-release version namings
+  - 0.0.0rc0 (rc = release candidate)
+  - 0.0.0.rc1
+  - 0.0.0a0 (alpha)
+  - 0.0.0b1 (beta)
+
+![alt text](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/cd.png?raw=true)
+
+
+## High-level CI/CD Workflow for Python Packages
+
+![CI/CD Workflow for Python Packages](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/workflow.png?raw=true)
+
+
+## Detailed CI/CD Workflow for Python Packages
+
+![Detailed CI/CD Workflow for Python Packages](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/detailed-workflow.png?raw=true)
+
+
+### GitHub CI/CD Workflow in worflows yaml file
+
+```toml
+# .github/workflows/publish.yaml
+
+name: Build, Test, and Publish
+
+# triggers: whenever there is new changes pulled/pushed on this
+# repo under given conditions, run the below jobs
+on:
+  pull_request:
+    types: [opened, synchronize]
+
+  push:
+    branches:
+      - main
+
+  # Manually trigger a workflow
+  # https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#workflow_dispatch
+  workflow_dispatch:
+
+jobs:
+
+  build-test-and-publish:
+
+    runs-on: ubuntu-latest
+
+    steps:
+    # github actions checksout, clones our repo, and checks out the branch we're working in
+    - uses: actions/checkout@v3
+      with:
+        # Number of commits to fetch. 0 indicates all history for all branches and tags
+        # fetching all tags so to aviod duplicate version tagging in 'Tag with the Release Version'
+        fetch-depth: 0
+
+    - name: Set up Python 3.8
+      uses: actions/setup-python@v3
+      with:
+        python-version: 3.8
+
+    # tagging the release version to avoid duplicate releases
+    - name: Tag with the Release Version
+      run: |
+        git tag $(cat version.txt)
+
+    - name: Install Python Dependencies
+      run: |
+        /bin/bash -x run.sh install
+
+    - name: Lint, Format, and Other Static Code Quality Check
+      run: |
+        /bin/bash -x run.sh lint:ci
+
+    - name: Build Python Package
+      run: |
+        /bin/bash -x run.sh build
+
+    - name: Publish to Test PyPI
+      # setting -x in below publish:test will not leak any secrets as they are masked in github
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+        /bin/bash -x run.sh publish:test
+      env:
+        TEST_PYPI_TOKEN: ${{ secrets.TEST_PYPI_TOKEN }}
+
+    - name: Publish to Prod PyPI
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+        /bin/bash -x run.sh publish:prod
+      env:
+        PROD_PYPI_TOKEN: ${{ secrets.PROD_PYPI_TOKEN }}
+
+    - name: Push Tags
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+       git push origin --tags
+```
+
+### GitHub Actions Optimizations
+
+1. Locking Requirements
+   - It's not really recommended to pin exact versions of dependencies to avoid future conflict
+   - But it's good practice to store them in the requirements file for future debugging.
+   - Tools:
+
+2. Dependency Caching
+   - Whenever github actions gets executed in the github CI, everytime it's run on a fresh container.
+    Thus, everytime we'll have to download and re-install dependencies from pip again and again;
+    which is not a good as it's inefficeint and slows our workflow.
+
+   - Thus we would want to install all the dependencies when the workflow ran first and use it every
+     time a new worflow is run.
+
+   - GitHub Actions provide this functionality by caching the dependencies, it stores the installed
+     dependencies(`~/.cache/pip`) and downloads it everytime a new workflow is run.
+     [**Docs**](https://github.com/actions/cache/blob/main/examples.md#python---pip)
+
+   ```toml
+   - uses: actions/cache@v3
+     with:
+      path: ~/.cache/pip
+      key: ${{ runner.os }}-pip-${{ hashFiles('**/requirements.txt') }}
+      restore-keys: |
+        ${{ runner.os }}-pip-
+   ```
+
+3. Parallelization
+
+   - We moved from above shown workflow to now a parallelized workflow as shown below.
+   - This helps in faster running of workflow, helping discover bugs in any steps
+     at the same time which was not possible in linear flow as earlier.
+
+```toml
+# See .github/workflows/publish.yaml
+
+jobs:
+
+  check-verison-txt:
+    ...
+
+  lint-format-and-static-code-checks:
+    ....
+
+  build-wheel-and-sdist:
+    ...
+
+  publish:
+    needs:
+      - check-verison-txt
+      - lint-format-and-static-code-checks
+      - build-wheel-and-sdist
+    ...
+```
```

### Comparing `packaging_demo_avr-0.0.4/README.md` & `packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: packaging-demo-avr
+Version: 0.0.7
+Summary: Demo for Python Packaging
+Author-email: Amit Vikram Raj <avr13405@gmail.com>
+License: MIT
+Project-URL: Repository, https://github.com/avr2002/python-packaging
+Project-URL: Documentation, https://github.com/avr2002/python-packaging/blob/main/README.md
+Keywords: python,bash,makefile,pypi,ci-cd,setuptools,wheels,package-development,github-actions,pypi-package,pre-commit-hooks,pyproject-toml,gitactions-workflow,github-actions-enabled,pre-commit-ci,pre-commit-config
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: fastapi
+Requires-Dist: importlib-metadata; python_version < "3.10"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: release
+Requires-Dist: build; extra == "release"
+Requires-Dist: twine; extra == "release"
+Provides-Extra: static-code-qa
+Requires-Dist: pre-commit; extra == "static-code-qa"
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: packaging-demo-avr[release,static-code-qa,test]; extra == "dev"
+Provides-Extra: colors
+Requires-Dist: rich; extra == "colors"
+Provides-Extra: all
+Requires-Dist: packaging-demo-avr[colors,dev]; extra == "all"
+
 ## Why package your Python code?
 
 1. Distributing your code
 2. Non-painful import statements
 3. Reproduciblity
 
 
@@ -737,7 +770,176 @@
 
 
 - [Taskfile](https://github.com/adriancooney/Taskfile)
 
 
 - [`justfile`](https://github.com/casey/just)
 - [pyinvoke](https://www.pyinvoke.org/)
+
+* **
+
+# Continuous Delivery using GitHub Actions
+
+## Goals
+1. Understand Continuous Delivery
+2. Know the parts of a CI/CD pipeline for Python Packages
+3. Have an advanced understanding of GitHub Actions
+
+
+
+## Delivery "Environments"
+
+>Dev $\rightarrow$ QA/Staging $\rightarrow$ Prod
+
+
+- Pre-release version namings
+  - 0.0.0rc0 (rc = release candidate)
+  - 0.0.0.rc1
+  - 0.0.0a0 (alpha)
+  - 0.0.0b1 (beta)
+
+![alt text](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/cd.png?raw=true)
+
+
+## High-level CI/CD Workflow for Python Packages
+
+![CI/CD Workflow for Python Packages](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/workflow.png?raw=true)
+
+
+## Detailed CI/CD Workflow for Python Packages
+
+![Detailed CI/CD Workflow for Python Packages](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/detailed-workflow.png?raw=true)
+
+
+### GitHub CI/CD Workflow in worflows yaml file
+
+```toml
+# .github/workflows/publish.yaml
+
+name: Build, Test, and Publish
+
+# triggers: whenever there is new changes pulled/pushed on this
+# repo under given conditions, run the below jobs
+on:
+  pull_request:
+    types: [opened, synchronize]
+
+  push:
+    branches:
+      - main
+
+  # Manually trigger a workflow
+  # https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#workflow_dispatch
+  workflow_dispatch:
+
+jobs:
+
+  build-test-and-publish:
+
+    runs-on: ubuntu-latest
+
+    steps:
+    # github actions checksout, clones our repo, and checks out the branch we're working in
+    - uses: actions/checkout@v3
+      with:
+        # Number of commits to fetch. 0 indicates all history for all branches and tags
+        # fetching all tags so to aviod duplicate version tagging in 'Tag with the Release Version'
+        fetch-depth: 0
+
+    - name: Set up Python 3.8
+      uses: actions/setup-python@v3
+      with:
+        python-version: 3.8
+
+    # tagging the release version to avoid duplicate releases
+    - name: Tag with the Release Version
+      run: |
+        git tag $(cat version.txt)
+
+    - name: Install Python Dependencies
+      run: |
+        /bin/bash -x run.sh install
+
+    - name: Lint, Format, and Other Static Code Quality Check
+      run: |
+        /bin/bash -x run.sh lint:ci
+
+    - name: Build Python Package
+      run: |
+        /bin/bash -x run.sh build
+
+    - name: Publish to Test PyPI
+      # setting -x in below publish:test will not leak any secrets as they are masked in github
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+        /bin/bash -x run.sh publish:test
+      env:
+        TEST_PYPI_TOKEN: ${{ secrets.TEST_PYPI_TOKEN }}
+
+    - name: Publish to Prod PyPI
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+        /bin/bash -x run.sh publish:prod
+      env:
+        PROD_PYPI_TOKEN: ${{ secrets.PROD_PYPI_TOKEN }}
+
+    - name: Push Tags
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+       git push origin --tags
+```
+
+### GitHub Actions Optimizations
+
+1. Locking Requirements
+   - It's not really recommended to pin exact versions of dependencies to avoid future conflict
+   - But it's good practice to store them in the requirements file for future debugging.
+   - Tools:
+
+2. Dependency Caching
+   - Whenever github actions gets executed in the github CI, everytime it's run on a fresh container.
+    Thus, everytime we'll have to download and re-install dependencies from pip again and again;
+    which is not a good as it's inefficeint and slows our workflow.
+
+   - Thus we would want to install all the dependencies when the workflow ran first and use it every
+     time a new worflow is run.
+
+   - GitHub Actions provide this functionality by caching the dependencies, it stores the installed
+     dependencies(`~/.cache/pip`) and downloads it everytime a new workflow is run.
+     [**Docs**](https://github.com/actions/cache/blob/main/examples.md#python---pip)
+
+   ```toml
+   - uses: actions/cache@v3
+     with:
+      path: ~/.cache/pip
+      key: ${{ runner.os }}-pip-${{ hashFiles('**/requirements.txt') }}
+      restore-keys: |
+        ${{ runner.os }}-pip-
+   ```
+
+3. Parallelization
+
+   - We moved from above shown workflow to now a parallelized workflow as shown below.
+   - This helps in faster running of workflow, helping discover bugs in any steps
+     at the same time which was not possible in linear flow as earlier.
+
+```toml
+# See .github/workflows/publish.yaml
+
+jobs:
+
+  check-verison-txt:
+    ...
+
+  lint-format-and-static-code-checks:
+    ....
+
+  build-wheel-and-sdist:
+    ...
+
+  publish:
+    needs:
+      - check-verison-txt
+      - lint-format-and-static-code-checks
+      - build-wheel-and-sdist
+    ...
+```
```

### Comparing `packaging_demo_avr-0.0.4/packaging_demo/cities.json` & `packaging_demo_avr-0.0.7/packaging_demo/cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.4/packaging_demo/my_folder/another-cities.json` & `packaging_demo_avr-0.0.7/packaging_demo/my_folder/another-cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.4/packaging_demo/states_info.py` & `packaging_demo_avr-0.0.7/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/PKG-INFO` & `packaging_demo_avr-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: packaging-demo-avr
-Version: 0.0.4
-Summary: Demo for Python Packaging
-Author-email: Amit Vikram Raj <avr13405@gmail.com>
-License: MIT
-Keywords: one,two
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: fastapi
-Requires-Dist: importlib-metadata; python_version < "3.10"
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: release
-Requires-Dist: build; extra == "release"
-Requires-Dist: twine; extra == "release"
-Provides-Extra: static-code-qa
-Requires-Dist: pre-commit; extra == "static-code-qa"
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: packaging-demo[release,static-code-qa,test]; extra == "dev"
-Provides-Extra: colors
-Requires-Dist: rich; extra == "colors"
-Provides-Extra: all
-Requires-Dist: packaging-demo[colors,dev]; extra == "all"
-
 ## Why package your Python code?
 
 1. Distributing your code
 2. Non-painful import statements
 3. Reproduciblity
 
 
@@ -768,7 +737,176 @@
 
 
 - [Taskfile](https://github.com/adriancooney/Taskfile)
 
 
 - [`justfile`](https://github.com/casey/just)
 - [pyinvoke](https://www.pyinvoke.org/)
+
+* **
+
+# Continuous Delivery using GitHub Actions
+
+## Goals
+1. Understand Continuous Delivery
+2. Know the parts of a CI/CD pipeline for Python Packages
+3. Have an advanced understanding of GitHub Actions
+
+
+
+## Delivery "Environments"
+
+>Dev $\rightarrow$ QA/Staging $\rightarrow$ Prod
+
+
+- Pre-release version namings
+  - 0.0.0rc0 (rc = release candidate)
+  - 0.0.0.rc1
+  - 0.0.0a0 (alpha)
+  - 0.0.0b1 (beta)
+
+![alt text](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/cd.png?raw=true)
+
+
+## High-level CI/CD Workflow for Python Packages
+
+![CI/CD Workflow for Python Packages](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/workflow.png?raw=true)
+
+
+## Detailed CI/CD Workflow for Python Packages
+
+![Detailed CI/CD Workflow for Python Packages](https://github.com/avr2002/python-packaging/blob/main/packaging_demo/assets/detailed-workflow.png?raw=true)
+
+
+### GitHub CI/CD Workflow in worflows yaml file
+
+```toml
+# .github/workflows/publish.yaml
+
+name: Build, Test, and Publish
+
+# triggers: whenever there is new changes pulled/pushed on this
+# repo under given conditions, run the below jobs
+on:
+  pull_request:
+    types: [opened, synchronize]
+
+  push:
+    branches:
+      - main
+
+  # Manually trigger a workflow
+  # https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows#workflow_dispatch
+  workflow_dispatch:
+
+jobs:
+
+  build-test-and-publish:
+
+    runs-on: ubuntu-latest
+
+    steps:
+    # github actions checksout, clones our repo, and checks out the branch we're working in
+    - uses: actions/checkout@v3
+      with:
+        # Number of commits to fetch. 0 indicates all history for all branches and tags
+        # fetching all tags so to aviod duplicate version tagging in 'Tag with the Release Version'
+        fetch-depth: 0
+
+    - name: Set up Python 3.8
+      uses: actions/setup-python@v3
+      with:
+        python-version: 3.8
+
+    # tagging the release version to avoid duplicate releases
+    - name: Tag with the Release Version
+      run: |
+        git tag $(cat version.txt)
+
+    - name: Install Python Dependencies
+      run: |
+        /bin/bash -x run.sh install
+
+    - name: Lint, Format, and Other Static Code Quality Check
+      run: |
+        /bin/bash -x run.sh lint:ci
+
+    - name: Build Python Package
+      run: |
+        /bin/bash -x run.sh build
+
+    - name: Publish to Test PyPI
+      # setting -x in below publish:test will not leak any secrets as they are masked in github
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+        /bin/bash -x run.sh publish:test
+      env:
+        TEST_PYPI_TOKEN: ${{ secrets.TEST_PYPI_TOKEN }}
+
+    - name: Publish to Prod PyPI
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+        /bin/bash -x run.sh publish:prod
+      env:
+        PROD_PYPI_TOKEN: ${{ secrets.PROD_PYPI_TOKEN }}
+
+    - name: Push Tags
+      if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
+      run: |
+       git push origin --tags
+```
+
+### GitHub Actions Optimizations
+
+1. Locking Requirements
+   - It's not really recommended to pin exact versions of dependencies to avoid future conflict
+   - But it's good practice to store them in the requirements file for future debugging.
+   - Tools:
+
+2. Dependency Caching
+   - Whenever github actions gets executed in the github CI, everytime it's run on a fresh container.
+    Thus, everytime we'll have to download and re-install dependencies from pip again and again;
+    which is not a good as it's inefficeint and slows our workflow.
+
+   - Thus we would want to install all the dependencies when the workflow ran first and use it every
+     time a new worflow is run.
+
+   - GitHub Actions provide this functionality by caching the dependencies, it stores the installed
+     dependencies(`~/.cache/pip`) and downloads it everytime a new workflow is run.
+     [**Docs**](https://github.com/actions/cache/blob/main/examples.md#python---pip)
+
+   ```toml
+   - uses: actions/cache@v3
+     with:
+      path: ~/.cache/pip
+      key: ${{ runner.os }}-pip-${{ hashFiles('**/requirements.txt') }}
+      restore-keys: |
+        ${{ runner.os }}-pip-
+   ```
+
+3. Parallelization
+
+   - We moved from above shown workflow to now a parallelized workflow as shown below.
+   - This helps in faster running of workflow, helping discover bugs in any steps
+     at the same time which was not possible in linear flow as earlier.
+
+```toml
+# See .github/workflows/publish.yaml
+
+jobs:
+
+  check-verison-txt:
+    ...
+
+  lint-format-and-static-code-checks:
+    ....
+
+  build-wheel-and-sdist:
+    ...
+
+  publish:
+    needs:
+      - check-verison-txt
+      - lint-format-and-static-code-checks
+      - build-wheel-and-sdist
+    ...
+```
```

### Comparing `packaging_demo_avr-0.0.4/packaging_demo_avr.egg-info/SOURCES.txt` & `packaging_demo_avr-0.0.7/packaging_demo_avr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.4/pyproject.toml` & `packaging_demo_avr-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 [build-system]
 # Minimum requirements for the build system to execute
 requires = ["setuptools>=61.0.0", "wheel"]
 # default value of build-backend is "setuptools.build_meta"
 build-backend = "setuptools.build_meta"
 
-# include-package-data defaults to true, not needed to add in toml file
-[tool.setuptools]
-include-package-data = true
-
-[tool.setuptools.package-data]
-packaging_demo = ["**/*.json"]
 
 [project]
 name = "packaging-demo-avr"
 authors = [{ name = "Amit Vikram Raj", email = "avr13405@gmail.com" }]
 description = "Demo for Python Packaging"
 readme = "README.md"
 requires-python = ">=3.8"
-keywords = ["one", "two"]
+keywords = [
+    "python", "bash", "makefile", "pypi", "ci-cd", "setuptools", "wheels",
+    "package-development", "github-actions", "pypi-package", "pre-commit-hooks",
+    "pyproject-toml", "gitactions-workflow", "github-actions-enabled", "pre-commit-ci",
+    "pre-commit-config"
+]
 license = { text = "MIT" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = ["numpy", "fastapi", 'importlib-metadata; python_version<"3.10"']
 dynamic = ["version"]
 # version = "0.0.3"
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html#dynamic-metadata
 
+[project.urls]
+# Ref: https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
+Repository = "https://github.com/avr2002/python-packaging"
+Documentation = "https://github.com/avr2002/python-packaging/blob/main/README.md"
+
 [tool.setuptools.dynamic]
 # every while making changes in package, you can change the verison in one of these files
 # version = {attr = "packaging_demo.VERSION"} # version read by 'packaging_demo/__init__.py' file
 version = {file  = ["version.txt"]} # version read by 'version.txt' file in root folder
 
+# include-package-data defaults to true, not needed to add in toml file
+[tool.setuptools]
+include-package-data = true
+
+# adding data files in our package; moving from MANIFEST.in to toml file
+[tool.setuptools.package-data]
+packaging_demo = ["**/*.json"]
+
+
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 release = ["build", "twine"]
 static-code-qa = ["pre-commit"]
 # for developement
-dev = ["ruff", "mypy", "black", "packaging-demo[test, release, static-code-qa]"]
+dev = ["ruff", "mypy", "black", "packaging-demo-avr[test, release, static-code-qa]"]
 # plugin based architecture
 colors = ["rich"]
 # install all dependencies
-all = ["packaging-demo[dev, colors]"]
+all = ["packaging-demo-avr[dev, colors]"]
 
 
 # Adding ruff.toml to pyproject.toml
 [tool.ruff]
 line-length = 119
 
 [tool.ruff.lint]
```


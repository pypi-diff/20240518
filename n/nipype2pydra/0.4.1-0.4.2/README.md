# Comparing `tmp/nipype2pydra-0.4.1.tar.gz` & `tmp/nipype2pydra-0.4.2.tar.gz`

## Comparing `nipype2pydra-0.4.1.tar` & `nipype2pydra-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/_version.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/exceptions.py
--rw-r--r--   0        0        0    14364 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/helpers.py
--rw-r--r--   0        0        0    40316 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/package.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/testing.py
--rw-r--r--   0        0        0    45837 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/workflow.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/cli/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/cli/base.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/cli/convert.py
--rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/cli/pkg_gen.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/__init__.py
--rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/base.py
--rw-r--r--   0        0        0    16959 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/function.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/loaders.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/shell_command.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/compute_dvars.yaml
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/non_steady_state_detector_callables.py
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/tsnr.yaml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/tsnr_callables.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/interface/tests/test_interface.py
--rw-r--r--   0        0        0    45492 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/__init__.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/NOTICE
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/README.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/init.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/pkg_gen/tests/test_pkg_gen.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/statements/__init__.py
--rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/statements/imports.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/statements/misc.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/statements/utility.py
--rw-r--r--   0        0        0    31670 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/statements/workflow_build.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/tests/test_package.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/utils/__init__.py
--rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/utils/misc.py
--rw-r--r--   0        0        0    23704 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/utils/symbols.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/utils/tests/test_utils_imports.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/nipype2pydra/utils/tests/test_utils_misc.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/LICENSE
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/README.rst
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 nipype2pydra-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/_version.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/exceptions.py
+-rw-r--r--   0        0        0    14364 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/helpers.py
+-rw-r--r--   0        0        0    40316 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/package.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/testing.py
+-rw-r--r--   0        0        0    45837 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/workflow.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/cli/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/cli/base.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/cli/convert.py
+-rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/cli/pkg_gen.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/__init__.py
+-rw-r--r--   0        0        0    36880 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/base.py
+-rw-r--r--   0        0        0    16959 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/function.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/loaders.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/shell_command.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/compute_dvars.yaml
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/non_steady_state_detector_callables.py
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/tsnr.yaml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/tsnr_callables.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/interface/tests/test_interface.py
+-rw-r--r--   0        0        0    45492 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/__init__.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/NOTICE
+-rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/README.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/init.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/nipype-auto-convert-requirements.txt
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/fileformats/medimage_CHANGEME/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/fileformats/extras/medimage_CHANGEME/__init__.py
+-rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/pkg_gen/tests/test_pkg_gen.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/statements/__init__.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/statements/imports.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/statements/misc.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/statements/utility.py
+-rw-r--r--   0        0        0    31670 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/statements/workflow_build.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/tests/test_package.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/utils/__init__.py
+-rw-r--r--   0        0        0    16939 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/utils/misc.py
+-rw-r--r--   0        0        0    23704 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/utils/symbols.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/utils/tests/test_utils_imports.py
+-rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/nipype2pydra/utils/tests/test_utils_misc.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/README.rst
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 nipype2pydra-0.4.2/PKG-INFO
```

### Comparing `nipype2pydra-0.4.1/nipype2pydra/helpers.py` & `nipype2pydra-0.4.2/nipype2pydra/helpers.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/package.py` & `nipype2pydra-0.4.2/nipype2pydra/package.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/testing.py` & `nipype2pydra-0.4.2/nipype2pydra/testing.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/workflow.py` & `nipype2pydra-0.4.2/nipype2pydra/workflow.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/cli/convert.py` & `nipype2pydra-0.4.2/nipype2pydra/cli/convert.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/cli/pkg_gen.py` & `nipype2pydra-0.4.2/nipype2pydra/cli/pkg_gen.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/__init__.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/base.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/base.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/function.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/function.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/loaders.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/loaders.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/shell_command.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/shell_command.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/compute_dvars.yaml` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/compute_dvars.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/compute_dvars_callables.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/framewise_displacement.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/framewise_displacement_callables.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/non_steady_state_detector.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/tsnr.yaml` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/tsnr.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/nipype-ports/tsnr_callables.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/nipype-ports/tsnr_callables.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/interface/tests/test_interface.py` & `nipype2pydra-0.4.2/nipype2pydra/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/__init__.py` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/README.rst` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/init.py` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/init.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-interface.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/gh_workflows/ci-cd-workflow.yaml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/conftest_.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/related-packages/fileformats-extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/resources/templates/tools/report_progress.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/pkg_gen/tests/test_pkg_gen.py` & `nipype2pydra-0.4.2/nipype2pydra/pkg_gen/tests/test_pkg_gen.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/statements/__init__.py` & `nipype2pydra-0.4.2/nipype2pydra/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/statements/imports.py` & `nipype2pydra-0.4.2/nipype2pydra/statements/imports.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/statements/misc.py` & `nipype2pydra-0.4.2/nipype2pydra/statements/misc.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/statements/utility.py` & `nipype2pydra-0.4.2/nipype2pydra/statements/utility.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/statements/workflow_build.py` & `nipype2pydra-0.4.2/nipype2pydra/statements/workflow_build.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/tests/test_package.py` & `nipype2pydra-0.4.2/nipype2pydra/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/utils/__init__.py` & `nipype2pydra-0.4.2/nipype2pydra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/utils/misc.py` & `nipype2pydra-0.4.2/nipype2pydra/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/utils/symbols.py` & `nipype2pydra-0.4.2/nipype2pydra/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/utils/tests/test_utils_imports.py` & `nipype2pydra-0.4.2/nipype2pydra/utils/tests/test_utils_imports.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/nipype2pydra/utils/tests/test_utils_misc.py` & `nipype2pydra-0.4.2/nipype2pydra/utils/tests/test_utils_misc.py`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/LICENSE` & `nipype2pydra-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/README.rst` & `nipype2pydra-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `nipype2pydra-0.4.1/pyproject.toml` & `nipype2pydra-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "PyYAML>=6.0",
     "fileformats >=0.8",
     "fileformats-medimage >=0.4",
     "fileformats-datascience",
     "requests>=2.31.0",
     "traits",
     "tqdm",
+    "toml",
     "typing_extensions",
 ]
 license = { file = "LICENSE" }
 authors = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 maintainers = [{ name = "Thomas G. Close", email = "tom.g.close@gmail.com" }]
 keywords = ["nipype", "data", "pydra", "workflows", "converters"]
 classifiers = [
```

### Comparing `nipype2pydra-0.4.1/PKG-INFO` & `nipype2pydra-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nipype2pydra
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tool for converting Nipype tasks and workflows into Pydra syntax
 Project-URL: repository, https://github.com/nipype/nipype2pydra
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -116,14 +116,15 @@
 Requires-Dist: fileformats-datascience
 Requires-Dist: fileformats-medimage>=0.4
 Requires-Dist: fileformats>=0.8
 Requires-Dist: nipype
 Requires-Dist: pydra
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: requests>=2.31.0
+Requires-Dist: toml
 Requires-Dist: tqdm
 Requires-Dist: traits
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
```


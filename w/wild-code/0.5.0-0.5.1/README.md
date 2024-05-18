# Comparing `tmp/wild_code-0.5.0.tar.gz` & `tmp/wild_code-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.5.0.tar", last modified: Sat May 18 19:18:49 2024, max compression
+gzip compressed data, was "wild_code-0.5.1.tar", last modified: Sat May 18 20:42:30 2024, max compression
```

## Comparing `wild_code-0.5.0.tar` & `wild_code-0.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:06.463576 wild_code-0.5.0/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-18 18:14:50.000000 wild_code-0.5.0/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.596301 wild_code-0.5.0/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.595851 wild_code-0.5.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-18 18:14:50.000000 wild_code-0.5.0/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-18 18:14:50.000000 wild_code-0.5.0/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-18 18:14:50.000000 wild_code-0.5.0/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      770 2024-05-18 18:14:50.000000 wild_code-0.5.0/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-18 18:14:50.000000 wild_code-0.5.0/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-18 18:14:50.000000 wild_code-0.5.0/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    11035 2024-05-18 19:16:06.457409 wild_code-0.5.0/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9966 2024-05-18 18:14:50.000000 wild_code-0.5.0/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-18 18:14:50.000000 wild_code-0.5.0/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-18 18:14:50.000000 wild_code-0.5.0/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      175 2024-05-18 18:14:50.000000 wild_code-0.5.0/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      809 2024-05-18 18:14:50.000000 wild_code-0.5.0/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1231 2024-05-18 19:16:06.480210 wild_code-0.5.0/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.600842 wild_code-0.5.0/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-18 18:14:50.000000 wild_code-0.5.0/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-18 18:14:50.000000 wild_code-0.5.0/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-18 18:14:50.000000 wild_code-0.5.0/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:06.431584 wild_code-0.5.0/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    11035 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      284 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.632185 wild_code-0.5.0/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-18 19:16:05.000000 wild_code-0.5.0/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.621202 wild_code-0.5.0/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6048 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1975 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.626586 wild_code-0.5.0/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7259 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    10640 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8688 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.639876 wild_code-0.5.0/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.639447 wild_code-0.5.0/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6205 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    16914 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8417 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:48.016506 wild_code-0.5.1/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-18 18:14:50.000000 wild_code-0.5.1/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.229497 wild_code-0.5.1/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.229004 wild_code-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-18 18:14:50.000000 wild_code-0.5.1/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-18 18:14:50.000000 wild_code-0.5.1/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-18 18:14:50.000000 wild_code-0.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-18 18:14:50.000000 wild_code-0.5.1/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-18 18:14:50.000000 wild_code-0.5.1/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-18 18:14:50.000000 wild_code-0.5.1/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-18 18:14:50.000000 wild_code-0.5.1/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      770 2024-05-18 18:14:50.000000 wild_code-0.5.1/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-18 18:14:50.000000 wild_code-0.5.1/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-18 18:14:50.000000 wild_code-0.5.1/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    11039 2024-05-18 20:39:48.011038 wild_code-0.5.1/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9970 2024-05-18 19:34:52.000000 wild_code-0.5.1/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-18 18:14:50.000000 wild_code-0.5.1/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-18 18:14:50.000000 wild_code-0.5.1/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      175 2024-05-18 18:14:50.000000 wild_code-0.5.1/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      789 2024-05-18 20:30:17.000000 wild_code-0.5.1/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1231 2024-05-18 20:39:48.031611 wild_code-0.5.1/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.234027 wild_code-0.5.1/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-18 18:14:50.000000 wild_code-0.5.1/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-18 18:14:50.000000 wild_code-0.5.1/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-18 18:14:50.000000 wild_code-0.5.1/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.992985 wild_code-0.5.1/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    11039 2024-05-18 20:39:46.000000 wild_code-0.5.1/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-18 20:39:47.000000 wild_code-0.5.1/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-18 20:39:47.000000 wild_code-0.5.1/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-18 20:39:47.000000 wild_code-0.5.1/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      284 2024-05-18 20:39:47.000000 wild_code-0.5.1/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-18 20:39:47.000000 wild_code-0.5.1/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.262870 wild_code-0.5.1/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-18 20:39:46.000000 wild_code-0.5.1/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.251781 wild_code-0.5.1/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6048 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1975 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.257639 wild_code-0.5.1/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7259 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    10640 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8688 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.269732 wild_code-0.5.1/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 20:39:47.269244 wild_code-0.5.1/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6285 2024-05-18 19:34:24.000000 wild_code-0.5.1/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    16914 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8425 2024-05-18 20:32:37.000000 wild_code-0.5.1/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-18 18:14:50.000000 wild_code-0.5.1/wildcode/syncheck.py
```

### Comparing `wild_code-0.5.0/.dockerignore` & `wild_code-0.5.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.5.1/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.5.1/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.5.1/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/.gitignore` & `wild_code-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/Dockerfile` & `wild_code-0.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/LICENSE` & `wild_code-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/PKG-INFO` & `wild_code-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.5.0
+Version: 0.5.1
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -132,15 +132,15 @@
     --bs [bs] \
     --temperature [temp] \
     --n_samples [n_samples] \
     --resume \
     --backend [vllm|hf|openai|mistral|anthropic|google]
     --tp [gpu_number]
 ```
-The generated code samples will be stored in a file named `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`.
+The generated code samples will be stored in a file named `[model_name]--wildcodebench-[nl2c|c2c]--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.5.0 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.5.1 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -59,16 +59,16 @@
 ### Code Generation You are suggested to use `flash-attn` for generating code
 samples. ```shell pip install -U flash-attn ``` To generate code samples from a
 model, you can use the following command: ```shell wildcode.generate \ --model
 [model_name] \ --dataset [wildcodebench] \ --nl2code [False|True] \ --greedy \
 --bs [bs] \ --temperature [temp] \ --n_samples [n_samples] \ --resume \ --
 backend [vllm|hf|openai|mistral|anthropic|google] --tp [gpu_number] ``` The
 generated code samples will be stored in a file named `[model_name]--
-wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
-`problem`? :: click to expand ::
+wildcodebench-[nl2c|c2c]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure
+of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench-[task]--
 [backend]-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the
 keys of `get_wildcodebench()` > 2. `solution` (optional): Self-contained
```

### Comparing `wild_code-0.5.0/README.md` & `wild_code-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     --bs [bs] \
     --temperature [temp] \
     --n_samples [n_samples] \
     --resume \
     --backend [vllm|hf|openai|mistral|anthropic|google]
     --tp [gpu_number]
 ```
-The generated code samples will be stored in a file named `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`.
+The generated code samples will be stored in a file named `[model_name]--wildcodebench-[nl2c|c2c]--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
```

#### html2text {}

```diff
@@ -45,16 +45,16 @@
 ### Code Generation You are suggested to use `flash-attn` for generating code
 samples. ```shell pip install -U flash-attn ``` To generate code samples from a
 model, you can use the following command: ```shell wildcode.generate \ --model
 [model_name] \ --dataset [wildcodebench] \ --nl2code [False|True] \ --greedy \
 --bs [bs] \ --temperature [temp] \ --n_samples [n_samples] \ --resume \ --
 backend [vllm|hf|openai|mistral|anthropic|google] --tp [gpu_number] ``` The
 generated code samples will be stored in a file named `[model_name]--
-wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
-`problem`? :: click to expand ::
+wildcodebench-[nl2c|c2c]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure
+of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench-[task]--
 [backend]-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the
 keys of `get_wildcodebench()` > 2. `solution` (optional): Self-contained
```

### Comparing `wild_code-0.5.0/release.sh` & `wild_code-0.5.1/release.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/run.sh` & `wild_code-0.5.1/run.sh`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,26 @@
   BASE_MODEL=$(echo $MODEL | cut -d'/' -f2)
 else
   ORG=""
   BASE_MODEL=$MODEL
 fi
 
 if [ "$NL2CODE" = "True" ]; then
-  FILE_HEADER=$ORG$BASE_MODEL--$DATASET-NL2C--$BACKEND-$TEMP-$N_SAMPLES
+  FILE_HEADER=$ORG$BASE_MODEL--$DATASET-nl2c--$BACKEND-$TEMP-$N_SAMPLES
 else
-  FILE_HEADER=$ORG$BASE_MODEL--$DATASET-C2C--$BACKEND-$TEMP-$N_SAMPLES
+  FILE_HEADER=$ORG$BASE_MODEL--$DATASET-c2c--$BACKEND-$TEMP-$N_SAMPLES
 fi
 
 echo $FILE_HEADER
 wildcode.generate \
   --tp $NUM_GPU \
   --model $MODEL \
   --bs $BS \
   --temperature $TEMP \
   --n_samples $N_SAMPLES \
   --resume \
   --dataset $DATASET \
   --nl2code $NL2CODE \
-  --id_range 0 10 \
   --backend $BACKEND 
 
 wildcode.sanitize --samples $FILE_HEADER.jsonl
 wildcode.evaluate --dataset $DATASET --samples $FILE_HEADER-sanitized.jsonl
```

### Comparing `wild_code-0.5.0/setup.cfg` & `wild_code-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/tests/test_legacy_sanitizer.py` & `wild_code-0.5.1/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/tests/test_treesitter_sanitizer.py` & `wild_code-0.5.1/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wild_code.egg-info/PKG-INFO` & `wild_code-0.5.1/wild_code.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.5.0
+Version: 0.5.1
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -132,15 +132,15 @@
     --bs [bs] \
     --temperature [temp] \
     --n_samples [n_samples] \
     --resume \
     --backend [vllm|hf|openai|mistral|anthropic|google]
     --tp [gpu_number]
 ```
-The generated code samples will be stored in a file named `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`.
+The generated code samples will be stored in a file named `[model_name]--wildcodebench-[nl2c|c2c]--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.5.0 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.5.1 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -59,16 +59,16 @@
 ### Code Generation You are suggested to use `flash-attn` for generating code
 samples. ```shell pip install -U flash-attn ``` To generate code samples from a
 model, you can use the following command: ```shell wildcode.generate \ --model
 [model_name] \ --dataset [wildcodebench] \ --nl2code [False|True] \ --greedy \
 --bs [bs] \ --temperature [temp] \ --n_samples [n_samples] \ --resume \ --
 backend [vllm|hf|openai|mistral|anthropic|google] --tp [gpu_number] ``` The
 generated code samples will be stored in a file named `[model_name]--
-wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
-`problem`? :: click to expand ::
+wildcodebench-[nl2c|c2c]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure
+of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench-[task]--
 [backend]-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the
 keys of `get_wildcodebench()` > 2. `solution` (optional): Self-contained
```

### Comparing `wild_code-0.5.0/wild_code.egg-info/SOURCES.txt` & `wild_code-0.5.1/wild_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/data/utils.py` & `wild_code-0.5.1/wildcode/data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/data/wildcodebench.py` & `wild_code-0.5.1/wildcode/data/wildcodebench.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/eval/__init__.py` & `wild_code-0.5.1/wildcode/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/eval/utils.py` & `wild_code-0.5.1/wildcode/eval/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/evaluate.py` & `wild_code-0.5.1/wildcode/evaluate.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/gen/__init__.py` & `wild_code-0.5.1/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/gen/util/__init__.py` & `wild_code-0.5.1/wildcode/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/gen/util/anthropic_request.py` & `wild_code-0.5.1/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/gen/util/openai_request.py` & `wild_code-0.5.1/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/generate.py` & `wild_code-0.5.1/wildcode/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,19 @@
         backend=args.backend,
         batch_size=args.bs,
         temperature=args.temperature,
         dataset=args.dataset,
         base_url=args.base_url,
         tp=args.tp,
     )
-    save_path = args.model.replace("/", "--") + f"--{args.dataset}--" +f"{args.backend}-{args.temperature}-{args.n_samples}.jsonl"
+    if args.nl2code:
+        task = "nl2c"
+    else:
+        task = "c2c"
+    save_path = args.model.replace("/", "--") + f"--{args.dataset}-{task}--{args.backend}-{args.temperature}-{args.n_samples}.jsonl"
     
     codegen(
         model=model_runner,
         save_path=save_path,
         dataset=args.dataset,
         nl2code=args.nl2code,
         greedy=args.greedy,
```

### Comparing `wild_code-0.5.0/wildcode/inspect.py` & `wild_code-0.5.1/wildcode/inspect.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/lecacy_sanitize.py` & `wild_code-0.5.1/wildcode/lecacy_sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/model.py` & `wild_code-0.5.1/wildcode/model.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.5.0/wildcode/sanitize.py` & `wild_code-0.5.1/wildcode/sanitize.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     for node in traverse_nodes:
         if node.type == RETURN_TYPE:
             return True
     return False
 
 
 def sanitize(code: str, entrypoint: Optional[str] = None) -> str:
-    code = code_extract(code)
+    code = code_extract(code.strip())
     code_bytes = bytes(code, "utf8")
     parser = get_parser("python")
     tree = parser.parse(code_bytes)
     class_names = set()
     function_names = set()
     variable_names = set()
```

### Comparing `wild_code-0.5.0/wildcode/syncheck.py` & `wild_code-0.5.1/wildcode/syncheck.py`

 * *Files identical despite different names*


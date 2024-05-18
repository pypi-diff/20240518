# Comparing `tmp/wild_code-0.4.5.tar.gz` & `tmp/wild_code-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.4.5.tar", last modified: Wed May 15 19:36:56 2024, max compression
+gzip compressed data, was "wild_code-0.5.0.tar", last modified: Sat May 18 19:18:49 2024, max compression
```

## Comparing `wild_code-0.4.5.tar` & `wild_code-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.991880 wild_code-0.4.5/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-15 18:58:13.000000 wild_code-0.4.5/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.156472 wild_code-0.4.5/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.156041 wild_code-0.4.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-15 15:44:35.000000 wild_code-0.4.5/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-15 15:44:35.000000 wild_code-0.4.5/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-15 15:44:35.000000 wild_code-0.4.5/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-15 15:44:35.000000 wild_code-0.4.5/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      764 2024-05-15 18:38:24.000000 wild_code-0.4.5/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-15 15:44:35.000000 wild_code-0.4.5/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-15 15:44:35.000000 wild_code-0.4.5/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10853 2024-05-15 19:34:15.987412 wild_code-0.4.5/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9819 2024-05-15 15:44:35.000000 wild_code-0.4.5/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-15 15:44:35.000000 wild_code-0.4.5/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-15 15:44:35.000000 wild_code-0.4.5/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      156 2024-05-15 15:44:35.000000 wild_code-0.4.5/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      777 2024-05-15 18:34:15.000000 wild_code-0.4.5/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1210 2024-05-15 19:34:16.007014 wild_code-0.4.5/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.160993 wild_code-0.4.5/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-15 15:44:35.000000 wild_code-0.4.5/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-15 15:44:35.000000 wild_code-0.4.5/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-15 15:44:35.000000 wild_code-0.4.5/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.972909 wild_code-0.4.5/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10853 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-15 19:34:15.000000 wild_code-0.4.5/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-15 19:34:14.000000 wild_code-0.4.5/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.188645 wild_code-0.4.5/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-15 19:34:14.000000 wild_code-0.4.5/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.179066 wild_code-0.4.5/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.184183 wild_code-0.4.5/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7216 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7110 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8190 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.197276 wild_code-0.4.5/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-15 19:34:15.196851 wild_code-0.4.5/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5592 2024-05-15 18:12:27.000000 wild_code-0.4.5/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    16130 2024-05-15 18:32:02.000000 wild_code-0.4.5/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-15 15:44:35.000000 wild_code-0.4.5/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:06.463576 wild_code-0.5.0/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-18 18:14:50.000000 wild_code-0.5.0/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.596301 wild_code-0.5.0/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.595851 wild_code-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-18 18:14:50.000000 wild_code-0.5.0/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-18 18:14:50.000000 wild_code-0.5.0/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-18 18:14:50.000000 wild_code-0.5.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-18 18:14:50.000000 wild_code-0.5.0/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      770 2024-05-18 18:14:50.000000 wild_code-0.5.0/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-18 18:14:50.000000 wild_code-0.5.0/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-18 18:14:50.000000 wild_code-0.5.0/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    11035 2024-05-18 19:16:06.457409 wild_code-0.5.0/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9966 2024-05-18 18:14:50.000000 wild_code-0.5.0/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-18 18:14:50.000000 wild_code-0.5.0/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-18 18:14:50.000000 wild_code-0.5.0/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      175 2024-05-18 18:14:50.000000 wild_code-0.5.0/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      809 2024-05-18 18:14:50.000000 wild_code-0.5.0/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1231 2024-05-18 19:16:06.480210 wild_code-0.5.0/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.600842 wild_code-0.5.0/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-18 18:14:50.000000 wild_code-0.5.0/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-18 18:14:50.000000 wild_code-0.5.0/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-18 18:14:50.000000 wild_code-0.5.0/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:06.431584 wild_code-0.5.0/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    11035 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      284 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-18 19:16:05.000000 wild_code-0.5.0/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.632185 wild_code-0.5.0/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-18 19:16:05.000000 wild_code-0.5.0/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.621202 wild_code-0.5.0/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6048 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1975 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.626586 wild_code-0.5.0/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7259 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    10640 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8688 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.639876 wild_code-0.5.0/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-18 19:16:05.639447 wild_code-0.5.0/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6205 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    16914 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8417 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-18 18:14:50.000000 wild_code-0.5.0/wildcode/syncheck.py
```

### Comparing `wild_code-0.4.5/.dockerignore` & `wild_code-0.5.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.5.0/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.5.0/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/.gitignore` & `wild_code-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/Dockerfile` & `wild_code-0.5.0/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 RUN pip install --upgrade pip
 
 # Add a new user "wildcodeuser"
 RUN adduser --disabled-password --gecos "" wildcodeuser
 
 COPY . /wildcode
 
-RUN cd /wildcode && pip install . && pip install -r https://raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/requirements.txt
+RUN cd /wildcode && pip install . && pip install -U -I -r https://raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/requirements.txt
 
 # Pre-install the dataset
 RUN python3 -c "from wildcode.data import get_wildcodebench; get_wildcodebench()"
 
 RUN chown -R wildcodeuser:wildcodeuser /wildcode
 USER wildcodeuser
```

### Comparing `wild_code-0.4.5/LICENSE` & `wild_code-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/PKG-INFO` & `wild_code-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.5
+Version: 0.5.0
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,32 +19,30 @@
 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0
 Requires-Dist: fire>=0.6.0
 Requires-Dist: openai>=1.11.1
 Requires-Dist: rich>=12.3.0
 Requires-Dist: tree_sitter_languages>=1.10.2
 Requires-Dist: tree-sitter==0.21.3
+Requires-Dist: Pympler>=1.0.1
 Requires-Dist: accelerate
 Requires-Dist: vllm
 Requires-Dist: anthropic
 Requires-Dist: mistralai
 Requires-Dist: stop-sequencer
-Requires-Dist: Pympler>=1.0.1
+Requires-Dist: google-generativeai
 
 # 🌳WildCodeBench
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
 > Please use WildCode with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus), WildCode has a much less constrained execution environment to support tasks with diverse library dependencies. This may lead to security risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/) to run the evaluation.
 
-> [!WARNING]
-> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task.
-
 <p align="center">
     <a href="https://pypi.org/project/wild-code/"><img src="https://img.shields.io/pypi/v/wild-code?color=g"></a>
     <a href="https://hub.docker.com/r/terryzho/wildcode" title="Docker"><img src="https://img.shields.io/docker/image-size/terryzho/wildcode"></a>
     <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/wild-code"></a>
 </p>
 
 <p align="center">
@@ -122,17 +120,27 @@
 ```shell
 pip install -U flash-attn
 ```
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
+wildcode.generate \
+    --model [model_name] \
+    --dataset [wildcodebench] \
+    --nl2code [False|True] \
+    --greedy \
+    --bs [bs] \
+    --temperature [temp] \
+    --n_samples [n_samples] \
+    --resume \
+    --backend [vllm|hf|openai|mistral|anthropic|google]
+    --tp [gpu_number]
 ```
-The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
+The generated code samples will be stored in a file named `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
@@ -141,15 +149,15 @@
 + `test` is the `unittest` test case
 
 </div>
 </details>
 
 > [!Note]
 >
-> **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
+> **Expected Schema of `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`**
 >
 > 1. `task_id`: Task ID, which are the keys of `get_wildcodebench()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
 >    * Example: `{"task_id": "WildCodeBench/?", "solution": "def f():\n    return 1"}`
 
 ### Code Post-processing
 
@@ -275,14 +283,16 @@
 
 We will share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
 
 ## Known Issues
 
 - [ ] We notice that some tasks heavily use memory for scientific modeling during testing. It will lead to timeout issues on some machines. If you get an error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.` in Tensorflow, it is very likely due to the memory issue. Try to allocate more memory to the process or reduce the number of parallel processes.
 
+- [ ] Due to the flakes in the evaluation, the execution results may vary slightly (~0.5%) between runs. We are working on improving the evaluation stability.
+
 ## 📜 Citation
 
 ```bibtex
 ```
 
 ## 🙏 Acknowledgement
```

#### html2text {}

```diff
@@ -1,30 +1,28 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.5 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.5.0 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
 appdirs>=1.4.4 Requires-Dist: numpy>=1.19.5 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0 Requires-Dist: fire>=0.6.0 Requires-Dist:
 openai>=1.11.1 Requires-Dist: rich>=12.3.0 Requires-Dist:
 tree_sitter_languages>=1.10.2 Requires-Dist: tree-sitter==0.21.3 Requires-Dist:
-accelerate Requires-Dist: vllm Requires-Dist: anthropic Requires-Dist:
-mistralai Requires-Dist: stop-sequencer Requires-Dist: Pympler>=1.0.1 #
-ð³WildCodeBench > [!WARNING] > The project is under active development.
-Please check back later for more updates. > [!WARNING] > Please use WildCode
-with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
-WildCode has a much less constrained execution environment to support tasks
-with diverse library dependencies. This may lead to security risks. We
-recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
-) to run the evaluation. > [!WARNING] > WildCode framework currently only
-supports the Code2Code generation task. We are working on adding the NL2Code
-task.
+Pympler>=1.0.1 Requires-Dist: accelerate Requires-Dist: vllm Requires-Dist:
+anthropic Requires-Dist: mistralai Requires-Dist: stop-sequencer Requires-Dist:
+google-generativeai # ð³WildCodeBench > [!WARNING] > The project is under
+active development. Please check back later for more updates. > [!WARNING] >
+Please use WildCode with caution. Different from [EvalPlus](https://github.com/
+evalplus/evalplus), WildCode has a much less constrained execution environment
+to support tasks with diverse library dependencies. This may lead to security
+risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/
+get-docker/) to run the evaluation.
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_w_i_l_d_-_c_o_d_e_?_c_o_l_o_r_=_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_e_r_r_y_z_h_o_/_w_i_l_d_c_o_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_w_i_l_d_-_c_o_d_e_]
  _ð___³_A_b_o_u_t â¢ _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð____F_a_i_l_u_r_e_ _i_n_s_p_e_c_t_i_o_n â¢
            _ð____K_n_o_w_n_ _i_s_s_u_e_s â¢ _ð____C_i_t_a_t_i_o_n â¢ _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
 ## About ### WildCodeBench WildCodeBench is a rigorous benchmark for code
 generation with realistic constraints in the wild. It aims to evaluate the true
 programming capabilities of large language models (LLMs) in a more realistic
@@ -56,37 +54,38 @@
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
 ### Code Generation You are suggested to use `flash-attn` for generating code
 samples. ```shell pip install -U flash-attn ``` To generate code samples from a
-model, you can use the following command: ```shell wildcode.generate --model
-[model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp]
---n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
-``` The generated code samples will be stored in a file named `[model_name]--
-wildcodebench--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
+model, you can use the following command: ```shell wildcode.generate \ --model
+[model_name] \ --dataset [wildcodebench] \ --nl2code [False|True] \ --greedy \
+--bs [bs] \ --temperature [temp] \ --n_samples [n_samples] \ --resume \ --
+backend [vllm|hf|openai|mistral|anthropic|google] --tp [gpu_number] ``` The
+generated code samples will be stored in a file named `[model_name]--
+wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
 `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
-> [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
-`get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
-(usually including the prompt) > * Example: `{"task_id": "WildCodeBench/?",
-"solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated text
-may not be compilable code for including natural language lines or incomplete
-extra code. We provide a tool namely `wildcode.sanitize` to clean up the code:
-```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize --samples
-samples.jsonl # Sanitized code will be produced to `samples-sanitized.jsonl` #
-ð¡ If you are storing codes in directories: wildcode.sanitize --samples /
-path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/
-vicuna-[??]b_temp_[??]-sanitized` ``` ð Checking the compilability of post-
-processed code:: click to expand ::
+> [!Note] > > **Expected Schema of `[model_name]--wildcodebench-[task]--
+[backend]-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the
+keys of `get_wildcodebench()` > 2. `solution` (optional): Self-contained
+solution (usually including the prompt) > * Example: `{"task_id":
+"WildCodeBench/?", "solution": "def f():\n return 1"}` ### Code Post-processing
+LLM-generated text may not be compilable code for including natural language
+lines or incomplete extra code. We provide a tool namely `wildcode.sanitize` to
+clean up the code: ```shell # ð¡ If you are storing codes in jsonl:
+wildcode.sanitize --samples samples.jsonl # Sanitized code will be produced to
+`samples-sanitized.jsonl` # ð¡ If you are storing codes in directories:
+wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
+will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
+Checking the compilability of post-processed code:: click to expand ::
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
@@ -128,9 +127,11 @@
 generated Code We will share pre-generated code samples from LLMs we have
 [evaluated](https://wildcodebench.github.io/leaderboard.html): ## Known Issues
 - [ ] We notice that some tasks heavily use memory for scientific modeling
 during testing. It will lead to timeout issues on some machines. If you get an
 error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via
 pthread_create() failed.` in Tensorflow, it is very likely due to the memory
 issue. Try to allocate more memory to the process or reduce the number of
-parallel processes. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
+parallel processes. - [ ] Due to the flakes in the evaluation, the execution
+results may vary slightly (~0.5%) between runs. We are working on improving the
+evaluation stability. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
 [EvalPlus](https://github.com/evalplus/evalplus)
```

### Comparing `wild_code-0.4.5/README.md` & `wild_code-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
 > Please use WildCode with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus), WildCode has a much less constrained execution environment to support tasks with diverse library dependencies. This may lead to security risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/) to run the evaluation.
 
-> [!WARNING]
-> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task.
-
 <p align="center">
     <a href="https://pypi.org/project/wild-code/"><img src="https://img.shields.io/pypi/v/wild-code?color=g"></a>
     <a href="https://hub.docker.com/r/terryzho/wildcode" title="Docker"><img src="https://img.shields.io/docker/image-size/terryzho/wildcode"></a>
     <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/wild-code"></a>
 </p>
 
 <p align="center">
@@ -90,17 +87,27 @@
 ```shell
 pip install -U flash-attn
 ```
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
+wildcode.generate \
+    --model [model_name] \
+    --dataset [wildcodebench] \
+    --nl2code [False|True] \
+    --greedy \
+    --bs [bs] \
+    --temperature [temp] \
+    --n_samples [n_samples] \
+    --resume \
+    --backend [vllm|hf|openai|mistral|anthropic|google]
+    --tp [gpu_number]
 ```
-The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
+The generated code samples will be stored in a file named `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
@@ -109,15 +116,15 @@
 + `test` is the `unittest` test case
 
 </div>
 </details>
 
 > [!Note]
 >
-> **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
+> **Expected Schema of `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`**
 >
 > 1. `task_id`: Task ID, which are the keys of `get_wildcodebench()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
 >    * Example: `{"task_id": "WildCodeBench/?", "solution": "def f():\n    return 1"}`
 
 ### Code Post-processing
 
@@ -243,14 +250,16 @@
 
 We will share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
 
 ## Known Issues
 
 - [ ] We notice that some tasks heavily use memory for scientific modeling during testing. It will lead to timeout issues on some machines. If you get an error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.` in Tensorflow, it is very likely due to the memory issue. Try to allocate more memory to the process or reduce the number of parallel processes.
 
+- [ ] Due to the flakes in the evaluation, the execution results may vary slightly (~0.5%) between runs. We are working on improving the evaluation stability.
+
 ## 📜 Citation
 
 ```bibtex
 ```
 
 ## 🙏 Acknowledgement
```

#### html2text {}

```diff
@@ -1,16 +1,14 @@
 # ð³WildCodeBench > [!WARNING] > The project is under active development.
 Please check back later for more updates. > [!WARNING] > Please use WildCode
 with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
 WildCode has a much less constrained execution environment to support tasks
 with diverse library dependencies. This may lead to security risks. We
 recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
-) to run the evaluation. > [!WARNING] > WildCode framework currently only
-supports the Code2Code generation task. We are working on adding the NL2Code
-task.
+) to run the evaluation.
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_w_i_l_d_-_c_o_d_e_?_c_o_l_o_r_=_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_e_r_r_y_z_h_o_/_w_i_l_d_c_o_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_w_i_l_d_-_c_o_d_e_]
  _ð___³_A_b_o_u_t â¢ _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð____F_a_i_l_u_r_e_ _i_n_s_p_e_c_t_i_o_n â¢
            _ð____K_n_o_w_n_ _i_s_s_u_e_s â¢ _ð____C_i_t_a_t_i_o_n â¢ _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
 ## About ### WildCodeBench WildCodeBench is a rigorous benchmark for code
 generation with realistic constraints in the wild. It aims to evaluate the true
 programming capabilities of large language models (LLMs) in a more realistic
@@ -42,37 +40,38 @@
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
 ### Code Generation You are suggested to use `flash-attn` for generating code
 samples. ```shell pip install -U flash-attn ``` To generate code samples from a
-model, you can use the following command: ```shell wildcode.generate --model
-[model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp]
---n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
-``` The generated code samples will be stored in a file named `[model_name]--
-wildcodebench--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
+model, you can use the following command: ```shell wildcode.generate \ --model
+[model_name] \ --dataset [wildcodebench] \ --nl2code [False|True] \ --greedy \
+--bs [bs] \ --temperature [temp] \ --n_samples [n_samples] \ --resume \ --
+backend [vllm|hf|openai|mistral|anthropic|google] --tp [gpu_number] ``` The
+generated code samples will be stored in a file named `[model_name]--
+wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
 `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
-> [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
-`get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
-(usually including the prompt) > * Example: `{"task_id": "WildCodeBench/?",
-"solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated text
-may not be compilable code for including natural language lines or incomplete
-extra code. We provide a tool namely `wildcode.sanitize` to clean up the code:
-```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize --samples
-samples.jsonl # Sanitized code will be produced to `samples-sanitized.jsonl` #
-ð¡ If you are storing codes in directories: wildcode.sanitize --samples /
-path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/
-vicuna-[??]b_temp_[??]-sanitized` ``` ð Checking the compilability of post-
-processed code:: click to expand ::
+> [!Note] > > **Expected Schema of `[model_name]--wildcodebench-[task]--
+[backend]-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the
+keys of `get_wildcodebench()` > 2. `solution` (optional): Self-contained
+solution (usually including the prompt) > * Example: `{"task_id":
+"WildCodeBench/?", "solution": "def f():\n return 1"}` ### Code Post-processing
+LLM-generated text may not be compilable code for including natural language
+lines or incomplete extra code. We provide a tool namely `wildcode.sanitize` to
+clean up the code: ```shell # ð¡ If you are storing codes in jsonl:
+wildcode.sanitize --samples samples.jsonl # Sanitized code will be produced to
+`samples-sanitized.jsonl` # ð¡ If you are storing codes in directories:
+wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
+will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
+Checking the compilability of post-processed code:: click to expand ::
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
@@ -114,9 +113,11 @@
 generated Code We will share pre-generated code samples from LLMs we have
 [evaluated](https://wildcodebench.github.io/leaderboard.html): ## Known Issues
 - [ ] We notice that some tasks heavily use memory for scientific modeling
 during testing. It will lead to timeout issues on some machines. If you get an
 error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via
 pthread_create() failed.` in Tensorflow, it is very likely due to the memory
 issue. Try to allocate more memory to the process or reduce the number of
-parallel processes. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
+parallel processes. - [ ] Due to the flakes in the evaluation, the execution
+results may vary slightly (~0.5%) between runs. We are working on improving the
+evaluation stability. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
 [EvalPlus](https://github.com/evalplus/evalplus)
```

### Comparing `wild_code-0.4.5/release.sh` & `wild_code-0.5.0/release.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/run.sh` & `wild_code-0.5.0/run.sh`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 BS=5
 DATASET=wildcodebench
-MODEL=models/gemini-1.5-flash-latest
-BACKEND=google
+MODEL=gpt-3.5-turbo-0125
+BACKEND=openai
 TEMP=0
 N_SAMPLES=1
 NUM_GPU=1
+NL2CODE=True
 if [[ $MODEL == *"/"* ]]; then
   ORG=$(echo $MODEL | cut -d'/' -f1)--
   BASE_MODEL=$(echo $MODEL | cut -d'/' -f2)
 else
   ORG=""
   BASE_MODEL=$MODEL
 fi
-echo $ORG$BASE_MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES.jsonl
-python -m wildcode.generate \
-    --tp $NUM_GPU \
-    --model $MODEL \
-    --bs $BS \
-    --temperature $TEMP \
-    --n_samples $N_SAMPLES \
-    --resume \
-    --dataset $DATASET \
-    --backend $BACKEND 
 
-SAMPLE_FILE=$ORG$BASE_MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES.jsonl
-python -m wildcode.sanitize --samples $SAMPLE_FILE
-python -m wildcode.evaluate --dataset $DATASET --samples $ORG$BASE_MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized.jsonl
+if [ "$NL2CODE" = "True" ]; then
+  FILE_HEADER=$ORG$BASE_MODEL--$DATASET-NL2C--$BACKEND-$TEMP-$N_SAMPLES
+else
+  FILE_HEADER=$ORG$BASE_MODEL--$DATASET-C2C--$BACKEND-$TEMP-$N_SAMPLES
+fi
+
+echo $FILE_HEADER
+wildcode.generate \
+  --tp $NUM_GPU \
+  --model $MODEL \
+  --bs $BS \
+  --temperature $TEMP \
+  --n_samples $N_SAMPLES \
+  --resume \
+  --dataset $DATASET \
+  --nl2code $NL2CODE \
+  --id_range 0 10 \
+  --backend $BACKEND 
+
+wildcode.sanitize --samples $FILE_HEADER.jsonl
+wildcode.evaluate --dataset $DATASET --samples $FILE_HEADER-sanitized.jsonl
```

### Comparing `wild_code-0.4.5/setup.cfg` & `wild_code-0.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 	tqdm>=4.56.0
 	termcolor>=2.0.0
 	fire>=0.6.0
 	openai>=1.11.1
 	rich>=12.3.0
 	tree_sitter_languages>=1.10.2
 	tree-sitter==0.21.3
+	Pympler>=1.0.1
 	accelerate
 	vllm
 	anthropic
 	mistralai
 	stop-sequencer
-	Pympler>=1.0.1
+	google-generativeai
 
 [options.entry_points]
 console_scripts = 
 	wildcode.evaluate = wildcode.evaluate:main
 	wildcode.sanitize = wildcode.sanitize:main
 	wildcode.syncheck = wildcode.syncheck:main
 	wildcode.legacy_sanitize = wildcode.legacy_sanitize:main
```

### Comparing `wild_code-0.4.5/tests/test_legacy_sanitizer.py` & `wild_code-0.5.0/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/tests/test_treesitter_sanitizer.py` & `wild_code-0.5.0/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wild_code.egg-info/PKG-INFO` & `wild_code-0.5.0/wild_code.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.5
+Version: 0.5.0
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,32 +19,30 @@
 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0
 Requires-Dist: fire>=0.6.0
 Requires-Dist: openai>=1.11.1
 Requires-Dist: rich>=12.3.0
 Requires-Dist: tree_sitter_languages>=1.10.2
 Requires-Dist: tree-sitter==0.21.3
+Requires-Dist: Pympler>=1.0.1
 Requires-Dist: accelerate
 Requires-Dist: vllm
 Requires-Dist: anthropic
 Requires-Dist: mistralai
 Requires-Dist: stop-sequencer
-Requires-Dist: Pympler>=1.0.1
+Requires-Dist: google-generativeai
 
 # 🌳WildCodeBench
 
 > [!WARNING] 
 > The project is under active development. Please check back later for more updates.
 
 > [!WARNING]
 > Please use WildCode with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus), WildCode has a much less constrained execution environment to support tasks with diverse library dependencies. This may lead to security risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/) to run the evaluation.
 
-> [!WARNING]
-> WildCode framework currently only supports the Code2Code generation task. We are working on adding the NL2Code task.
-
 <p align="center">
     <a href="https://pypi.org/project/wild-code/"><img src="https://img.shields.io/pypi/v/wild-code?color=g"></a>
     <a href="https://hub.docker.com/r/terryzho/wildcode" title="Docker"><img src="https://img.shields.io/docker/image-size/terryzho/wildcode"></a>
     <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/wild-code"></a>
 </p>
 
 <p align="center">
@@ -122,17 +120,27 @@
 ```shell
 pip install -U flash-attn
 ```
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
+wildcode.generate \
+    --model [model_name] \
+    --dataset [wildcodebench] \
+    --nl2code [False|True] \
+    --greedy \
+    --bs [bs] \
+    --temperature [temp] \
+    --n_samples [n_samples] \
+    --resume \
+    --backend [vllm|hf|openai|mistral|anthropic|google]
+    --tp [gpu_number]
 ```
-The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
+The generated code samples will be stored in a file named `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
@@ -141,15 +149,15 @@
 + `test` is the `unittest` test case
 
 </div>
 </details>
 
 > [!Note]
 >
-> **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
+> **Expected Schema of `[model_name]--wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`**
 >
 > 1. `task_id`: Task ID, which are the keys of `get_wildcodebench()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
 >    * Example: `{"task_id": "WildCodeBench/?", "solution": "def f():\n    return 1"}`
 
 ### Code Post-processing
 
@@ -275,14 +283,16 @@
 
 We will share pre-generated code samples from LLMs we have [evaluated](https://wildcodebench.github.io/leaderboard.html):
 
 ## Known Issues
 
 - [ ] We notice that some tasks heavily use memory for scientific modeling during testing. It will lead to timeout issues on some machines. If you get an error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via pthread_create() failed.` in Tensorflow, it is very likely due to the memory issue. Try to allocate more memory to the process or reduce the number of parallel processes.
 
+- [ ] Due to the flakes in the evaluation, the execution results may vary slightly (~0.5%) between runs. We are working on improving the evaluation stability.
+
 ## 📜 Citation
 
 ```bibtex
 ```
 
 ## 🙏 Acknowledgement
```

#### html2text {}

```diff
@@ -1,30 +1,28 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.5 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.5.0 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
 appdirs>=1.4.4 Requires-Dist: numpy>=1.19.5 Requires-Dist: tqdm>=4.56.0
 Requires-Dist: termcolor>=2.0.0 Requires-Dist: fire>=0.6.0 Requires-Dist:
 openai>=1.11.1 Requires-Dist: rich>=12.3.0 Requires-Dist:
 tree_sitter_languages>=1.10.2 Requires-Dist: tree-sitter==0.21.3 Requires-Dist:
-accelerate Requires-Dist: vllm Requires-Dist: anthropic Requires-Dist:
-mistralai Requires-Dist: stop-sequencer Requires-Dist: Pympler>=1.0.1 #
-ð³WildCodeBench > [!WARNING] > The project is under active development.
-Please check back later for more updates. > [!WARNING] > Please use WildCode
-with caution. Different from [EvalPlus](https://github.com/evalplus/evalplus),
-WildCode has a much less constrained execution environment to support tasks
-with diverse library dependencies. This may lead to security risks. We
-recommend using a sandbox such as [Docker](https://docs.docker.com/get-docker/
-) to run the evaluation. > [!WARNING] > WildCode framework currently only
-supports the Code2Code generation task. We are working on adding the NL2Code
-task.
+Pympler>=1.0.1 Requires-Dist: accelerate Requires-Dist: vllm Requires-Dist:
+anthropic Requires-Dist: mistralai Requires-Dist: stop-sequencer Requires-Dist:
+google-generativeai # ð³WildCodeBench > [!WARNING] > The project is under
+active development. Please check back later for more updates. > [!WARNING] >
+Please use WildCode with caution. Different from [EvalPlus](https://github.com/
+evalplus/evalplus), WildCode has a much less constrained execution environment
+to support tasks with diverse library dependencies. This may lead to security
+risks. We recommend using a sandbox such as [Docker](https://docs.docker.com/
+get-docker/) to run the evaluation.
    _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_w_i_l_d_-_c_o_d_e_?_c_o_l_o_r_=_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_t_e_r_r_y_z_h_o_/_w_i_l_d_c_o_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_l_/_w_i_l_d_-_c_o_d_e_]
  _ð___³_A_b_o_u_t â¢ _ð___¥_Q_u_i_c_k_ _S_t_a_r_t â¢ _ð___»_L_L_M_ _c_o_d_e â¢ _ð____F_a_i_l_u_r_e_ _i_n_s_p_e_c_t_i_o_n â¢
            _ð____K_n_o_w_n_ _i_s_s_u_e_s â¢ _ð____C_i_t_a_t_i_o_n â¢ _ð____A_c_k_n_o_w_l_e_d_g_e_m_e_n_t
 ## About ### WildCodeBench WildCodeBench is a rigorous benchmark for code
 generation with realistic constraints in the wild. It aims to evaluate the true
 programming capabilities of large language models (LLMs) in a more realistic
@@ -56,37 +54,38 @@
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
 ### Code Generation You are suggested to use `flash-attn` for generating code
 samples. ```shell pip install -U flash-attn ``` To generate code samples from a
-model, you can use the following command: ```shell wildcode.generate --model
-[model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp]
---n_samples [n_samples] --resume --backend [vllm|hf|openai] --tp [gpu_number]
-``` The generated code samples will be stored in a file named `[model_name]--
-wildcodebench--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
+model, you can use the following command: ```shell wildcode.generate \ --model
+[model_name] \ --dataset [wildcodebench] \ --nl2code [False|True] \ --greedy \
+--bs [bs] \ --temperature [temp] \ --n_samples [n_samples] \ --resume \ --
+backend [vllm|hf|openai|mistral|anthropic|google] --tp [gpu_number] ``` The
+generated code samples will be stored in a file named `[model_name]--
+wildcodebench-[task]--[backend]-[temp]-[n_samples].jsonl`. ð¤ Structure of
 `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
 is the ground-truth implementation + `test` is the `unittest` test case
-> [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
-`get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
-(usually including the prompt) > * Example: `{"task_id": "WildCodeBench/?",
-"solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated text
-may not be compilable code for including natural language lines or incomplete
-extra code. We provide a tool namely `wildcode.sanitize` to clean up the code:
-```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize --samples
-samples.jsonl # Sanitized code will be produced to `samples-sanitized.jsonl` #
-ð¡ If you are storing codes in directories: wildcode.sanitize --samples /
-path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/
-vicuna-[??]b_temp_[??]-sanitized` ``` ð Checking the compilability of post-
-processed code:: click to expand ::
+> [!Note] > > **Expected Schema of `[model_name]--wildcodebench-[task]--
+[backend]-[temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the
+keys of `get_wildcodebench()` > 2. `solution` (optional): Self-contained
+solution (usually including the prompt) > * Example: `{"task_id":
+"WildCodeBench/?", "solution": "def f():\n return 1"}` ### Code Post-processing
+LLM-generated text may not be compilable code for including natural language
+lines or incomplete extra code. We provide a tool namely `wildcode.sanitize` to
+clean up the code: ```shell # ð¡ If you are storing codes in jsonl:
+wildcode.sanitize --samples samples.jsonl # Sanitized code will be produced to
+`samples-sanitized.jsonl` # ð¡ If you are storing codes in directories:
+wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
+will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
+Checking the compilability of post-processed code:: click to expand ::
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
@@ -128,9 +127,11 @@
 generated Code We will share pre-generated code samples from LLMs we have
 [evaluated](https://wildcodebench.github.io/leaderboard.html): ## Known Issues
 - [ ] We notice that some tasks heavily use memory for scientific modeling
 during testing. It will lead to timeout issues on some machines. If you get an
 error message like `Check failed: ret == 0 (11 vs. 0)Thread creation via
 pthread_create() failed.` in Tensorflow, it is very likely due to the memory
 issue. Try to allocate more memory to the process or reduce the number of
-parallel processes. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
+parallel processes. - [ ] Due to the flakes in the evaluation, the execution
+results may vary slightly (~0.5%) between runs. We are working on improving the
+evaluation stability. ## ð Citation ```bibtex ``` ## ð Acknowledgement -
 [EvalPlus](https://github.com/evalplus/evalplus)
```

### Comparing `wild_code-0.4.5/wild_code.egg-info/SOURCES.txt` & `wild_code-0.5.0/wild_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/data/utils.py` & `wild_code-0.5.0/wildcode/data/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,45 +8,45 @@
 import wget
 from appdirs import user_cache_dir
 
 CACHE_DIR = user_cache_dir("wildcodebench")
 
 
 def get_dataset_metadata(name: str, version: str, mini: bool, noextreme: bool = False):
-    assert name in ["WildCodeBenchPlus"], f"Unknown/unsupported dataset: {name}"
+    assert name in ["WildCodeBench"], f"Unknown/unsupported dataset: {name}"
     extra = ""
     assert not (mini and noextreme), "Cannot have both mini and noextreme"
     if mini:
         extra = "-Mini"
     if noextreme:
         extra = "-NoExtreme"
-    url = f"https://github.com/wildcode/{name.lower()}_release/releases/download/{version}/{name}{extra}.jsonl.gz"
+    url = f"https://github.com/bigcode-project/wildcodebench-annotation/releases/download/{version}/{name}{extra}.jsonl.gz"
     cache_path = os.path.join(CACHE_DIR, f"{name}{extra}-{version}.jsonl")
     return url, cache_path
 
 
 def make_cache(gzip_url, cache_path):
     # Check if open eval file exists in CACHE_DIR
     if not os.path.exists(cache_path):
         # Install WildCodeBench dataset and parse as jsonl
         print(f"Downloading dataset from {gzip_url}")
         with tempdir.TempDir() as tmpdir:
-            plus_gz_path = os.path.join(tmpdir, f"data.jsonl.gz")
-            wget.download(gzip_url, plus_gz_path)
+            gz_path = os.path.join(tmpdir, f"data.jsonl.gz")
+            wget.download(gzip_url, gz_path)
 
-            with gzip.open(plus_gz_path, "rb") as f:
-                plus = f.read().decode("utf-8")
+            with gzip.open(gz_path, "rb") as f:
+                data = f.read().decode("utf-8")
 
         # create CACHE_DIR if not exists
         if not os.path.exists(CACHE_DIR):
             os.makedirs(CACHE_DIR)
 
         # Write the original open eval file to CACHE_DIR
         with open(cache_path, "w") as f:
-            f.write(plus)
+            f.write(data)
 
 
 def write_jsonl(
     filename: str, data: Iterable[Dict], append: bool = False, drop_builtin: bool = True
 ):
     """
     Writes an iterable of dictionaries to jsonl
@@ -145,21 +145,20 @@
             counters[task_id] = 0
         sample_id = counters[task_id]
         with open(os.path.join(task_dir, f"{sample_id}.py"), "w") as f:
             f.write(sample["solution"])
         counters[task_id] += 1
 
 
-def completeness_check(name, plus):
-    for task_id, task in plus.items():
+def completeness_check(name, data):
+    for task_id, task in data.items():
         for key in [
             "prompt",
-            "contract",
             "canonical_solution",
             "test",
-            "atol",
+            "instruction"
         ]:
             assert key in task, f"{key} not found in {name} #{task_id}!"
 
 
 def to_raw(string):
     return string.encode("unicode-escape").decode().replace("\\\\", "\\")
```

### Comparing `wild_code-0.4.5/wildcode/eval/__init__.py` & `wild_code-0.5.0/wildcode/eval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     _poly,
 )
 from wildcode.eval.utils import (
     create_tempdir,
     reliability_guard,
     swallow_io,
     time_limit,
+    safe_environment,
 )
 
 
 def compatible_eval_result(results: Dict) -> Dict:
     # compatibility
     for task_results in results["eval"].values():
         # update the "files" field to "nfiles"
@@ -109,15 +110,15 @@
     entry_point: str,
     code: str,
     test_code: str,
     timeout: float,
     stat,  # Value
     details,  # Array
 ):
-    with create_tempdir():
+    with safe_environment(), create_tempdir():
         # These system calls are needed when cleaning up tempdir.
         import os
         import shutil
         import builtins
         
         rmtree = shutil.rmtree
         rmdir = os.rmdir
```

### Comparing `wild_code-0.4.5/wildcode/evaluate.py` & `wild_code-0.5.0/wildcode/evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,18 +94,24 @@
         n_workers = flags.parallel
 
     if flags.check_gt_only:
         # bypass the samples
         flags.samples = "__dummy__.jsonl"
         
     if os.path.isdir(flags.samples):
-        result_path = os.path.join(flags.samples, "eval_results.json")
+        if flags.reprompt:
+            result_path = os.path.join(flags.samples, "reprompt_eval_results.json")
+        else:
+            result_path = os.path.join(flags.samples, "eval_results.json")
     else:
         assert flags.samples.endswith(".jsonl")
-        result_path = flags.samples.replace(".jsonl", "_eval_results.json")
+        if flags.reprompt:
+            result_path = flags.samples.replace(".jsonl", "_reprompt_eval_results.json")
+        else:
+            result_path = flags.samples.replace(".jsonl", "_eval_results.json")
 
     if os.path.isfile(result_path):
         print(f"Load from previous results from {result_path}")
         with open(result_path, "r") as f:
             results = json.load(f)
 
         results = compatible_eval_result(results)
@@ -140,14 +146,16 @@
                     )
                     continue
                 solution = (
                     sample["solution"]
                     if "solution" in sample
                     else problems[task_id]["prompt"] + sample["completion"]
                 )
+                if flags.reprompt:
+                    solution = problems[task_id]["prompt_wo_doc"] + "\n    pass\n" + solution
                 remainings.add(sample["_identifier"])
                 args = (
                     flags.dataset,
                     completion_id[task_id],
                     problems[task_id],
                     solution,
                     sample["_identifier"],
@@ -237,14 +245,17 @@
     parser.add_argument(
         "--dataset", required=True, type=str, choices=["wildcodebench"]
     )
     parser.add_argument("--samples", required=True, type=str)
     parser.add_argument("--parallel", default=None, type=int)
     parser.add_argument("--min-time-limit", default=1, type=float)
     parser.add_argument(
+        "--reprompt", action="store_true", help="Prepend the prompt again"
+    )
+    parser.add_argument(
         "--check-gt-only", action="store_true", help="Check the groundtruth"
     )
     args = parser.parse_args()
 
     evaluate(args)
```

### Comparing `wild_code-0.4.5/wildcode/gen/__init__.py` & `wild_code-0.5.0/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/gen/util/__init__.py` & `wild_code-0.5.0/wildcode/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/gen/util/anthropic_request.py` & `wild_code-0.5.0/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/gen/util/openai_request.py` & `wild_code-0.5.0/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/generate.py` & `wild_code-0.5.0/wildcode/generate.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 )
 
 
 def codegen(
     model: DecoderBase,
     save_path: str,
     dataset: str,
+    nl2code=False,
     greedy=False,
+    strip_newlines=False,
     n_samples=1,
     id_range=None,
     resume=True,
 ):
     with Progress(
         TextColumn(f"{dataset} •" + "[progress.percentage]{task.percentage:>3.0f}%"),
         BarColumn(),
@@ -31,14 +33,17 @@
         TimeElapsedColumn(),
     ) as p:
         if dataset == "wildcodebench":
             from wildcode.data import get_wildcodebench, write_jsonl
 
             dataset = get_wildcodebench()
 
+        if model.is_direct_completion() and nl2code:
+            raise Exception("Base model does not support direct completion for NL2Code tasks")
+            
         # create save_path if it doesn't exist, e.g., a/b.jsonl
         dirname = os.path.dirname(save_path)
         if not os.path.exists(dirname) and dirname != "":
             os.makedirs(dirname)
         for task_id, task in p.track(dataset.items()):
             if id_range is not None:
                 id_num = int(task_id.split("/")[1])
@@ -64,25 +69,30 @@
                     log += f" (resuming from {n_existing})"
 
             nsamples = n_samples - n_existing
             p.console.print(log)
 
             sidx = n_samples - nsamples
             while sidx < n_samples:
+                prompt = task["prompt"]
+                if nl2code:
+                    prompt = task["instruction"]
+                if strip_newlines:
+                    prompt = prompt.strip("\n")
                 outputs = model.codegen(
-                    task["prompt"],
+                    prompt,
                     do_sample=not greedy,
                     num_samples=n_samples - sidx,
                 )
                 assert outputs, "No outputs from model!"
                 if model.is_direct_completion():
                     samples = [
                         dict(
                             task_id=task_id,
-                            solution=task["prompt"]+completion,
+                            solution=task["prompt"]+completion
                         )
                         for task_id, completion in zip([task_id]*len(outputs), outputs)
                     ]
                 else:
                     samples = [
                         dict(
                             task_id=task_id,
@@ -95,18 +105,20 @@
                 sidx += len(outputs)
                 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--model", required=True, type=str)
     parser.add_argument("--dataset", required=True, type=str)
+    parser.add_argument("--nl2code", default=False, type=bool)
     parser.add_argument("--bs", default=1, type=int)
     parser.add_argument("--n_samples", default=1, type=int)
     parser.add_argument("--temperature", default=0.0, type=float)
     parser.add_argument("--greedy", action="store_true")
+    parser.add_argument("--strip_newlines", action="store_true")
     parser.add_argument("--resume", action="store_true")
     parser.add_argument("--id_range", nargs=2, type=int)
     parser.add_argument("--backend", default="vllm", type=str)
     parser.add_argument("--base_url", default=None, type=str)
     parser.add_argument("--tp", default=1, type=int)
     args = parser.parse_args()
     
@@ -136,18 +148,20 @@
         dataset=args.dataset,
         base_url=args.base_url,
         tp=args.tp,
     )
     save_path = args.model.replace("/", "--") + f"--{args.dataset}--" +f"{args.backend}-{args.temperature}-{args.n_samples}.jsonl"
     
     codegen(
-        dataset=args.dataset,
-        greedy=args.greedy,
         model=model_runner,
         save_path=save_path,
+        dataset=args.dataset,
+        nl2code=args.nl2code,
+        greedy=args.greedy,
+        strip_newlines=args.strip_newlines,
         n_samples=args.n_samples,
         resume=args.resume,
         id_range=args.id_range,
     )
 
 
 if __name__ == "__main__":
```

### Comparing `wild_code-0.4.5/wildcode/inspect.py` & `wild_code-0.5.0/wildcode/inspect.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/lecacy_sanitize.py` & `wild_code-0.5.0/wildcode/lecacy_sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.5/wildcode/model.py` & `wild_code-0.5.0/wildcode/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -427,26 +427,48 @@
         if not do_sample:
             assert batch_size == 1, "Sampling only supports batch size of 1"
 
         genai_config = genai.GenerationConfig(
             max_output_tokens=self.max_new_tokens,
             **kwargs,
         )
-    
-        model = genai.GenerativeModel(model_name=self.name, generation_config=genai_config)
 
+        safety_settings = [
+            {
+                "category": "HARM_CATEGORY_DANGEROUS",
+                "threshold": "BLOCK_NONE",
+            },
+            {
+                "category": "HARM_CATEGORY_HARASSMENT",
+                "threshold": "BLOCK_NONE",
+            },
+            {
+                "category": "HARM_CATEGORY_HATE_SPEECH",
+                "threshold": "BLOCK_NONE",
+            },
+            {
+                "category": "HARM_CATEGORY_SEXUALLY_EXPLICIT",
+                "threshold": "BLOCK_NONE",
+            },
+            {
+                "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
+                "threshold": "BLOCK_NONE",
+            },
+        ]
+        
+        model = genai.GenerativeModel(model_name=self.name, generation_config=genai_config, safety_settings=safety_settings)
         
         outputs = []
         for _ in range(batch_size):
-            message = model.generate_content(
+            response = model.generate_content(
                 "Please generate self-contained code to complete the following problem wrapped in a Python markdown block:"
                 + f"\n```python\n{prompt.strip()}\n```",
                 generation_config=genai_config
             )
-            outputs.append(message.text)
+            outputs.append(response.candidates[0].content.parts[0].text)
 
         return outputs
 
 
 def make_model(
     model: str,
     backend: str,
```

### Comparing `wild_code-0.4.5/wildcode/sanitize.py` & `wild_code-0.5.0/wildcode/sanitize.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,32 +176,38 @@
             outer_lines.append(i)
     if outer_lines:
         sanitized_output = "\n".join(lines[: outer_lines[-1]])
     return sanitized_output
 
 
 def script(
-    samples: str, inplace: bool = False, debug_task: str = None
+    samples: str, inplace: bool = False, debug_task: str = None, reprompt: bool = False
 ):
     # task_id -> entry_point
     entry_point = {}
     # merge two datasets
     dataset = {**get_wildcodebench()}
 
     for task_id, problem in dataset.items():
         entry_point[task_id] = problem["entry_point"]
 
     # make a new folder with "-sanitized" suffix
     is_folder = os.path.isdir(samples)
     target_path = pathlib.Path(samples)
     if not inplace:
         if is_folder:
-            new_name = target_path.name + "-sanitized"
+            if reprompt:
+                new_name = target_path.name + "-sanitized-reprompt"
+            else:
+                new_name = target_path.name + "-sanitized"
         else:
-            new_name = target_path.name.replace(".jsonl", "-sanitized.jsonl")
+            if reprompt:
+                new_name = target_path.name.replace(".jsonl", "-sanitized-reprompt.jsonl")
+            else:
+                new_name = target_path.name.replace(".jsonl", "-sanitized.jsonl")
         target_path = target_path.parent / new_name
     target_path = str(target_path)
 
     nsan = 0
     ntotal = 0
 
     new_solutions = []
@@ -218,14 +224,16 @@
         dbg_identifier = solution["_identifier"]
         if debug_task is not None and task_id != debug_task:
             continue
 
         ntotal += 1
         if "solution" in solution:
             old_code = solution["solution"]
+            if reprompt:
+                old_code = solution["solution"].replace("```python\n    ", "```python\n"+dataset[task_id]["prompt"]+"    ")
         else:
             assert "completion" in solution
             old_code = dataset[task_id]["prompt"] + "\n" + solution["completion"]
 
         new_code = sanitize(code=old_code, entrypoint=function_name)
         # if changed, print the message
         if new_code != old_code:
```

### Comparing `wild_code-0.4.5/wildcode/syncheck.py` & `wild_code-0.5.0/wildcode/syncheck.py`

 * *Files identical despite different names*


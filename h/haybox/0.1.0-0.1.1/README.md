# Comparing `tmp/haybox-0.1.0.tar.gz` & `tmp/haybox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haybox-0.1.0.tar", max compression
+gzip compressed data, was "haybox-0.1.1.tar", max compression
```

## Comparing `haybox-0.1.0.tar` & `haybox-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,39 @@
--rw-r--r--   0        0        0       67 2024-05-18 14:57:44.977694 haybox-0.1.0/README.md
--rw-r--r--   0        0        0      497 2024-05-18 14:57:44.977694 haybox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      106 2024-05-18 14:57:44.977694 haybox-0.1.0/src/haybox/__init__.py
--rw-r--r--   0        0        0     5952 2024-05-18 14:57:44.977694 haybox-0.1.0/src/haybox/haybox.py
--rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 haybox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2024-05-18 15:27:51.760790 haybox-0.1.1/README.md
+-rw-r--r--   0        0        0      507 2024-05-18 15:27:51.760790 haybox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-05-18 15:27:51.760790 haybox-0.1.1/src/haybox/__init__.py
+-rw-r--r--   0        0        0     5952 2024-05-18 15:27:51.760790 haybox-0.1.1/src/haybox/haybox.py
+-rw-r--r--   0        0        0      105 2024-05-18 15:27:52.500801 haybox-0.1.1/src/haybox/proto/.git/FETCH_HEAD
+-rw-r--r--   0        0        0       41 2024-05-18 15:27:52.568802 haybox-0.1.1/src/haybox/proto/.git/HEAD
+-rw-r--r--   0        0        0      423 2024-05-18 15:27:52.512802 haybox-0.1.1/src/haybox/proto/.git/config
+-rw-r--r--   0        0        0       83 2024-05-18 15:27:52.504802 haybox-0.1.1/src/haybox/proto/.git/config.worktree
+-rwxr-xr-x   0        0        0       73 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/description
+-rwxr-xr-x   0        0        0      478 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4726 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1649 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2024-05-18 15:27:51.912793 haybox-0.1.1/src/haybox/proto/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     2308 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0        0        0     3650 2024-05-18 15:27:51.908793 haybox-0.1.1/src/haybox/proto/.git/hooks/update.sample
+-rw-r--r--   0        0        0      305 2024-05-18 15:27:52.568802 haybox-0.1.1/src/haybox/proto/.git/index
+-rwxr-xr-x   0        0        0      240 2024-05-18 15:27:51.912793 haybox-0.1.1/src/haybox/proto/.git/info/exclude
+-rw-r--r--   0        0        0      347 2024-05-18 15:27:52.568802 haybox-0.1.1/src/haybox/proto/.git/logs/HEAD
+-rw-r--r--   0        0        0      182 2024-05-18 15:27:52.512802 haybox-0.1.1/src/haybox/proto/.git/logs/refs/heads/main
+-rw-r--r--   0        0        0      256 2024-05-18 15:27:52.500801 haybox-0.1.1/src/haybox/proto/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0        0        0     5216 2024-05-18 15:27:52.492801 haybox-0.1.1/src/haybox/proto/.git/objects/pack/pack-443230d58a801023f2973578cca4e9ccd56d7770.idx
+-rw-r--r--   0        0        0    35951 2024-05-18 15:27:52.492801 haybox-0.1.1/src/haybox/proto/.git/objects/pack/pack-443230d58a801023f2973578cca4e9ccd56d7770.pack
+-rw-r--r--   0        0        0      644 2024-05-18 15:27:52.496801 haybox-0.1.1/src/haybox/proto/.git/objects/pack/pack-443230d58a801023f2973578cca4e9ccd56d7770.rev
+-rw-r--r--   0        0        0       41 2024-05-18 15:27:52.512802 haybox-0.1.1/src/haybox/proto/.git/refs/heads/main
+-rw-r--r--   0        0        0       41 2024-05-18 15:27:52.500801 haybox-0.1.1/src/haybox/proto/.git/refs/remotes/origin/main
+-rw-r--r--   0        0        0     2489 2024-05-18 15:27:52.512802 haybox-0.1.1/src/haybox/proto/config.options
+-rw-r--r--   0        0        0     5122 2024-05-18 15:27:52.512802 haybox-0.1.1/src/haybox/proto/config.proto
+-rw-r--r--   0        0        0    11648 2024-05-18 15:27:57.012854 haybox-0.1.1/src/haybox/proto/config_pb2.py
+-rw-r--r--   0        0        0    19676 2024-05-18 15:27:57.012854 haybox-0.1.1/src/haybox/proto/config_pb2.pyi
+-rw-r--r--   0        0        0      667 2024-05-18 15:27:52.512802 haybox-0.1.1/src/haybox/proto/library.json
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 haybox-0.1.1/PKG-INFO
```

### Comparing `haybox-0.1.0/src/haybox/haybox.py` & `haybox-0.1.1/src/haybox/haybox.py`

 * *Files identical despite different names*

### Comparing `haybox-0.1.0/PKG-INFO` & `haybox-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haybox
-Version: 0.1.0
+Version: 0.1.1
 Summary: HayBox firmware config protocol Python library
 License: GPL-3.0-only
 Author: Jonathan Haylett
 Author-email: jonathan@haylett.dev
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


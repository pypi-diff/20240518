# Comparing `tmp/heliumcli-1.6.8.tar.gz` & `tmp/heliumcli-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heliumcli-1.6.8.tar", last modified: Wed Nov 22 17:03:22 2023, max compression
+gzip compressed data, was "heliumcli-1.6.9.tar", last modified: Wed Nov 22 17:35:12 2023, max compression
```

## Comparing `heliumcli-1.6.8.tar` & `heliumcli-1.6.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.367303 heliumcli-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-22 17:02:10.000000 heliumcli-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-22 17:02:10.000000 heliumcli-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-22 17:03:22.367303 heliumcli-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-11-22 17:02:10.000000 heliumcli-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.355302 heliumcli-1.6.8/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.363303 heliumcli-1.6.8/_build/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)    22728 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/coverage.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21865 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/coverage_html.js
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_8289d082374b3103___init___py.html
--rw-r--r--   0 runner    (1001) docker     (127)    20396 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/d_8289d082374b3103_main_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/d_8289d082374b3103_settings_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    41475 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/d_8289d082374b3103_utils_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b___init___py.html
--rw-r--r--   0 runner    (1001) docker     (127)    46352 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_buildrelease_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    31731 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_deploybuild_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    41631 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_init_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    17700 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_listbuilds_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    53621 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_prepcode_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    20051 2023-11-22 17:03:21.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_setbuild_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    15574 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_startservers_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_update_py.html
--rw-r--r--   0 runner    (1001) docker     (127)    22984 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_updateprojects_py.html
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/favicon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/keybd_closed.png
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/keybd_open.png
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/status.json
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2023-11-22 17:03:22.000000 heliumcli-1.6.8/_build/coverage/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.363303 heliumcli-1.6.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      246 2023-11-22 17:02:10.000000 heliumcli-1.6.8/bin/helium-cli
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.363303 heliumcli-1.6.8/heliumcli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.363303 heliumcli-1.6.8/heliumcli/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/buildrelease.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/deploybuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/listbuilds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/prepcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/setbuild.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/startservers.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/actions/updateprojects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1562 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2023-11-22 17:02:10.000000 heliumcli-1.6.8/heliumcli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.367303 heliumcli-1.6.8/heliumcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-22 17:03:22.000000 heliumcli-1.6.8/heliumcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-11-22 17:03:22.000000 heliumcli-1.6.8/heliumcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 17:03:22.000000 heliumcli-1.6.8/heliumcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-22 17:03:22.000000 heliumcli-1.6.8/heliumcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-22 17:03:22.000000 heliumcli-1.6.8/heliumcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-22 17:03:22.367303 heliumcli-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-11-22 17:02:10.000000 heliumcli-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:03:22.367303 heliumcli-1.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2023-11-22 17:02:10.000000 heliumcli-1.6.8/tests/testactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-11-22 17:02:10.000000 heliumcli-1.6.8/tests/testconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-11-22 17:02:10.000000 heliumcli-1.6.8/tests/testinit.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-22 17:02:10.000000 heliumcli-1.6.8/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.734917 heliumcli-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-11-22 17:34:02.000000 heliumcli-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-22 17:34:02.000000 heliumcli-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-22 17:35:12.734917 heliumcli-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-11-22 17:34:02.000000 heliumcli-1.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.722917 heliumcli-1.6.9/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.730918 heliumcli-1.6.9/_build/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    22762 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/coverage.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21865 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/coverage_html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_8289d082374b3103___init___py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20396 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_8289d082374b3103_main_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_8289d082374b3103_settings_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    41475 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_8289d082374b3103_utils_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b___init___py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    46352 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_buildrelease_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    31731 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_deploybuild_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    41631 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_init_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17700 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_listbuilds_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    53621 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_prepcode_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20051 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_setbuild_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_startservers_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_update_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23543 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_updateprojects_py.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/favicon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/keybd_closed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/keybd_open.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/status.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2023-11-22 17:35:12.000000 heliumcli-1.6.9/_build/coverage/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.730918 heliumcli-1.6.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      246 2023-11-22 17:34:02.000000 heliumcli-1.6.9/bin/helium-cli
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.730918 heliumcli-1.6.9/heliumcli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.730918 heliumcli-1.6.9/heliumcli/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/buildrelease.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/deploybuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/listbuilds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/prepcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/setbuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/startservers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/actions/updateprojects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1562 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2023-11-22 17:34:02.000000 heliumcli-1.6.9/heliumcli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.734917 heliumcli-1.6.9/heliumcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-22 17:35:12.000000 heliumcli-1.6.9/heliumcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-11-22 17:35:12.000000 heliumcli-1.6.9/heliumcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 17:35:12.000000 heliumcli-1.6.9/heliumcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-22 17:35:12.000000 heliumcli-1.6.9/heliumcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-22 17:35:12.000000 heliumcli-1.6.9/heliumcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-22 17:35:12.734917 heliumcli-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-11-22 17:34:02.000000 heliumcli-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 17:35:12.734917 heliumcli-1.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2023-11-22 17:34:02.000000 heliumcli-1.6.9/tests/testactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-11-22 17:34:02.000000 heliumcli-1.6.9/tests/testconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-11-22 17:34:02.000000 heliumcli-1.6.9/tests/testinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-22 17:34:02.000000 heliumcli-1.6.9/tests/testutils.py
```

### Comparing `heliumcli-1.6.8/LICENSE` & `heliumcli-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/PKG-INFO` & `heliumcli-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: heliumcli
-Version: 1.6.8
+Version: 1.6.9
 Summary: CLI tool that provides a useful set of tools for maintaining, building, and deploying code in compatible projects
 Home-page: https://github.com/HeliumEdu/heliumcli
-Download-URL: https://github.com/HeliumEdu/heliumcli/archive/1.6.8.tar.gz
+Download-URL: https://github.com/HeliumEdu/heliumcli/archive/1.6.9.tar.gz
 Author: Alex Laird
 Author-email: contact@alexlaird.com
 License: MIT
 Project-URL: Sponsor, https://github.com/sponsors/alexdlaird
 Keywords: cli,build,deployment,ansible,git
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `heliumcli-1.6.8/README.md` & `heliumcli-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/_build/coverage/coverage.xml` & `heliumcli-1.6.9/_build/coverage/coverage.xml`

 * *Files 0% similar despite different names*

#### Comparing `heliumcli-1.6.8/_build/coverage/coverage.xml` & `heliumcli-1.6.9/_build/coverage/coverage.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.3.2" timestamp="1700672601801" lines-valid="559" lines-covered="510" line-rate="0.9123" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
+<coverage version="7.3.2" timestamp="1700674512163" lines-valid="560" lines-covered="511" line-rate="0.9125" branches-covered="0" branches-valid="0" branch-rate="0" complexity="0">
   <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.3.2 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/runner/work/heliumcli/heliumcli</source>
   </sources>
   <packages>
     <package name="heliumcli" line-rate="0.9681" branch-rate="0" complexity="0">
@@ -119,15 +119,15 @@
             <line number="125" hits="1"/>
             <line number="127" hits="1"/>
             <line number="129" hits="1"/>
           </lines>
         </class>
       </classes>
     </package>
-    <package name="heliumcli.actions" line-rate="0.9011" branch-rate="0" complexity="0">
+    <package name="heliumcli.actions" line-rate="0.9013" branch-rate="0" complexity="0">
       <classes>
         <class name="__init__.py" filename="heliumcli/actions/__init__.py" complexity="0" line-rate="1" branch-rate="0">
           <methods/>
           <lines/>
         </class>
         <class name="buildrelease.py" filename="heliumcli/actions/buildrelease.py" complexity="0" line-rate="0.8506" branch-rate="0">
           <methods/>
@@ -591,15 +591,15 @@
             <line number="13" hits="1"/>
             <line number="14" hits="1"/>
             <line number="15" hits="1"/>
             <line number="17" hits="1"/>
             <line number="18" hits="1"/>
           </lines>
         </class>
-        <class name="updateprojects.py" filename="heliumcli/actions/updateprojects.py" complexity="0" line-rate="0.9744" branch-rate="0">
+        <class name="updateprojects.py" filename="heliumcli/actions/updateprojects.py" complexity="0" line-rate="0.975" branch-rate="0">
           <methods/>
           <lines>
             <line number="1" hits="1"/>
             <line number="2" hits="1"/>
             <line number="4" hits="1"/>
             <line number="6" hits="1"/>
             <line number="8" hits="1"/>
@@ -618,28 +618,29 @@
             <line number="26" hits="1"/>
             <line number="27" hits="1"/>
             <line number="28" hits="1"/>
             <line number="29" hits="1"/>
             <line number="31" hits="1"/>
             <line number="32" hits="1"/>
             <line number="33" hits="1"/>
-            <line number="35" hits="1"/>
+            <line number="34" hits="1"/>
             <line number="36" hits="1"/>
-            <line number="38" hits="1"/>
+            <line number="37" hits="1"/>
             <line number="39" hits="1"/>
-            <line number="41" hits="1"/>
+            <line number="40" hits="1"/>
             <line number="42" hits="1"/>
-            <line number="44" hits="0"/>
-            <line number="46" hits="1"/>
+            <line number="43" hits="1"/>
+            <line number="45" hits="0"/>
             <line number="47" hits="1"/>
             <line number="48" hits="1"/>
-            <line number="50" hits="1"/>
+            <line number="49" hits="1"/>
             <line number="51" hits="1"/>
             <line number="52" hits="1"/>
-            <line number="54" hits="1"/>
-            <line number="56" hits="1"/>
+            <line number="53" hits="1"/>
+            <line number="55" hits="1"/>
+            <line number="57" hits="1"/>
           </lines>
         </class>
       </classes>
     </package>
   </packages>
 </coverage>
```

### Comparing `heliumcli-1.6.8/_build/coverage/coverage_html.js` & `heliumcli-1.6.9/_build/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/_build/coverage/d_8289d082374b3103___init___py.html` & `heliumcli-1.6.9/_build/coverage/d_8289d082374b3103___init___py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_8289d082374b3103_main_py.html` & `heliumcli-1.6.9/_build/coverage/d_8289d082374b3103_main_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_updateprojects_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8289d082374b3103_settings_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -148,13 +148,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_updateprojects_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8289d082374b3103_settings_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2277 ssttaatteemmeennttss ?  2277 rruunn 00 mmiissssiinngg 88 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1#!/usr/bin/env python 
 _2 
 _3import argparse 
 _4import sys 
 _5 
 _6from heliumcli.actions.listbuilds import ListBuildsAction 
 _7from . import utils 
@@ -72,8 +72,8 @@
 _5_8 
 _5_9 print("") 
 _6_0 
 _6_1 
 _6_2if __name__ == "__main__": 
 _6_3 main(sys.argv) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_8289d082374b3103_settings_py.html` & `heliumcli-1.6.9/_build/coverage/d_8289d082374b3103_settings_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8289d082374b3103_main_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8289d082374b3103_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -81,15 +81,15 @@
 </header>
 <main id="source">
     <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">json</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">os</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="nam">__author__</span> <span class="op">=</span> <span class="str">"Alex Laird"</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="nam">__copyright__</span> <span class="op">=</span> <span class="str">"Copyright 2023, Helium Edu"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.6.8"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.6.9"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">VERSION</span> <span class="op">=</span> <span class="nam">__version__</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">def</span> <span class="nam">get_default_settings</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="str">"gitProject"</span><span class="op">:</span> <span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"HELIUMCLI_GIT_PROJECT"</span><span class="op">,</span> <span class="str">"https://github.com/HeliumEdu"</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
@@ -112,13 +112,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8289d082374b3103_main_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8289d082374b3103_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,21 +6,21 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import json 
 _2import os 
 _3 
 _4__author__ = "Alex Laird" 
 _5__copyright__ = "Copyright 2023, Helium Edu" 
-_6__version__ = "1.6.8" 
+_6__version__ = "1.6.9" 
 _7 
 _8VERSION = __version__ 
 _9 
 _1_0 
 _1_1def get_default_settings(): 
 _1_2 return { 
 _1_3 "gitProject": os.environ.get("HELIUMCLI_GIT_PROJECT", "https://github.com/
@@ -43,8 +43,8 @@
 _2_3 "path": os.environ.get("HELIUMCLI_VERSION_INFO_PATH", "conf/configs/
 common.py"), 
 _2_4 }, 
 _2_5 "remoteName": os.environ.get("HELIUMCLI_REMOTE_NAME", "origin"), 
 _2_6 "branchName": os.environ.get("HELIUMCLI_BRANCH_NAME", "main"), 
 _2_7 } 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_8289d082374b3103_utils_py.html` & `heliumcli-1.6.9/_build/coverage/d_8289d082374b3103_utils_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8289d082374b3103_settings_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -214,13 +214,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8289d082374b3103_settings_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 5599 ssttaatteemmeennttss ?  5566 rruunn 33 mmiissssiinngg 1144 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2import re 
 _3import subprocess 
 _4import sys 
 _5from builtins import input 
 _6 
 _7import yaml 
@@ -143,8 +143,8 @@
 _1_2_5 version_tags.append(git_tag) 
 _1_2_6 
 _1_2_7 version_tags.sort(key=lambda v: list(map(int, v.tag.tag.lstrip("v").split
 (".")))) 
 _1_2_8 
 _1_2_9 return version_tags 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b___init___py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8289d082374b3103___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_buildrelease_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8289d082374b3103___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_buildrelease_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_buildrelease_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_buildrelease_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_deploybuild_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -218,13 +218,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_deploybuild_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 8877 ssttaatteemmeennttss ?  7744 rruunn 1133 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import datetime 
 _2import os 
 _3import shutil 
 _4 
 _5import git 
 _6 
 _7from .. import utils 
@@ -148,8 +148,8 @@
 _1_2_8 
 _1_2_9 version_file.close() 
 _1_3_0 new_version_file.close() 
 _1_3_1 
 _1_3_2 shutil.copy(version_file_path + ".tmp", version_file_path) 
 _1_3_3 os.remove(version_file_path + ".tmp") 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_deploybuild_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_deploybuild_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_buildrelease_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_init_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -166,13 +166,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_buildrelease_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_init_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 5599 ssttaatteemmeennttss ?  5511 rruunn 88 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2import subprocess 
 _3 
 _4import git 
 _5 
 _6from .. import utils 
 _7 
@@ -96,8 +96,8 @@
 _7_7 if args.roles: 
 _7_8 playbook_options.append("--limit") 
 _7_9 playbook_options.append(",".join(args.roles)) 
 _8_0 
 _8_1 subprocess.call(["ansible-playbook"] + playbook_options + ["{}/
 {}.yml".format(ansible_dir, args.env)]) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_init_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_init_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_deploybuild_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_listbuilds_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -187,13 +187,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_deploybuild_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_listbuilds_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 7711 ssttaatteemmeennttss ?  6677 rruunn 44 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2import shutil 
 _3import subprocess 
 _4import sys 
 _5 
 _6import git 
 _7 
@@ -126,8 +126,8 @@
 _9_7 s = s.replace("{%PROJECT_ID_LOWER%}", self._lower_slug) 
 _9_8 s = s.replace("{%PROJECT_NAME%}", args.name) 
 _9_9 s = s.replace("{%PROJECT_GITHUB_USER%}", args.github_user) 
 _1_0_0 
 _1_0_1 with open(path, "w") as f: 
 _1_0_2 f.write(s) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_listbuilds_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_listbuilds_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_init_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_prepcode_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -131,13 +131,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_init_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_prepcode_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3322 ssttaatteemmeennttss ?  2200 rruunn 1122 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2 
 _3import git 
 _4 
 _5from .. import utils 
 _6 
 _7__author__ = "Alex Laird" 
@@ -55,8 +55,8 @@
 _4_1 print(version_tags[-1]) 
 _4_2 else: 
 _4_3 for tag in version_tags: 
 _4_4 print(tag) 
 _4_5 
 _4_6 print("") 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_prepcode_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_prepcode_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_listbuilds_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_setbuild_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -238,13 +238,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_listbuilds_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_setbuild_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 110011 ssttaatteemmeennttss ?  9955 rruunn 66 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import datetime 
 _2import os 
 _3import shutil 
 _4import subprocess 
 _5 
 _6import git 
 _7 
@@ -175,8 +175,8 @@
 _1_4_9 def _process_package_json(self, line): 
 _1_5_0 if utils.should_update(line, "\"version\": \"{}\",".format
 (self._current_version), "\"version\": \""): 
 _1_5_1 line = " \"version\": \"{}\",\n".format(self._current_version) 
 _1_5_2 return line, True 
 _1_5_3 return line, False 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_setbuild_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_setbuild_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_prepcode_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_startservers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -137,13 +137,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_prepcode_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_startservers_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3366 ssttaatteemmeennttss ?  3355 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2import subprocess 
 _3 
 _4import git 
 _5 
 _6from .. import utils 
 _7 
@@ -62,8 +62,8 @@
 _4_7 repo.git.fetch(tags=True, prune=True) 
 _4_8 repo.git.checkout(args.version) 
 _4_9 
 _5_0 subprocess.call(["make", "install", "-C", project_path]) 
 _5_1 
 _5_2 print("") 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_startservers_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_startservers_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_setbuild_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_update_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -125,13 +125,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_setbuild_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_update_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2277 ssttaatteemmeennttss ?  2266 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2import subprocess 
 _3 
 _4from .. import utils 
 _5 
 _6__author__ = "Alex Laird" 
 _7__copyright__ = "Copyright 2018, Helium Edu" 
@@ -48,8 +48,8 @@
 _3_5 
 _3_6 if os.path.exists(runserver_bin): 
 _3_7 processes.append(subprocess.Popen(runserver_bin)) 
 _3_8 
 _3_9 if len(processes) > 0: 
 _4_0 processes[-1].wait() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_update_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_update_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_startservers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_updateprojects_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -103,13 +103,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_startservers_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b1a8285c6e0e875b_updateprojects_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1133 ssttaatteemmeennttss ?  1133 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import subprocess 
 _2 
 _3__author__ = "Alex Laird" 
 _4__copyright__ = "Copyright 2018, Helium Edu" 
 _5__version__ = "1.5.0" 
 _6 
 _7 
@@ -26,8 +26,8 @@
 _1_3 def setup(self, subparsers): 
 _1_4 parser = subparsers.add_parser(self.name, help=self.help) 
 _1_5 parser.set_defaults(action=self) 
 _1_6 
 _1_7 def run(self, args): 
 _1_8 subprocess.call(["pip", "install", "--upgrade", "heliumcli"]) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/d_b1a8285c6e0e875b_updateprojects_py.html` & `heliumcli-1.6.9/_build/coverage/d_b1a8285c6e0e875b_updateprojects_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for heliumcli/actions/updateprojects.py: 97.44%</title>
+    <title>Coverage for heliumcli/actions/updateprojects.py: 97.50%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>heliumcli/actions/updateprojects.py</b>:
-            <span class="pc_cov">97.44%</span>
+            <span class="pc_cov">97.50%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">39 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">38<span class="text"> run</span></button>
+            <span class="text">40 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">39<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">1<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_update_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8289d082374b3103_main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -108,46 +108,47 @@
     <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">if</span> <span class="nam">config</span><span class="op">[</span><span class="str">"projectsRelativeDir"</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">            <span class="nam">root_dir</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">abspath</span><span class="op">(</span><span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">,</span> <span class="str">".."</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="key">if</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">root_dir</span><span class="op">,</span> <span class="str">".git"</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="nam">utils</span><span class="op">.</span><span class="nam">get_repo_name</span><span class="op">(</span><span class="nam">root_dir</span><span class="op">,</span> <span class="nam">config</span><span class="op">[</span><span class="str">"remoteName"</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">                <span class="nam">repo</span> <span class="op">=</span> <span class="nam">git</span><span class="op">.</span><span class="nam">Repo</span><span class="op">(</span><span class="nam">root_dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">                <span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">fetch</span><span class="op">(</span><span class="nam">tags</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">prune</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">force</span><span class="op">=</span><span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"HELIUMCLI_FORCE_FETCH"</span><span class="op">,</span> <span class="str">"False"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"True"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">pull</span><span class="op">(</span><span class="op">)</span> <span class="op">+</span> <span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">            <span class="nam">os</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="key">for</span> <span class="nam">project</span> <span class="key">in</span> <span class="nam">utils</span><span class="op">.</span><span class="nam">get_projects</span><span class="op">(</span><span class="nam">config</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">project</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="key">if</span> <span class="nam">config</span><span class="op">[</span><span class="str">"projectsRelativeDir"</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">                <span class="nam">project_path</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">,</span> <span class="nam">project</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">                <span class="nam">project_path</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">project_path</span><span class="op">,</span> <span class="str">".git"</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="str">"Cloning repo to ./projects/{}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">project</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">                <span class="nam">git</span><span class="op">.</span><span class="nam">Repo</span><span class="op">.</span><span class="nam">clone_from</span><span class="op">(</span><span class="str">"{}/{}.git"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">config</span><span class="op">[</span><span class="str">"gitProject"</span><span class="op">]</span><span class="op">,</span> <span class="nam">project</span><span class="op">)</span><span class="op">,</span> <span class="nam">project_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">                <span class="nam">repo</span> <span class="op">=</span> <span class="nam">git</span><span class="op">.</span><span class="nam">Repo</span><span class="op">(</span><span class="nam">project_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">                <span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">fetch</span><span class="op">(</span><span class="nam">tags</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">prune</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">force</span><span class="op">=</span><span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"HELIUMCLI_FORCE_FETCH"</span><span class="op">,</span> <span class="str">"False"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"True"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">pull</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">subprocess</span><span class="op">.</span><span class="nam">call</span><span class="op">(</span><span class="op">[</span><span class="str">"make"</span><span class="op">,</span> <span class="str">"install"</span><span class="op">,</span> <span class="str">"-C"</span><span class="op">,</span> <span class="nam">project_path</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">                <span class="key">if</span> <span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"HELIUMCLI_SKIP_UPDATE_PULL"</span><span class="op">,</span> <span class="str">"False"</span><span class="op">)</span> <span class="op">!=</span> <span class="str">"True"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">                    <span class="nam">print</span><span class="op">(</span><span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">pull</span><span class="op">(</span><span class="op">)</span> <span class="op">+</span> <span class="str">"\n"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="nam">os</span><span class="op">.</span><span class="nam">mkdir</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">for</span> <span class="nam">project</span> <span class="key">in</span> <span class="nam">utils</span><span class="op">.</span><span class="nam">get_projects</span><span class="op">(</span><span class="nam">config</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">project</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="key">if</span> <span class="nam">config</span><span class="op">[</span><span class="str">"projectsRelativeDir"</span><span class="op">]</span> <span class="op">!=</span> <span class="str">"."</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">                <span class="nam">project_path</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">,</span> <span class="nam">project</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">                <span class="nam">project_path</span> <span class="op">=</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">projects_dir</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">exists</span><span class="op">(</span><span class="nam">os</span><span class="op">.</span><span class="nam">path</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">project_path</span><span class="op">,</span> <span class="str">".git"</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="str">"Cloning repo to ./projects/{}"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">project</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">                <span class="nam">git</span><span class="op">.</span><span class="nam">Repo</span><span class="op">.</span><span class="nam">clone_from</span><span class="op">(</span><span class="str">"{}/{}.git"</span><span class="op">.</span><span class="nam">format</span><span class="op">(</span><span class="nam">config</span><span class="op">[</span><span class="str">"gitProject"</span><span class="op">]</span><span class="op">,</span> <span class="nam">project</span><span class="op">)</span><span class="op">,</span> <span class="nam">project_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">                <span class="nam">repo</span> <span class="op">=</span> <span class="nam">git</span><span class="op">.</span><span class="nam">Repo</span><span class="op">(</span><span class="nam">project_path</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">fetch</span><span class="op">(</span><span class="nam">tags</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">prune</span><span class="op">=</span><span class="key">True</span><span class="op">,</span> <span class="nam">force</span><span class="op">=</span><span class="nam">os</span><span class="op">.</span><span class="nam">environ</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"HELIUMCLI_FORCE_FETCH"</span><span class="op">,</span> <span class="str">"False"</span><span class="op">)</span> <span class="op">==</span> <span class="str">"True"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="nam">repo</span><span class="op">.</span><span class="nam">git</span><span class="op">.</span><span class="nam">pull</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">            <span class="nam">subprocess</span><span class="op">.</span><span class="nam">call</span><span class="op">(</span><span class="op">[</span><span class="str">"make"</span><span class="op">,</span> <span class="str">"install"</span><span class="op">,</span> <span class="str">"-C"</span><span class="op">,</span> <span class="nam">project_path</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="str">""</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b1a8285c6e0e875b_update_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8289d082374b3103_main_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr hheelliiuummccllii//aaccttiioonnss//uuppddaatteepprroojjeeccttss..ppyy:: 9977..4444%% ************
+************ CCoovveerraaggee ffoorr hheelliiuummccllii//aaccttiioonnss//uuppddaatteepprroojjeeccttss..ppyy:: 9977..5500%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3399 ssttaatteemmeennttss ?  3388 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 4400 ssttaatteemmeennttss ?  3399 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
 _1import os 
 _2import subprocess 
 _3 
 _4import git 
 _5 
 _6from .. import utils 
 _7 
@@ -41,35 +41,36 @@
 _2_7 root_dir = os.path.abspath(os.path.join(projects_dir, "..")) 
 _2_8 if os.path.exists(os.path.join(root_dir, ".git")): 
 _2_9 print(utils.get_repo_name(root_dir, config["remoteName"])) 
 _3_0 
 _3_1 repo = git.Repo(root_dir) 
 _3_2 repo.git.fetch(tags=True, prune=True, force=os.environ.get
 ("HELIUMCLI_FORCE_FETCH", "False") == "True") 
-_3_3 print(repo.git.pull() + "\n") 
-_3_4 
-_3_5 if not os.path.exists(projects_dir): 
-_3_6 os.mkdir(projects_dir) 
-_3_7 
-_3_8 for project in utils.get_projects(config): 
-_3_9 print(project) 
-_4_0 
-_4_1 if config["projectsRelativeDir"] != ".": 
-_4_2 project_path = os.path.join(projects_dir, project) 
-_4_3 else: 
-_4_4 project_path = os.path.join(projects_dir) 
-_4_5 
-_4_6 if not os.path.exists(os.path.join(project_path, ".git")): 
-_4_7 print("Cloning repo to ./projects/{}".format(project)) 
-_4_8 git.Repo.clone_from("{}/{}.git".format(config["gitProject"], project),
+_3_3 if os.environ.get("HELIUMCLI_SKIP_UPDATE_PULL", "False") != "True": 
+_3_4 print(repo.git.pull() + "\n") 
+_3_5 
+_3_6 if not os.path.exists(projects_dir): 
+_3_7 os.mkdir(projects_dir) 
+_3_8 
+_3_9 for project in utils.get_projects(config): 
+_4_0 print(project) 
+_4_1 
+_4_2 if config["projectsRelativeDir"] != ".": 
+_4_3 project_path = os.path.join(projects_dir, project) 
+_4_4 else: 
+_4_5 project_path = os.path.join(projects_dir) 
+_4_6 
+_4_7 if not os.path.exists(os.path.join(project_path, ".git")): 
+_4_8 print("Cloning repo to ./projects/{}".format(project)) 
+_4_9 git.Repo.clone_from("{}/{}.git".format(config["gitProject"], project),
 project_path) 
-_4_9 else: 
-_5_0 repo = git.Repo(project_path) 
-_5_1 repo.git.fetch(tags=True, prune=True, force=os.environ.get
+_5_0 else: 
+_5_1 repo = git.Repo(project_path) 
+_5_2 repo.git.fetch(tags=True, prune=True, force=os.environ.get
 ("HELIUMCLI_FORCE_FETCH", "False") == "True") 
-_5_2 print(repo.git.pull()) 
-_5_3 
-_5_4 subprocess.call(["make", "install", "-C", project_path]) 
-_5_5 
-_5_6 print("") 
+_5_3 print(repo.git.pull()) 
+_5_4 
+_5_5 subprocess.call(["make", "install", "-C", project_path]) 
+_5_6 
+_5_7 print("") 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-
-22 17:03 +0000
+22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/favicon_32.png` & `heliumcli-1.6.9/_build/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/_build/coverage/index.html` & `heliumcli-1.6.9/_build/coverage/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Helium CLI Coverage Report:
-            <span class="pc_cov">91.23%</span>
+            <span class="pc_cov">91.25%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -129,18 +129,18 @@
                 <td>13</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="13 13">100.00%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_b1a8285c6e0e875b_updateprojects_py.html">heliumcli/actions/updateprojects.py</a></td>
-                <td>39</td>
+                <td>40</td>
                 <td>1</td>
                 <td>0</td>
-                <td class="right" data-ratio="38 39">97.44%</td>
+                <td class="right" data-ratio="39 40">97.50%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8289d082374b3103_main_py.html">heliumcli/main.py</a></td>
                 <td>27</td>
                 <td>0</td>
                 <td>8</td>
                 <td class="right" data-ratio="27 27">100.00%</td>
@@ -159,30 +159,30 @@
                 <td>14</td>
                 <td class="right" data-ratio="56 59">94.92%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>559</td>
+                <td>560</td>
                 <td>49</td>
                 <td>22</td>
-                <td class="right" data-ratio="510 559">91.23%</td>
+                <td class="right" data-ratio="511 560">91.25%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.3.2">coverage.py v7.3.2</a>,
-            created at 2023-11-22 17:03 +0000
+            created at 2023-11-22 17:35 +0000
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_8289d082374b3103_utils_py.html"/>
         <a id="nextFileLink" class="nav" href="d_8289d082374b3103___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-************ HHeelliiuumm CCLLII CCoovveerraaggee RReeppoorrtt:: 9911..2233%% ************
+************ HHeelliiuumm CCLLII CCoovveerraaggee RReeppoorrtt:: 9911..2255%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-22 17:03 +0000
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-22 17:35 +0000
 MMoodduullee                              ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _h_e_l_i_u_m_c_l_i_/_____i_n_i_t_____._p_y               0          0       0        100.00%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_____i_n_i_t_____._p_y       0          0       0        100.00%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_b_u_i_l_d_r_e_l_e_a_s_e_._p_y   87         13      0        85.06%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_d_e_p_l_o_y_b_u_i_l_d_._p_y    59         8       0        86.44%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_i_n_i_t_._p_y           71         4       0        94.37%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_l_i_s_t_b_u_i_l_d_s_._p_y     32         12      0        62.50%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_p_r_e_p_c_o_d_e_._p_y       101        6       0        94.06%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_s_e_t_b_u_i_l_d_._p_y       36         1       0        97.22%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_s_t_a_r_t_s_e_r_v_e_r_s_._p_y   27         1       0        96.30%
 _h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_u_p_d_a_t_e_._p_y         13         0       0        100.00%
-_h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_u_p_d_a_t_e_p_r_o_j_e_c_t_s_._p_y 39         1       0        97.44%
+_h_e_l_i_u_m_c_l_i_/_a_c_t_i_o_n_s_/_u_p_d_a_t_e_p_r_o_j_e_c_t_s_._p_y 40         1       0        97.50%
 _h_e_l_i_u_m_c_l_i_/_m_a_i_n_._p_y                   27         0       8        100.00%
 _h_e_l_i_u_m_c_l_i_/_s_e_t_t_i_n_g_s_._p_y               8          0       0        100.00%
 _h_e_l_i_u_m_c_l_i_/_u_t_i_l_s_._p_y                  59         3       14       94.92%
-Total                               559        49      22       91.23%
+Total                               560        49      22       91.25%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-22 17:03 +0000
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._3_._2, created at 2023-11-22 17:35 +0000
```

### Comparing `heliumcli-1.6.8/_build/coverage/keybd_closed.png` & `heliumcli-1.6.9/_build/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/_build/coverage/keybd_open.png` & `heliumcli-1.6.9/_build/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/_build/coverage/status.json` & `heliumcli-1.6.9/_build/coverage/status.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977265211640212%*

 * *Differences: {"'files'": "{'d_b1a8285c6e0e875b_updateprojects_py': {'hash': '1527e77eb05eedfbf48baeab335be3f5', "*

 * *            "'index': {'nums': {insert: [(2, 40)], delete: [2]}}}, "*

 * *            "'d_8289d082374b3103_settings_py': {'hash': '5fd9152782a91bb35ac68e7d709fb5b8'}}"}*

```diff
@@ -31,15 +31,15 @@
                     0,
                     0
                 ],
                 "relative_filename": "heliumcli/main.py"
             }
         },
         "d_8289d082374b3103_settings_py": {
-            "hash": "3c3b4c835b62aea08a8173afe8d1ea27",
+            "hash": "5fd9152782a91bb35ac68e7d709fb5b8",
             "index": {
                 "html_filename": "d_8289d082374b3103_settings_py.html",
                 "nums": [
                     2,
                     1,
                     8,
                     0,
@@ -218,21 +218,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "heliumcli/actions/update.py"
             }
         },
         "d_b1a8285c6e0e875b_updateprojects_py": {
-            "hash": "2518d1839c4f69c1d5b2a8dc237a8219",
+            "hash": "1527e77eb05eedfbf48baeab335be3f5",
             "index": {
                 "html_filename": "d_b1a8285c6e0e875b_updateprojects_py.html",
                 "nums": [
                     2,
                     1,
-                    39,
+                    40,
                     0,
                     1,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "heliumcli/actions/updateprojects.py"
```

### Comparing `heliumcli-1.6.8/_build/coverage/style.css` & `heliumcli-1.6.9/_build/coverage/style.css`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/buildrelease.py` & `heliumcli-1.6.9/heliumcli/actions/buildrelease.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/deploybuild.py` & `heliumcli-1.6.9/heliumcli/actions/deploybuild.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/init.py` & `heliumcli-1.6.9/heliumcli/actions/init.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/listbuilds.py` & `heliumcli-1.6.9/heliumcli/actions/listbuilds.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/prepcode.py` & `heliumcli-1.6.9/heliumcli/actions/prepcode.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/setbuild.py` & `heliumcli-1.6.9/heliumcli/actions/setbuild.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/startservers.py` & `heliumcli-1.6.9/heliumcli/actions/startservers.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/actions/updateprojects.py` & `heliumcli-1.6.9/heliumcli/actions/updateprojects.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         if config["projectsRelativeDir"] != ".":
             root_dir = os.path.abspath(os.path.join(projects_dir, ".."))
             if os.path.exists(os.path.join(root_dir, ".git")):
                 print(utils.get_repo_name(root_dir, config["remoteName"]))
 
                 repo = git.Repo(root_dir)
                 repo.git.fetch(tags=True, prune=True, force=os.environ.get("HELIUMCLI_FORCE_FETCH", "False") == "True")
-                print(repo.git.pull() + "\n")
+                if os.environ.get("HELIUMCLI_SKIP_UPDATE_PULL", "False") != "True":
+                    print(repo.git.pull() + "\n")
 
         if not os.path.exists(projects_dir):
             os.mkdir(projects_dir)
 
         for project in utils.get_projects(config):
             print(project)
```

### Comparing `heliumcli-1.6.8/heliumcli/main.py` & `heliumcli-1.6.9/heliumcli/main.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli/settings.py` & `heliumcli-1.6.9/heliumcli/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 
 __author__ = "Alex Laird"
 __copyright__ = "Copyright 2023, Helium Edu"
-__version__ = "1.6.8"
+__version__ = "1.6.9"
 
 VERSION = __version__
 
 
 def get_default_settings():
     return {
         "gitProject": os.environ.get("HELIUMCLI_GIT_PROJECT", "https://github.com/HeliumEdu"),
```

### Comparing `heliumcli-1.6.8/heliumcli/utils.py` & `heliumcli-1.6.9/heliumcli/utils.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/heliumcli.egg-info/PKG-INFO` & `heliumcli-1.6.9/heliumcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: heliumcli
-Version: 1.6.8
+Version: 1.6.9
 Summary: CLI tool that provides a useful set of tools for maintaining, building, and deploying code in compatible projects
 Home-page: https://github.com/HeliumEdu/heliumcli
-Download-URL: https://github.com/HeliumEdu/heliumcli/archive/1.6.8.tar.gz
+Download-URL: https://github.com/HeliumEdu/heliumcli/archive/1.6.9.tar.gz
 Author: Alex Laird
 Author-email: contact@alexlaird.com
 License: MIT
 Project-URL: Sponsor, https://github.com/sponsors/alexdlaird
 Keywords: cli,build,deployment,ansible,git
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `heliumcli-1.6.8/heliumcli.egg-info/SOURCES.txt` & `heliumcli-1.6.9/heliumcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/setup.py` & `heliumcli-1.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/tests/testactions.py` & `heliumcli-1.6.9/tests/testactions.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/tests/testconfig.py` & `heliumcli-1.6.9/tests/testconfig.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/tests/testinit.py` & `heliumcli-1.6.9/tests/testinit.py`

 * *Files identical despite different names*

### Comparing `heliumcli-1.6.8/tests/testutils.py` & `heliumcli-1.6.9/tests/testutils.py`

 * *Files identical despite different names*


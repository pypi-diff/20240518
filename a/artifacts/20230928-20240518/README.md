# Comparing `tmp/artifacts-20230928.tar.gz` & `tmp/artifacts-20240518.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artifacts-20230928.tar", last modified: Thu Sep 28 12:39:38 2023, max compression
+gzip compressed data, was "artifacts-20240518.tar", last modified: Sat May 18 05:37:27 2024, max compression
```

## Comparing `artifacts-20230928.tar` & `artifacts-20240518.tar`

### file list

```diff
@@ -1,129 +1,133 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.370903 artifacts-20230928/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.165903 artifacts-20230928/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.237903 artifacts-20230928/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2515 2023-09-03 09:48:25.000000 artifacts-20230928/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1366 2023-09-03 09:48:25.000000 artifacts-20230928/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4070 2023-09-03 09:48:25.000000 artifacts-20230928/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22994 2023-09-03 09:48:25.000000 artifacts-20230928/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-12-20 18:52:11.000000 artifacts-20230928/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2021-11-01 18:53:11.000000 artifacts-20230928/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      488 2014-11-26 17:20:08.000000 artifacts-20230928/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11325 2014-11-19 19:52:15.000000 artifacts-20230928/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      609 2022-12-20 18:52:11.000000 artifacts-20230928/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      674 2023-09-28 12:39:38.370903 artifacts-20230928/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      303 2022-12-20 18:52:11.000000 artifacts-20230928/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      932 2022-12-20 18:52:11.000000 artifacts-20230928/README.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-09-03 09:48:25.000000 artifacts-20230928/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.240903 artifacts-20230928/artifacts/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2023-09-28 12:34:48.000000 artifacts-20230928/artifacts/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3274 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts/artifact.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      946 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      387 2018-03-18 07:06:42.000000 artifacts-20230928/artifacts/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10920 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts/reader.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8516 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts/registry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13704 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts/source_type.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2733 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts/writer.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.241903 artifacts-20230928/artifacts.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      674 2023-09-28 12:39:36.000000 artifacts-20230928/artifacts.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2452 2023-09-28 12:39:37.000000 artifacts-20230928/artifacts.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-09-28 12:39:36.000000 artifacts-20230928/artifacts.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-09-28 12:39:36.000000 artifacts-20230928/artifacts.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       10 2023-09-28 12:39:36.000000 artifacts-20230928/artifacts.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      529 2022-12-20 18:52:11.000000 artifacts-20230928/artifacts.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.166903 artifacts-20230928/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.253903 artifacts-20230928/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2023-09-03 09:48:25.000000 artifacts-20230928/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-09-03 09:48:25.000000 artifacts-20230928/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-09-03 09:48:25.000000 artifacts-20230928/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.305903 artifacts-20230928/config/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       21 2017-05-20 19:17:24.000000 artifacts-20230928/config/dpkg/artifacts-data.dirs
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2017-07-01 08:08:23.000000 artifacts-20230928/config/dpkg/artifacts-data.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        8 2017-05-21 20:05:37.000000 artifacts-20230928/config/dpkg/artifacts-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      159 2023-09-28 12:34:48.000000 artifacts-20230928/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2017-05-20 19:17:24.000000 artifacts-20230928/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-09-03 09:48:25.000000 artifacts-20230928/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2023-09-03 09:48:25.000000 artifacts-20230928/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2017-05-13 17:01:46.000000 artifacts-20230928/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2017-05-20 19:17:24.000000 artifacts-20230928/config/dpkg/python3-artifacts.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-09-03 09:48:25.000000 artifacts-20230928/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.306903 artifacts-20230928/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-05-20 19:17:24.000000 artifacts-20230928/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.323903 artifacts-20230928/data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6762 2022-12-20 18:52:11.000000 artifacts-20230928/data/antivirus.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4248 2022-12-20 18:52:11.000000 artifacts-20230928/data/applications.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2787 2022-12-20 18:52:11.000000 artifacts-20230928/data/cloud_services.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1664 2022-12-20 18:52:11.000000 artifacts-20230928/data/config_files.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-12-20 18:52:11.000000 artifacts-20230928/data/containerd.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6324 2022-12-20 18:52:11.000000 artifacts-20230928/data/database_servers.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2022-12-20 18:52:11.000000 artifacts-20230928/data/docker.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3602 2022-12-20 18:52:11.000000 artifacts-20230928/data/esxi.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2022-12-20 18:52:11.000000 artifacts-20230928/data/file_systems.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2022-12-20 18:52:11.000000 artifacts-20230928/data/hadoop.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2023-01-30 17:22:48.000000 artifacts-20230928/data/ics.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2022-12-20 18:52:11.000000 artifacts-20230928/data/installed_module_paths.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5243 2022-12-20 18:52:11.000000 artifacts-20230928/data/installed_modules.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2316 2023-01-30 17:22:48.000000 artifacts-20230928/data/instant_messaging.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      558 2022-12-20 18:52:11.000000 artifacts-20230928/data/java.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5174 2022-12-20 18:52:11.000000 artifacts-20230928/data/kaspersky_careto.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5223 2022-12-20 18:52:11.000000 artifacts-20230928/data/kubernetes.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2743 2022-12-20 18:52:11.000000 artifacts-20230928/data/legacy.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24996 2023-09-28 11:23:28.000000 artifacts-20230928/data/linux.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5117 2022-12-20 18:52:11.000000 artifacts-20230928/data/linux_proc.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2022-12-20 18:52:11.000000 artifacts-20230928/data/linux_services.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35506 2023-08-15 04:45:56.000000 artifacts-20230928/data/macos.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8373 2022-12-20 18:52:11.000000 artifacts-20230928/data/shell.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2022-12-20 18:52:11.000000 artifacts-20230928/data/tomcat.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8988 2022-12-20 18:52:11.000000 artifacts-20230928/data/triage.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2855 2023-07-23 09:17:05.000000 artifacts-20230928/data/unix_common.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      892 2023-01-30 17:22:48.000000 artifacts-20230928/data/user.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75728 2023-08-11 05:28:06.000000 artifacts-20230928/data/webbrowser.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2884 2022-12-20 18:52:11.000000 artifacts-20230928/data/webservers.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   168123 2023-09-28 11:23:28.000000 artifacts-20230928/data/windows.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6174 2022-12-20 18:52:11.000000 artifacts-20230928/data/windows_dll_hijacking.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8549 2022-12-20 18:52:11.000000 artifacts-20230928/data/wmi.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      150 2021-11-01 18:53:11.000000 artifacts-20230928/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.334903 artifacts-20230928/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       88 2022-12-20 18:52:11.000000 artifacts-20230928/docs/Artifacts definition format and style guide.asciidoc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2023-09-03 09:48:25.000000 artifacts-20230928/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      673 2022-12-20 18:52:11.000000 artifacts-20230928/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-09-03 09:48:25.000000 artifacts-20230928/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.334903 artifacts-20230928/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15892 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/Format-specification.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.335903 artifacts-20230928/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1176 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/api/artifacts.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       64 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.335903 artifacts-20230928/docs/sources/background/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      739 2023-09-28 12:34:48.000000 artifacts-20230928/docs/sources/background/Stats.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      873 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/background/Terminology.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/background/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.336903 artifacts-20230928/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      311 2022-12-20 18:52:11.000000 artifacts-20230928/docs/sources/user/index.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-09-03 09:48:25.000000 artifacts-20230928/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2022-12-20 18:52:11.000000 artifacts-20230928/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      320 2023-09-28 12:39:38.371903 artifacts-20230928/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6702 2023-09-03 09:48:46.000000 artifacts-20230928/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.336903 artifacts-20230928/test_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2422 2022-12-20 18:52:11.000000 artifacts-20230928/test_data/definitions.json
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2312 2022-12-20 18:52:11.000000 artifacts-20230928/test_data/definitions.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-20 18:52:11.000000 artifacts-20230928/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-03 09:48:25.000000 artifacts-20230928/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.348903 artifacts-20230928/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2021-11-01 18:53:11.000000 artifacts-20230928/tests/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11907 2022-12-20 18:52:11.000000 artifacts-20230928/tests/reader_test.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4906 2022-12-20 18:52:11.000000 artifacts-20230928/tests/registry_test.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5365 2022-12-20 18:52:11.000000 artifacts-20230928/tests/source_type_test.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2022-12-20 18:52:11.000000 artifacts-20230928/tests/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1135 2022-12-20 18:52:11.000000 artifacts-20230928/tests/validator_test.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2022-12-20 18:52:11.000000 artifacts-20230928/tests/writer_test.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.356903 artifacts-20230928/tools/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       46 2021-11-01 18:53:12.000000 artifacts-20230928/tools/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4074 2023-08-09 04:19:04.000000 artifacts-20230928/tools/stats.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    21234 2023-09-03 12:02:14.000000 artifacts-20230928/tools/validator.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1055 2023-09-03 09:48:46.000000 artifacts-20230928/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-09-28 12:39:38.370903 artifacts-20230928/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2018-03-18 07:06:41.000000 artifacts-20230928/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-09-03 09:48:25.000000 artifacts-20230928/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-09-03 09:48:25.000000 artifacts-20230928/utils/dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9073 2015-05-07 21:05:55.000000 artifacts-20230928/utils/pylintrc
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      675 2022-12-20 18:52:11.000000 artifacts-20230928/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.152580 artifacts-20240518/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.138580 artifacts-20240518/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.142580 artifacts-20240518/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2423 2024-05-13 04:50:53.000000 artifacts-20240518/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1372 2024-05-13 04:50:53.000000 artifacts-20240518/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4170 2024-05-13 04:50:53.000000 artifacts-20240518/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-05-13 04:39:45.000000 artifacts-20240518/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-05-13 04:39:45.000000 artifacts-20240518/.readthedocs.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 10:42:59.000000 artifacts-20240518/.yamllint.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2023-12-03 10:43:00.000000 artifacts-20240518/ACKNOWLEDGEMENTS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      488 2023-12-03 10:43:00.000000 artifacts-20240518/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11325 2023-12-03 10:43:00.000000 artifacts-20240518/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      584 2024-01-07 10:18:36.000000 artifacts-20240518/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      717 2024-05-18 05:37:27.152580 artifacts-20240518/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      303 2023-12-03 10:42:59.000000 artifacts-20240518/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      932 2023-12-03 10:43:00.000000 artifacts-20240518/README.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-05-13 04:39:45.000000 artifacts-20240518/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.142580 artifacts-20240518/artifacts/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2024-05-18 05:37:13.000000 artifacts-20240518/artifacts/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3088 2024-03-05 05:21:29.000000 artifacts-20240518/artifacts/artifact.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.146580 artifacts-20240518/artifacts/data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6762 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/antivirus.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4248 2024-01-10 04:23:51.000000 artifacts-20240518/artifacts/data/applications.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2787 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/cloud_services.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1664 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/config_files.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      812 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/containerd.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6324 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/database_servers.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/docker.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3602 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/esxi.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-01-10 04:23:51.000000 artifacts-20240518/artifacts/data/file_systems.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1258 2024-01-10 04:23:51.000000 artifacts-20240518/artifacts/data/hadoop.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/ics.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/installed_module_paths.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5243 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/installed_modules.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2316 2024-01-10 04:23:51.000000 artifacts-20240518/artifacts/data/instant_messaging.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      558 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/java.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5174 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/kaspersky_careto.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5223 2024-01-10 04:23:51.000000 artifacts-20240518/artifacts/data/kubernetes.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2525 2024-02-10 10:02:11.000000 artifacts-20240518/artifacts/data/legacy.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24948 2024-04-01 06:45:49.000000 artifacts-20240518/artifacts/data/linux.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5117 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/linux_proc.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/linux_services.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43242 2024-02-18 12:30:30.000000 artifacts-20240518/artifacts/data/macos.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8373 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/shell.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4201 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/tomcat.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8992 2024-04-01 06:45:49.000000 artifacts-20240518/artifacts/data/triage.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3407 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/unix_common.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      874 2024-02-10 10:02:11.000000 artifacts-20240518/artifacts/data/user.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    90521 2024-04-01 06:45:49.000000 artifacts-20240518/artifacts/data/webbrowser.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2951 2024-04-01 06:45:49.000000 artifacts-20240518/artifacts/data/webservers.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   171225 2024-05-18 05:32:09.000000 artifacts-20240518/artifacts/data/windows.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6174 2024-01-07 10:18:36.000000 artifacts-20240518/artifacts/data/windows_dll_hijacking.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8494 2024-02-10 10:02:11.000000 artifacts-20240518/artifacts/data/wmi.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1112 2024-05-18 05:32:09.000000 artifacts-20240518/artifacts/definitions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      387 2023-12-03 10:44:55.000000 artifacts-20240518/artifacts/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10520 2024-03-05 05:21:29.000000 artifacts-20240518/artifacts/reader.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8512 2024-01-14 04:58:18.000000 artifacts-20240518/artifacts/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.146580 artifacts-20240518/artifacts/scripts/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       46 2024-01-28 17:41:59.000000 artifacts-20240518/artifacts/scripts/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4195 2024-01-28 17:41:59.000000 artifacts-20240518/artifacts/scripts/stats.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    21746 2024-01-28 17:41:59.000000 artifacts-20240518/artifacts/scripts/validator.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13572 2024-03-05 05:33:19.000000 artifacts-20240518/artifacts/source_type.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2465 2024-03-05 05:21:29.000000 artifacts-20240518/artifacts/writer.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.152580 artifacts-20240518/artifacts.egg-info/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      717 2024-05-18 05:37:27.000000 artifacts-20240518/artifacts.egg-info/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2916 2024-05-18 05:37:27.000000 artifacts-20240518/artifacts.egg-info/SOURCES.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-05-18 05:37:27.000000 artifacts-20240518/artifacts.egg-info/dependency_links.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      100 2024-05-18 05:37:27.000000 artifacts-20240518/artifacts.egg-info/entry_points.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       13 2024-05-18 05:37:27.000000 artifacts-20240518/artifacts.egg-info/requires.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       10 2024-05-18 05:37:27.000000 artifacts-20240518/artifacts.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      529 2023-12-03 10:43:00.000000 artifacts-20240518/artifacts.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.138580 artifacts-20240518/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.147580 artifacts-20240518/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2024-05-13 04:39:45.000000 artifacts-20240518/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-05-13 04:39:45.000000 artifacts-20240518/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-05-13 04:39:45.000000 artifacts-20240518/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.148580 artifacts-20240518/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       21 2023-12-03 10:44:54.000000 artifacts-20240518/config/dpkg/artifacts-data.dirs
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2024-03-03 09:18:24.000000 artifacts-20240518/config/dpkg/artifacts-data.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        8 2023-12-03 10:44:54.000000 artifacts-20240518/config/dpkg/artifacts-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      159 2024-05-18 05:37:13.000000 artifacts-20240518/config/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-12-03 10:44:54.000000 artifacts-20240518/config/dpkg/clean
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-05-13 04:39:45.000000 artifacts-20240518/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-05-13 04:40:03.000000 artifacts-20240518/config/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1017 2023-12-03 10:44:54.000000 artifacts-20240518/config/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       99 2023-12-03 10:44:54.000000 artifacts-20240518/config/dpkg/python3-artifacts.install
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      485 2024-05-13 04:40:03.000000 artifacts-20240518/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.149580 artifacts-20240518/config/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 10:44:54.000000 artifacts-20240518/config/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      150 2023-12-03 10:42:59.000000 artifacts-20240518/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.149580 artifacts-20240518/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       88 2024-02-10 07:22:25.000000 artifacts-20240518/docs/Artifacts definition format and style guide.asciidoc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2024-05-13 04:39:45.000000 artifacts-20240518/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      673 2024-02-10 07:22:25.000000 artifacts-20240518/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-05-13 04:39:45.000000 artifacts-20240518/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.149580 artifacts-20240518/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16117 2024-05-18 05:32:09.000000 artifacts-20240518/docs/sources/Format-specification.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.149580 artifacts-20240518/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1253 2024-02-10 07:22:25.000000 artifacts-20240518/docs/sources/api/artifacts.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      525 2024-02-10 07:22:25.000000 artifacts-20240518/docs/sources/api/artifacts.scripts.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       64 2024-02-10 07:22:25.000000 artifacts-20240518/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.150580 artifacts-20240518/docs/sources/background/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      759 2024-05-18 05:37:13.000000 artifacts-20240518/docs/sources/background/Stats.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      873 2024-02-10 07:22:25.000000 artifacts-20240518/docs/sources/background/Terminology.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1276 2024-02-10 07:22:25.000000 artifacts-20240518/docs/sources/background/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.150580 artifacts-20240518/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1721 2024-02-10 07:44:35.000000 artifacts-20240518/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      311 2024-02-10 07:22:25.000000 artifacts-20240518/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-05-13 04:39:45.000000 artifacts-20240518/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       15 2024-05-13 04:39:45.000000 artifacts-20240518/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2023-12-03 10:42:59.000000 artifacts-20240518/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1093 2024-05-18 05:37:27.153580 artifacts-20240518/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-05-13 04:39:45.000000 artifacts-20240518/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.150580 artifacts-20240518/test_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2313 2024-02-10 07:17:12.000000 artifacts-20240518/test_data/definitions.json
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2218 2024-02-10 07:17:12.000000 artifacts-20240518/test_data/definitions.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:43:00.000000 artifacts-20240518/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-13 04:39:45.000000 artifacts-20240518/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.151580 artifacts-20240518/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:44:53.000000 artifacts-20240518/tests/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11732 2024-02-10 07:17:12.000000 artifacts-20240518/tests/reader_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4978 2024-01-14 04:58:18.000000 artifacts-20240518/tests/registry_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5365 2023-12-03 10:44:53.000000 artifacts-20240518/tests/source_type_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-01-07 10:18:36.000000 artifacts-20240518/tests/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1253 2024-01-28 17:41:59.000000 artifacts-20240518/tests/validator_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2023-12-03 10:44:53.000000 artifacts-20240518/tests/writer_test.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-05-13 04:39:45.000000 artifacts-20240518/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-18 05:37:27.152580 artifacts-20240518/utils/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:44:54.000000 artifacts-20240518/utils/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-05-13 04:39:45.000000 artifacts-20240518/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-05-13 04:39:45.000000 artifacts-20240518/utils/dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9073 2023-12-03 10:44:54.000000 artifacts-20240518/utils/pylintrc
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      802 2024-01-28 17:41:59.000000 artifacts-20240518/utils/update_release.sh
```

### Comparing `artifacts-20230928/.github/workflows/test_docker.yml` & `artifacts-20240518/.github/workflows/test_docker.yml`

 * *Files 11% similar despite different names*

```diff
@@ -3,79 +3,71 @@
 on: [push]
 permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['38']
+        version: ['39', '40']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel python3-pyyaml python3-setuptools
+        dnf install -y @development-tools python3 python3-build python3-devel python3-pyyaml python3-setuptools python3-wheel
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Build source distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
-      run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
   test_ubuntu:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['22.04']
+        version: ['24.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev python3-distutils python3-setuptools python3-yaml
+        apt-get install -y build-essential python3 python3-build python3-dev python3-pip python3-setuptools python3-wheel python3-yaml
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
         LANG: en_US.UTF-8
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Build source distribution
-      run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
```

### Comparing `artifacts-20230928/.github/workflows/test_docs.yml` & `artifacts-20240518/.github/workflows/test_docs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.11'
+        - python-version: '3.12'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -32,15 +32,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools python3-yaml
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `artifacts-20230928/.github/workflows/test_tox.yml` & `artifacts-20240518/.github/workflows/test_tox.yml`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.7'
-          toxenv: 'py37'
         - python-version: '3.8'
-          toxenv: 'py38'
+          toxenv: 'py38,wheel'
         - python-version: '3.9'
-          toxenv: 'py39'
+          toxenv: 'py39,wheel'
         - python-version: '3.10'
-          toxenv: 'py310'
+          toxenv: 'py310,wheel'
         - python-version: '3.11'
-          toxenv: 'py311'
+          toxenv: 'py311,wheel'
+        - python-version: '3.12'
+          toxenv: 'py312,wheel'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -40,34 +40,34 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools python3-yaml
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         tox -e${{ matrix.toxenv }}
   coverage:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.11'
-          toxenv: 'py311,coverage'
+        - python-version: '3.10'
+          toxenv: 'coverage'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -76,36 +76,38 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools python3-yaml
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests with coverage
       env:
         LANG: en_US.UTF-8
       run: |
         tox -e${{ matrix.toxenv }}
     - name: Upload coverage report to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
-        - python-version: '3.11'
+        - python-version: '3.12'
           toxenv: 'lint'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -114,15 +116,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git libffi-dev python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools python3-yaml
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools python3-yaml
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run linter
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `artifacts-20230928/.pylintrc` & `artifacts-20240518/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pylint 2.17.x configuration file
+# Pylint 3.0.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
 [MAIN]
 
 # Analyse import fallback blocks. This can be used to support both Python 2 and
 # 3 compatible code, which means that the block might have code that exists
@@ -81,23 +81,22 @@
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
-# load-plugins=
 load-plugins=pylint.extensions.docparams
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Minimum Python version to use for version dependent checks. Will default to
 # the version used to run pylint.
-py-version=3.11
+py-version=3.12
 
 # Discover python modules and packages in the file system subtree.
 # recursive=no
 recursive=yes
 
 # Add paths to the list of the source roots. Supports globbing patterns. The
 # source root is an absolute path or a path relative to the current working
@@ -437,14 +436,15 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once). You can also use "--disable=all" to
 # disable everything first and then re-enable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
+
 disable=assignment-from-none,
         bad-inline-option,
         consider-using-f-string,
         deprecated-pragma,
         duplicate-code,
         file-ignored,
         fixme,
@@ -464,14 +464,16 @@
         too-many-lines,
         too-many-locals,
         too-many-nested-blocks,
         too-many-public-methods,
         too-many-return-statements,
         too-many-statements,
         unsubscriptable-object,
+        use-implicit-booleaness-not-comparison-to-string,
+        use-implicit-booleaness-not-comparison-to-zero,
         useless-object-inheritance,
         useless-suppression,
         use-symbolic-message-instead
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
@@ -518,16 +520,17 @@
 # analyzed. This score is used by the global evaluation report (RP0004).
 evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
 
 # Template used to display messages. This is a python new-style format string
 # used to format the message information. See doc for all details.
 msg-template=
 
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
+# Set the output format. Available formats are: text, parseable, colorized,
+# json2 (improved json format), json (old json format) and msvs (visual
+# studio). You can also give a reporter class, e.g.
 # mypackage.mymodule.MyReporterClass.
 #output-format=
 
 # Tells whether to display a full report or only the messages.
 reports=no
 
 # Activate the evaluation score.
```

### Comparing `artifacts-20230928/LICENSE` & `artifacts-20240518/LICENSE`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/MANIFEST.in` & `artifacts-20240518/MANIFEST.in`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 include ACKNOWLEDGEMENTS AUTHORS LICENSE README
 include dependencies.ini run_tests.py utils/__init__.py utils/dependencies.py
 include utils/check_dependencies.py
 include requirements.txt test_requirements.txt
 recursive-include config *
-recursive-include data *
 recursive-include test_data *
 exclude .gitignore
 exclude *.pyc
+recursive-exclude artifacts *.pyc
 recursive-include tools *.py
 recursive-exclude tools *.pyc
-recursive-exclude artifacts *.pyc
 # The test scripts are not required in a binary distribution package they
 # are considered source distribution files and excluded in find_package()
 # in setup.py.
 recursive-include tests *.py
```

### Comparing `artifacts-20230928/PKG-INFO` & `artifacts-20240518/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: artifacts
-Version: 20230928
+Version: 20240518
 Summary: ForensicArtifacts.com Artifact Repository.
 Home-page: https://github.com/ForensicArtifacts/artifacts
 Maintainer: Forensic artifacts
 Maintainer-email: forensicartifacts@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/plain
+License-File: ACKNOWLEDGEMENTS
+License-File: AUTHORS
 License-File: LICENSE
+License-File: README
+Requires-Dist: PyYAML>=3.10
 
 A free, community-sourced, machine-readable knowledge base of forensic artifacts that the world can use both as an information source and within other tools.
```

### Comparing `artifacts-20230928/README.md` & `artifacts-20240518/README.md`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/artifacts/artifact.py` & `artifacts-20240518/artifacts/artifact.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 class ArtifactDefinition(object):
   """Artifact definition interface.
 
   Attributes:
     aliases (list[str]): aliases that identify the artifact definition.
     description (str): description.
     name (str): name that uniquely identifiers the artifact definition.
-    provides (list[str]): hints to what information the artifact definition
-        provides.
-    sources (list[str]): sources.
+    sources (list[SourceType]): sources.
     supported_os (list[str]): supported operating systems.
     urls (list[str]): URLs with more information about the artifact definition.
   """
 
   def __init__(self, name, aliases=None, description=None):
     """Initializes an artifact definition.
 
@@ -27,15 +25,14 @@
       aliases (Optional[str]): aliases that identify the artifact definition.
       description (Optional[str]): description of the artifact definition.
     """
     super(ArtifactDefinition, self).__init__()
     self.aliases = aliases or []
     self.description = description
     self.name = name
-    self.provides = []
     self.sources = []
     self.supported_os = []
     self.urls = []
 
   def AppendSource(self, type_indicator, attributes):
     """Appends a source.
 
@@ -90,12 +87,10 @@
         'doc': self.description,
         'sources': sources,
     }
     if self.aliases:
       artifact_definition['aliases'] = self.aliases
     if self.supported_os:
       artifact_definition['supported_os'] = self.supported_os
-    if self.provides:
-      artifact_definition['provides'] = self.provides
     if self.urls:
       artifact_definition['urls'] = self.urls
     return artifact_definition
```

### Comparing `artifacts-20230928/artifacts/definitions.py` & `artifacts-20240518/artifacts/definitions.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 TYPE_INDICATOR_DIRECTORY = 'DIRECTORY'  # deprecated use PATH instead.
 TYPE_INDICATOR_FILE = 'FILE'
 TYPE_INDICATOR_PATH = 'PATH'
 TYPE_INDICATOR_WINDOWS_REGISTRY_KEY = 'REGISTRY_KEY'
 TYPE_INDICATOR_WINDOWS_REGISTRY_VALUE = 'REGISTRY_VALUE'
 TYPE_INDICATOR_WMI_QUERY = 'WMI'
 
+SUPPORTED_OS_ANDROID = 'Android'
 SUPPORTED_OS_DARWIN = 'Darwin'
 SUPPORTED_OS_ESXI = 'ESXi'
+SUPPORTED_OD_IOS = 'iOS'
 SUPPORTED_OS_LINUX = 'Linux'
 SUPPORTED_OS_WINDOWS = 'Windows'
 
 SUPPORTED_OS = frozenset([
+    SUPPORTED_OS_ANDROID,
     SUPPORTED_OS_DARWIN,
     SUPPORTED_OS_ESXI,
+    SUPPORTED_OD_IOS,
     SUPPORTED_OS_LINUX,
     SUPPORTED_OS_WINDOWS])
 
 TOP_LEVEL_KEYS = frozenset([
     'aliases',
     # conditions have been deprecated as of version 20220710.
     'conditions',
     'doc',
     # labels have been deprecated as of version 20220311.
     'labels',
     'name',
+    # provides have been deprecated as of version 20240210.
     'provides',
     'sources',
     'supported_os',
     'urls'])
```

### Comparing `artifacts-20230928/artifacts/reader.py` & `artifacts-20240518/artifacts/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 class BaseArtifactsReader(object):
   """Artifacts reader interface.
 
   Attributes:
     supported_os (set[str]): supported operating systems.
   """
 
-  # Note that redundant-returns-doc and redundant-yields-doc are broken for
-  # pylint 1.7.x for abstract methods.
-  # pylint: disable=redundant-returns-doc,redundant-yields-doc
-
   def __init__(self):
     """Initializes an artifacts reader."""
     super(BaseArtifactsReader, self).__init__()
     self.supported_os = set()
 
   @abc.abstractmethod
   def ReadArtifactDefinitionValues(self, artifact_definition_values):
@@ -85,18 +81,14 @@
           or incorrect.
     """
 
 
 class ArtifactsReader(BaseArtifactsReader):
   """Artifacts reader common functionality."""
 
-  # Note that redundant-yields-doc is broken for pylint 1.7.x for
-  # abstract methods.
-  # pylint: disable=redundant-yields-doc
-
   def __init__(self):
     """Initializes an artifacts reader."""
     super(ArtifactsReader, self).__init__()
     self.supported_os = set(definitions.SUPPORTED_OS)
 
   # Pylint fails on detecting the type of definition_object based on
   # the docstring.
@@ -217,16 +209,14 @@
           f'Invalid artifact definition: {name:s} still uses collectors.')
 
     urls = artifact_definition_values.get('urls', [])
     if not isinstance(urls, list):
       raise errors.FormatError(
           f'Invalid artifact definition: {name:s} urls is not a list.')
 
-    artifact_definition.provides = artifact_definition_values.get(
-        'provides', [])
     self._ReadSupportedOS(artifact_definition_values, artifact_definition, name)
     artifact_definition.urls = urls
     self._ReadSources(artifact_definition_values, artifact_definition, name)
 
     return artifact_definition
 
   def ReadDirectory(self, path, extension='yaml'):
```

### Comparing `artifacts-20230928/artifacts/registry.py` & `artifacts-20240518/artifacts/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,18 +124,18 @@
       return None
 
     return self._artifact_definitions_by_name.get(name.lower(), None)
 
   def GetDefinitions(self):
     """Retrieves the artifact definitions.
 
-    Returns:
-      list[ArtifactDefinition]: artifact definitions.
+    Yields:
+      ArtifactDefinition: artifact definition.
     """
-    return self._artifact_definitions_by_name.values()
+    yield from self._artifact_definitions_by_name.values()
 
   def GetUndefinedArtifacts(self):
     """Retrieves the names of undefined artifacts used by artifact groups.
 
     Returns:
       set[str]: undefined artifacts names.
     """
```

### Comparing `artifacts-20230928/artifacts/source_type.py` & `artifacts-20240518/artifacts/source_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,14 @@
 from artifacts import definitions
 from artifacts import errors
 
 
 class SourceType(object):
   """Artifact definition source type interface."""
 
-  # Note that redundant-returns-doc is broken for pylint 1.7.x for
-  # abstract methods.
-  # pylint: disable=redundant-returns-doc
-
   TYPE_INDICATOR = None
 
   def __init__(self):
     """Initializes an artifact definition source type.
 
     Raises:
       FormatError: if the indicator is not defined.
```

### Comparing `artifacts-20230928/artifacts.egg-info/PKG-INFO` & `artifacts-20240518/artifacts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: artifacts
-Version: 20230928
+Version: 20240518
 Summary: ForensicArtifacts.com Artifact Repository.
 Home-page: https://github.com/ForensicArtifacts/artifacts
 Maintainer: Forensic artifacts
 Maintainer-email: forensicartifacts@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Requires-Python: >=3.8
 Description-Content-Type: text/plain
+License-File: ACKNOWLEDGEMENTS
+License-File: AUTHORS
 License-File: LICENSE
+License-File: README
+Requires-Dist: PyYAML>=3.10
 
 A free, community-sourced, machine-readable knowledge base of forensic artifacts that the world can use both as an information source and within other tools.
```

### Comparing `artifacts-20230928/artifacts.ini` & `artifacts-20240518/artifacts.ini`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/config/appveyor/install.ps1` & `artifacts-20240518/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/config/appveyor/runtests.sh` & `artifacts-20240518/config/appveyor/runtests.sh`

 * *Files 3% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 export CPPFLAGS="-I/usr/local/include -I/usr/local/opt/gettext/include ${CPPFLAGS}";
 export LDFLAGS="-L/usr/local/lib -L/usr/local/opt/gettext/lib ${LDFLAGS}";
 
 # Set the following environment variables to build pycrypto and yara-python.
 export CPPFLAGS="-I/usr/local/opt/openssl@1.1/include ${CPPFLAGS}";
 export LDFLAGS="-L/usr/local/opt/openssl@1.1/lib ${LDFLAGS}";
 
-# Set the following environment variables to ensure tox can find Python 3.11.
-export PATH="/usr/local/opt/python@3.11/bin:${PATH}";
+# Set the following environment variables to ensure tox can find Python 3.12.
+export PATH="/usr/local/opt/python@3.12/bin:${PATH}";
 
-tox -e py311
+tox -e py312
```

### Comparing `artifacts-20230928/config/dpkg/control` & `artifacts-20240518/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/config/dpkg/copyright` & `artifacts-20240518/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/antivirus.yaml` & `artifacts-20240518/artifacts/data/antivirus.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/applications.yaml` & `artifacts-20240518/artifacts/data/applications.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Application artifacts.
 ---
+name: GnomeEvolution
+doc: Gnome Evolution files.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/.cache/evolution/**'
+    - '%%users.homedir%%/.config/evolution/**'
+    - '%%users.homedir%%/.local/share/evolution/**'
+supported_os: [Linux]
+---
 name: MicrosoftOfficeAutosave
 aliases: [WindowsMsOfficeAutosave]
 doc: Automatically created Microsoft Office recovery files.
 sources:
 - type: FILE
   attributes:
     paths:
@@ -118,18 +129,7 @@
 ---
 name: MozillaThunderbird
 doc: Mozilla Thunderbird files.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/.thunderbird/**']}
 supported_os: [Linux]
----
-name: GnomeEvolution
-doc: Gnome Evolution files.
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.homedir%%/.cache/evolution/**'
-    - '%%users.homedir%%/.config/evolution/**'
-    - '%%users.homedir%%/.local/share/evolution/**'
-supported_os: [Linux]
```

### Comparing `artifacts-20230928/data/cloud_services.yaml` & `artifacts-20240518/artifacts/data/cloud_services.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/config_files.yaml` & `artifacts-20240518/artifacts/data/config_files.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/containerd.yaml` & `artifacts-20240518/artifacts/data/containerd.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/database_servers.yaml` & `artifacts-20240518/artifacts/data/database_servers.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/docker.yaml` & `artifacts-20240518/artifacts/data/docker.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/esxi.yaml` & `artifacts-20240518/artifacts/data/esxi.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/file_systems.yaml` & `artifacts-20240518/artifacts/data/file_systems.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # File system artifacts.
 ---
-name: NTFSMFTFiles
-doc: The NTFS $MFT and $MFTMirr file system metadata files.
+name: NTFSLogFile
+doc: The NTFS $LogFile file system metadata file.
 sources:
 - type: FILE
   attributes:
-    paths:
-    - '%%environ_systemdrive%%\$MFT'
-    - '%%environ_systemdrive%%\$MFTMirr'
+    paths: ['%%environ_systemdrive%%\$LogFile']
     separator: '\'
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/file_systems/NTFS.html']
 supported_os: [Windows]
 ---
-name: NTFSLogFile
-doc: The NTFS $LogFile file system metadata file.
+name: NTFSMFTFiles
+doc: The NTFS $MFT and $MFTMirr file system metadata files.
 sources:
 - type: FILE
   attributes:
-    paths: ['%%environ_systemdrive%%\$LogFile']
+    paths:
+    - '%%environ_systemdrive%%\$MFT'
+    - '%%environ_systemdrive%%\$MFTMirr'
     separator: '\'
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/file_systems/NTFS.html']
 supported_os: [Windows]
 ---
 name: NTFSUSNJournal
 doc: |
   The NTFS $UsnJnrl file system metadata file.
```

### Comparing `artifacts-20230928/data/hadoop.yaml` & `artifacts-20240518/artifacts/data/hadoop.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Hadoop artifacts
 ---
+name: HadoopAppLogs
+doc: Location where Hadoop application logs are stored
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/hadoop/logs/*'
+    - '/hadoop/logs/userlogs/application_*/container_*/*'
+    - '/**2/hadoop/logs/*'
+    - '/**2/hadoop/logs/userlogs/application_*/container_*/*'
+supported_os: [Linux]
+---
 name: HadoopAppRoot
 doc: Location where Hadoop application files are stored
 sources:
 - type: FILE
   attributes:
     paths:
     - '/hadoop/*/yarn/system/rmstore/FSRMStateRoot/RMAppRoot/application_*/application_*'
@@ -19,19 +31,7 @@
   attributes:
     paths:
     - '/hadoop/yarn/timeline/leveldb-timeline-store.ldb/*'
     - '/hadoop/*/yarn/timeline/leveldb-timeline-store.ldb/*'
     - '/**2/hadoop/yarn/timeline/leveldb-timeline-store.ldb/*'
     - '/**2/hadoop/*/yarn/timeline/leveldb-timeline-store.ldb/*'
 supported_os: [Linux]
----
-name: HadoopAppLogs
-doc: Location where Hadoop application logs are stored
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '/hadoop/logs/*'
-    - '/hadoop/logs/userlogs/application_*/container_*/*'
-    - '/**2/hadoop/logs/*'
-    - '/**2/hadoop/logs/userlogs/application_*/container_*/*'
-supported_os: [Linux]
```

### Comparing `artifacts-20230928/data/ics.yaml` & `artifacts-20240518/artifacts/data/ics.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/installed_module_paths.yaml` & `artifacts-20240518/artifacts/data/installed_module_paths.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/installed_modules.yaml` & `artifacts-20240518/artifacts/data/installed_modules.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/instant_messaging.yaml` & `artifacts-20240518/artifacts/data/instant_messaging.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Instant Messaging applications specific artifacts.
 ---
+name: SignalApplicationContent
+doc: Signal Application Content and Configuration
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/.var/app/org.signal.Signal/*/attachments.noindex/*'
+    - '%%users.homedir%%/.var/app/org.signal.Signal/*/Cache/*'
+    - '%%users.homedir%%/.var/app/org.signal.Signal/*/logs/*'
+    - '%%users.homedir%%/.var/app/org.signal.Signal/config.json'
+  supported_os: [Linux]
+supported_os: [Linux]
+---
+name: SignalDatabase
+doc: Signal Database file.
+sources:
+- type: FILE
+  attributes: {paths: ['%%users.homedir%%/.var/app/org.signal.Signal/db.sqlite']}
+  supported_os: [Linux]
+supported_os: [Linux]
+---
 name: SkypeChatSync
 doc: Chat Sync Directory
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.homedir%%/Library/Application Support/Skype/*/chatsync/*']
   supported_os: [Darwin]
@@ -45,35 +66,14 @@
 - type: FILE
   attributes:
     paths: ['%%users.homedir%%/Library/Application Support/Skype/*/*']
   supported_os: [Darwin]
 supported_os: [Darwin]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#skype']
 ---
-name: SignalApplicationContent
-doc: Signal Application Content and Configuration
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.homedir%%/.var/app/org.signal.Signal/*/attachments.noindex/*'
-    - '%%users.homedir%%/.var/app/org.signal.Signal/*/Cache/*'
-    - '%%users.homedir%%/.var/app/org.signal.Signal/*/logs/*'
-    - '%%users.homedir%%/.var/app/org.signal.Signal/config.json'
-  supported_os: [Linux]
-supported_os: [Linux]
----
-name: SignalDatabase
-doc: Signal Database file.
-sources:
-- type: FILE
-  attributes: {paths: ['%%users.homedir%%/.var/app/org.signal.Signal/db.sqlite']}
-  supported_os: [Linux]
-supported_os: [Linux]
----
 name: XChatLogs
 doc: XChat Log Files
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/.xchat2/xchatlogs/*.log'
```

### Comparing `artifacts-20230928/data/java.yaml` & `artifacts-20240518/artifacts/data/java.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/kaspersky_careto.yaml` & `artifacts-20240518/artifacts/data/kaspersky_careto.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/kubernetes.yaml` & `artifacts-20240518/artifacts/data/kubernetes.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 # Kubernetes artifacts
 ---
-name: KubernetesLogs
-doc: Log files that contain information about the Kubernetes installation of a node.
-sources:
-- type: FILE
-  attributes: {paths: ['/var/log/syslog*']}
-supported_os: [Linux]
----
 name: KubernetesCertificates
 doc: |
   Certificate files that are used for a Kubernetes cluster.
 
   The files are typically only present on the control-plane node.
 sources:
 - type: FILE
@@ -144,7 +137,14 @@
 sources:
 - type: FILE
   attributes: {paths: ['/var/log/pods/*/*/*.log']}
 supported_os: [Linux]
 urls:
 - 'https://github.com/kubernetes/kubernetes/pull/74441'
 - 'https://kubernetes.io/docs/concepts/cluster-administration/logging/'
+---
+name: KubernetesLogs
+doc: Log files that contain information about the Kubernetes installation of a node.
+sources:
+- type: FILE
+  attributes: {paths: ['/var/log/syslog*']}
+supported_os: [Linux]
```

### Comparing `artifacts-20230928/data/legacy.yaml` & `artifacts-20240518/artifacts/data/legacy.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 # https://github.com/google/grr/blob/master/grr/parsers/windows_registry_parser.py
 ---
 name: AllUsersAppDataEnvironmentVariable
 doc: The %ProgramData% environment variable.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList', value: 'ProgramData'}]}
-provides: [environ_allusersappdata]
 supported_os: [Windows]
 urls: ['http://environmentvariables.org/ProgramData']
 ---
 name: AllUsersProfileEnvironmentVariable
 doc: The %AllUsersProfile% environment variable.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
     - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList\ProfilesDirectory'
     - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList\AllUsersProfile'
-provides: [environ_allusersprofile]
 supported_os: [Windows]
 urls: ['http://support.microsoft.com/kb//214653']
 ---
 name: LinuxRelease
 doc: |
   Linux specific distribution information.
 
@@ -36,43 +34,39 @@
   attributes:
     paths:
     - '/etc/enterprise-release'
     - '/etc/lsb-release'
     - '/etc/oracle-release'
     - '/etc/redhat-release'
     - '/etc/system-release'
-provides: [os_release, os_major_version, os_minor_version]
 supported_os: [Linux]
 ---
 name: SystemDriveEnvironmentVariable
 doc: |
   The %SystemDrive% environment variable, usually "C:".
 
   This value isn't actually present in the Registry but with some parsing we
   can figure it out from SystemRoot.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion', value: 'SystemRoot'}]}
-provides: [environ_systemdrive]
 supported_os: [Windows]
 urls:
 - 'http://environmentvariables.org/SystemDrive'
 - 'https://msdn.microsoft.com/en-us/library/cc231436.aspx'
 ---
 name: WinDomainName
 doc: The Windows domain the system is connected to.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\Tcpip\Parameters', value: 'Domain'}]}
-provides: [domain]
 supported_os: [Windows]
 ---
 name: WindowsEnvironmentVariableAllUsersAppData
 doc: The %ProgramData% environment variable.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList', value: 'ProgramData'}
-provides: [environ_allusersappdata]
 supported_os: [Windows]
 urls: ['http://environmentvariables.org/ProgramData']
```

### Comparing `artifacts-20230928/data/linux.yaml` & `artifacts-20240518/artifacts/data/linux.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 supported_os: [Linux]
 ---
 name: DebianVersion
 doc: Debian version information.
 sources:
 - type: FILE
   attributes: {paths: ['/etc/debian_version']}
-provides: [os_release, os_major_version, os_minor_version]
 supported_os: [Linux]
 ---
 name: DNSResolvConfFile
 doc: DNS Resolver configuration file.
 sources:
 - type: FILE
   attributes: {paths: ['/etc/resolv.conf']}
@@ -211,15 +210,15 @@
 ---
 name: LinuxAuthLogs
 doc: Linux authentication log files.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '/var/log/auth.log*'
+    - '/var/log/auth*'
     - '/var/log/secure*'
 supported_os: [Linux]
 ---
 name: LinuxCACertificatesConfiguration
 doc: Linux CA Certificates configuration file.
 sources:
 - type: FILE
@@ -256,15 +255,15 @@
     - '/var/spool/cron/**'
 supported_os: [Linux]
 ---
 name: LinuxDaemonLogFiles
 doc: Linux daemon log files.
 sources:
 - type: FILE
-  attributes: {paths: ['/var/log/daemon.log*']}
+  attributes: {paths: ['/var/log/daemon*']}
 supported_os: [Linux]
 ---
 name: LinuxDHCPConfigurationFile
 doc: Linux DHCP Configuration File
 sources:
 - type: FILE
   attributes:
@@ -281,15 +280,14 @@
     - '/etc/centos-release'
     - '/etc/enterprise-release'
     - '/etc/oracle-release'
     - '/etc/redhat-release'
     - '/etc/rocky-release'
     - '/etc/SuSE-release'
     - '/etc/system-release'
-provides: [os_release, os_major_version, os_minor_version]
 supported_os: [Linux]
 ---
 name: LinuxDSDTTable
 doc: Linux file containing DSDT table.
 sources:
 - type: FILE
   attributes: {paths: ['/sys/firmware/acpi/tables/DSDT']}
@@ -364,15 +362,15 @@
 supported_os: [Linux]
 urls: ['https://web.mit.edu/kerberos/krb5-1.12/doc/admin/conf_files/krb5_conf.html']
 ---
 name: LinuxKernelLogFiles
 doc: Linux kernel log files.
 sources:
 - type: FILE
-  attributes: {paths: ['/var/log/kern.log*']}
+  attributes: {paths: ['/var/log/kern*']}
 supported_os: [Linux]
 ---
 name: LinuxLastlogFile
 doc: Linux lastlog file.
 sources:
 - type: FILE
   attributes: {paths: ['/var/log/lastlog']}
@@ -406,15 +404,14 @@
 supported_os: [Linux]
 ---
 name: LinuxLSBRelease
 doc: Linux Standard Base (LSB) release information
 sources:
 - type: FILE
   attributes: {paths: ['/etc/lsb-release']}
-provides: [os_release, os_major_version, os_minor_version]
 supported_os: [Linux]
 urls: ['https://linux.die.net/man/1/lsb_release']
 ---
 name: LinuxMessagesLogFiles
 doc: Linux messages log files.
 sources:
 - type: FILE
@@ -454,14 +451,22 @@
     - '/var/lib/NetworkManager/NetworkManager-intern.conf'
     - '/var/lib/NetworkManager/*'
 supported_os: [Linux]
 urls:
 - 'https://linux.die.net/man/5/networkmanager.conf'
 - 'https://man.archlinux.org/man/NetworkManager.conf.5.en#FILE_FORMAT'
 ---
+name: LinuxNssCachePasswdFile
+doc: Local NSS database for remote directory services.
+sources:
+- type: FILE
+  attributes: {paths: ['/etc/passwd.cache']}
+supported_os: [Linux]
+urls: ['https://github.com/google/nsscache']
+---
 name: LinuxPamConfigs
 doc: Configuration files for PAM.
 sources:
 - type: FILE
   attributes:
     paths:
     - '/etc/pam.conf'
@@ -487,15 +492,14 @@
 sources:
 - type: ARTIFACT_GROUP
   attributes:
     names:
     - LinuxDistributionRelease
     - LinuxLSBRelease
     - LinuxSystemdOSRelease
-provides: [os_release, os_major_version, os_minor_version]
 supported_os: [Linux]
 ---
 name: LinuxRsyslogConfigs
 doc: Linux rsyslog configurations.
 sources:
 - type: FILE
   attributes:
@@ -601,15 +605,14 @@
 doc: Linux systemd /etc/os-release file
 sources:
 - type: FILE
   attributes:
     paths:
     - '/etc/os-release'
     - '/usr/lib/os-release'
-provides: [os_release, os_major_version, os_minor_version]
 supported_os: [Linux]
 urls: ['https://www.freedesktop.org/software/systemd/man/os-release.html']
 ---
 name: LinuxSystemdServices
 doc: Linux systemd service unit files
 sources:
 - type: FILE
@@ -713,26 +716,25 @@
 ---
 name: LinuxUtmpFiles
 doc: Linux btmp, utmp and wtmp login record files.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '/var/log/btmp'
-    - '/var/log/wtmp'
-    - '/var/run/utmp'
+    - '/var/log/btmp*'
+    - '/var/log/wtmp*'
+    - '/var/run/utmp*'
 supported_os: [Linux]
 urls: ['https://github.com/libyal/dtformats/blob/main/documentation/Utmp%20login%20records%20format.asciidoc']
 ---
 name: LinuxWtmp
 doc: Linux wtmp login record file
 sources:
 - type: FILE
-  attributes: {paths: ['/var/log/wtmp']}
-provides: [users.username, users.last_logon]
+  attributes: {paths: ['/var/log/wtmp*']}
 supported_os: [Linux]
 urls: ['https://github.com/libyal/dtformats/blob/main/documentation/Utmp%20login%20records%20format.asciidoc']
 ---
 name: LinuxXinetd
 doc: Linux xinetd configurations.
 sources:
 - type: FILE
@@ -791,14 +793,16 @@
 ---
 name: MySQLHistoryFile
 doc: MySQL History file.
 sources:
 - type: FILE
   attributes:
     paths:
+    - '/.mysql_history'
+    - '/root/.mysql_history'
     - '%%users.homedir%%/.mysql_history'
 supported_os: [Linux]
 ---
 name: NanoHistoryFile
 doc: nano history file that logs search and replace strings.
 sources:
 - type: FILE
@@ -807,15 +811,14 @@
 urls: ['https://www.nano-editor.org/dist/v2.2/nano.html']
 ---
 name: NetgroupConfiguration
 doc: Linux netgroup configuration.
 sources:
 - type: FILE
   attributes: {paths: ['/etc/netgroup']}
-provides: [users.username]
 supported_os: [Linux]
 ---
 name: NtpConfFile
 doc: The configuration file for ntpd. e.g. ntp.conf.
 sources:
 - type: FILE
   attributes: {paths: ['/etc/ntp.conf']}
@@ -840,14 +843,16 @@
 ---
 name: PostgreSQLHistoryFile
 doc: PostgreSQL History file.
 sources:
 - type: FILE
   attributes:
     paths:
+    - '/.psql_history'
+    - '/root/.psql_history'
     - '/var/lib/postgresql/.psql_history'
     - '/var/lib/pgsql/.psql_history'
     - '%%users.homedir%%/.psql_history'
 supported_os: [Linux]
 ---
 name: PythonHistoryFile
 doc: Python REPL history file.
```

### Comparing `artifacts-20230928/data/linux_proc.yaml` & `artifacts-20240518/artifacts/data/linux_proc.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/linux_services.yaml` & `artifacts-20240518/artifacts/data/linux_services.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/macos.yaml` & `artifacts-20240518/artifacts/data/macos.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,75 @@
 - type: FILE
   attributes:
     paths:
     - '/Applications/Xcode.app/Contents/Developer/Platforms/*.platform/Developer/Library/CoreSimulator/Profiles/Runtimes/*.simruntime/Contents/Resources/SampleContent/Library/AddressBook/AddressBookImages.sqlitedb'
     - '%%users.homedir%%/Library/Developer/CoreSimulator/Devices/*/data/Library/AddressBook/AddressBookImages.sqlitedb'
 supported_os: [Darwin]
 ---
+name: MacOSAirportPreferencesPlistFile
+aliases: [MacOSWirelessNetworks]
+doc: Airport (wireless networking) preferences property list (plist) file.
+sources:
+- type: FILE
+  attributes: {paths: ['/Library/Preferences/SystemConfiguration/com.apple.airport.preferences.plist']}
+supported_os: [Darwin]
+urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/macos/NetworkSettings.html']
+---
 name: MacOSApplePushServiceSQLiteDatabaseFile
 doc: Apple push service SQLite database file.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Application Support/ApplePushService/aps.db']}
 supported_os: [Darwin]
 ---
+name: MacOSAppleSetupDoneFile
+aliases: [MacOSSystemInstallationTime]
+doc: Mac OS .AppleSetupDone file that hints to the system installation date and time.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/private/var/db/.AppleSetupDone'
+    - '/var/db/.AppleSetupDone'
+supported_os: [Darwin]
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-settings-and-informations']
+---
+name: MacOSAppleSystemLogFile
+aliases: [MacOSAppleSystemLogFiles]
+doc: Apple system log (ASL) files.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/private/var/log/asl/*.asl'
+    - '/private/var/log/DiagnosticMessages/*.asl'
+    - '/var/log/asl/*.asl'
+    - '/var/log/DiagnosticMessages/*.asl'
+supported_os: [Darwin]
+urls:
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs'
+- 'https://support.apple.com/guide/console/reports-cnsl664be99a/mac'
+---
 name: MacOSApplicationBundleCacheSQLiteDatabaseFile
 doc: Application bundle cache SQLite database file.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Caches/*/Cache.db']}
 supported_os: [Darwin]
 ---
+name: MacOSApplicationResourcesStringsPlistFile
+doc: Application resources strings plist file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/Applications/*.app/Contents/Resources/*.lproj/*.strings'
+    - '/Applications/*/*.app/Contents/Resources/*.lproj/*.strings'
+supported_os: [Darwin]
+---
 name: MacOSAssetCacheInfoSQLiteDatabaseFile
 doc: Asset cache information SQLite database file.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Caches/com.apple.AssetCache/AssetInfo.db']}
 supported_os: [Darwin]
 ---
@@ -54,51 +101,14 @@
 name: MacOSCallHistoryCacheSQLiteDatabaseFile
 doc: Call history cache SQLite database file.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/CallHistoryDB/CallHistory.storedata']}
 supported_os: [Darwin]
 ---
-name: MacOSAirportPreferencesPlistFile
-aliases: [MacOSWirelessNetworks]
-doc: Airport (wireless networking) preferences property list (plist) file.
-sources:
-- type: FILE
-  attributes: {paths: ['/Library/Preferences/SystemConfiguration/com.apple.airport.preferences.plist']}
-supported_os: [Darwin]
-urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/macos/NetworkSettings.html']
----
-name: MacOSAppleSetupDoneFile
-aliases: [MacOSSystemInstallationTime]
-doc: Mac OS .AppleSetupDone file that hints to the system installation date and time.
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '/private/var/db/.AppleSetupDone'
-    - '/var/db/.AppleSetupDone'
-supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-settings-and-informations']
----
-name: MacOSAppleSystemLogFile
-aliases: [MacOSAppleSystemLogFiles]
-doc: Apple system log (ASL) files.
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '/private/var/log/asl/*.asl'
-    - '/private/var/log/DiagnosticMessages/*.asl'
-    - '/var/log/asl/*.asl'
-    - '/var/log/DiagnosticMessages/*.asl'
-supported_os: [Darwin]
-urls:
-- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs'
-- 'https://support.apple.com/guide/console/reports-cnsl664be99a/mac'
----
 name: MacOSApplicationsDirectory
 aliases: [MacOSApplications]
 doc: Contents of the Applications directory.
 sources:
 - type: PATH
   attributes: {paths: ['/Applications/*']}
 supported_os: [Darwin]
@@ -140,14 +150,74 @@
 doc: Bluetooth preferences and paired device information property list (plist) file
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.Bluetooth.plist']}
 supported_os: [Darwin]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
 ---
+name: MacOSCodeSignatureCodeResourcesPlistFile
+doc: Code signature CodeResources plist file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/Applications/Utilities/*.app/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/CoreServices/*.app/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Extensions/*.kext/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/PlugIns/*.plugin/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/Resources/*.bundle/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Extensions/*.kext/Contents/Resources/*.bundle/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Filesystems/*/*.kext/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/Filesystems/*/Encodings/*.kext/Contents/_CodeSignature/CodeResources'
+    - '/System/Library/PrivateFrameworks/*.framework/Versions/A/Resources/*.kext/Contents/_CodeSignature/CodeResources'
+supported_os: [Darwin]
+---
+name: MacOSContentsInfoPlistFile
+doc: Contents Info.plist file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/Applications/*/*.app/Contents/Info.plist'
+    - '/Applications/*/*.app/Contents/Resources/*.help/Contents/Info.plist'
+    - '/System/Library/CoreServices/*.app/Contents/Info.plist'
+    - '/System/Library/Extensions/*.kext/Contents/Info.plist'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/Info.plist'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/PlugIns/*.plugin/Contents/Info.plist'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/Resources/*.bundle/Contents/Info.plist'
+    - '/System/Library/Extensions/*.kext/Contents/Resources/*.bundle/Contents/Info.plist'
+    - '/System/Library/Extensions/*.kext/PlugIns/*.kext/Info.plist'
+    - '/System/Library/Filesystems/*/*.kext/Contents/Info.plist'
+    - '/System/Library/Filesystems/*/Encodings/*.kext/Contents/Info.plist'
+    - '/System/Library/Frameworks/*.framework/Versions/A/Resources/Info.plist'
+    - '/System/Library/PrivateFrameworks/*.framework/Versions/A/Resources/*.kext/Contents/Info.plist'
+supported_os: [Darwin]
+---
+name: MacOSContentsVersionPlistFile
+doc: Contents version.plist file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/Applications/*/*.app/Contents/version.plist'
+    - '/Applications/*/*.app/Contents/Resources/*.help/Contents/version.plist'
+    - '/System/Library/CoreServices/*.app/Contents/version.plist'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/version.plist'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/PlugIns/*.plugin/Contents/version.plist'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/Resources/*.bundle/Contents/version.plist'
+    - '/System/Library/Extensions/*.kext/Contents/Resources/*.bundle/Contents/version.plist'
+    - '/System/Library/Extensions/*.kext/Contents/version.plist'
+    - '/System/Library/Extensions/*.kext/PlugIns/*.kext/version.plist'
+    - '/System/Library/Filesystems/*/*.kext/Contents/version.plist'
+    - '/System/Library/Filesystems/*/Encodings/*.kext/Contents/version.plist'
+    - '/System/Library/Frameworks/*.framework/Versions/A/Resources/version.plist'
+    - '/System/Library/PrivateFrameworks/*.framework/Versions/A/Resources/*.kext/Contents/version.plist'
+supported_os: [Darwin]
+---
 name: MacOSCoreAnalyticsFile
 aliases: [MacOSCoreAnalyticsFiles]
 doc: CoreAnalytics log files.
 sources:
 - type: FILE
   attributes:
     paths:
@@ -322,14 +392,21 @@
   attributes:
     paths:
     - '/private/var/log/install.log'
     - '/var/log/install.log'
 supported_os: [Darwin]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-logs']
 ---
+name: MacOSiTunesInterfaceBuilderDocumentPlistFile
+doc: iTunes Interface Builder document (*.itxib) plist file.
+sources:
+- type: FILE
+  attributes: {paths: ['/Applications/iTunes.app/Contents/Resources/*.lproj/*.itxib']}
+supported_os: [Darwin]
+---
 name: MacOSiOSBackupInfo
 doc: iOS device backup information
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Application Support/MobileSync/Backup/*/info.plist']}
 supported_os: [Darwin]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#idevice-backup']
@@ -439,17 +516,27 @@
 supported_os: [Darwin]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#logs']
 ---
 name: MacOSLoginWindowPlistFile
 doc: Log-in window information property list (plist) file
 sources:
 - type: FILE
-  attributes: {paths: ['/Library/Preferences/com.apple.loginwindow.plist']}
+  attributes:
+    paths:
+    - '/Library/Preferences/com.apple.loginwindow.plist'
+    - '%%users.homedir%%/Library/Preferences/loginwindow.plist'
+    - '%%users.homedir%%/Library/Preferences/ByHost/com.apple.loginwindow.plist'
+    - '%%users.homedir%%/Library/Preferences/ByHost/com.apple.loginwindow.*.plist'
+    - '/var/root/Library/Preferences/com.apple.loginwindow.plist'
+    - '/private/var/root/Library/Preferences/com.apple.loginwindow.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences']
+urls:
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#system-preferences'
+- 'https://taomm.org/PDFs/vol1/CH%200x02%20Persistence.pdf'
+- 'https://developer.apple.com/documentation/devicemanagement/loginwindowscripts'
 ---
 name: MacOSMailAccounts
 doc: Mail Accounts. Until now only V2, V3 and V5 have been observed.
 sources:
 - type: FILE
   attributes: {paths: ['%%users.homedir%%/Library/Mail/V[0-9]/MailData/Accounts.plist']}
 supported_os: [Darwin]
@@ -673,14 +760,48 @@
     - '/var/db/RemoteManagement/caches/UserAcct.tmp'
 supported_os: [Darwin]
 urls:
 - 'https://help.apple.com/remotedesktop/mac/3.9/'
 - 'https://www.fireeye.com/blog/threat-research/2019/10/leveraging-apple-remote-desktop-for-good-and-evil.html'
 - 'https://github.com/fireeye/ARDvark#ard-artifacts-to-parse'
 ---
+name: MacOSResourcesInfoStringsPlistFile
+doc: Resources InfoPlist.strings plist file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/Applications/*.app/Contents/Resources/*.help/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/Applications/*/*.app/Contents/Resources/*.help/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/CoreServices/*.app/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.bundle/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/Resources/*.bundle/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/Extensions/*.kext/Contents/Resources/InfoPlist.strings'
+    - '/System/Library/Extensions/*.kext/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/Filesystems/*/*.kext/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/Filesystems/*/Encodings/*.kext/Contents/Resources/*.lproj/InfoPlist.strings'
+    - '/System/Library/PrivateFrameworks/*.framework/Versions/A/Resources/*.kext/Contents/Resources/*.lproj/InfoPlist.strings'
+supported_os: [Darwin]
+---
+name: MacOSResourcesLocalizableStringsPlistFile
+doc: Resources Localizable.strings plist file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/System/Library/CoreServices/*.app/Contents/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/Extensions/*.kext/Contents/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/Extensions/*.kext/Contents/PlugIns/*.kext/Contents/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/Frameworks/*.framework/Versions/A/Frameworks/*.framework/Versions/A/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/PreferencePanes/*.prefPane/Contents/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/PrivateFrameworks/*.framework/Versions/A/Plugins/*.bundle/Contents/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/PrivateFrameworks/*.framework/Versions/A/Resources/*.lproj/Localizable.strings'
+    - '/System/Library/SystemProfiler/*/Contents/Resources/*.lproj/Localizable.strings'
+supported_os: [Darwin]
+---
 name: MacOSSidebarListsPlistFile
 aliases: [MacOSSidebarLists]
 doc: |
   Sidebar lists preferences property list (plist) file.
 
   This property list contains the names of volumes mounted on the desktop that have appeared in the sidebar list.
 sources:
@@ -745,25 +866,41 @@
 doc: Software update preferences property list (plist) files.
 sources:
 - type: FILE
   attributes: {paths: ['/Library/Preferences/com.apple.SoftwareUpdate.plist']}
 supported_os: [Darwin]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#software-installation']
 ---
+name: MacOSSpotlightStoreVolumeConfigurationPlistFile
+doc: Spotlight store volume configuration plist file.
+sources:
+- type: FILE
+  attributes: {paths: ['/.Spotlight-V100/Store-V1/VolumeConfig.plist']}
+supported_os: [Darwin]
+---
+name: MacOSSpotlightVolumeConfigurationPlistFile
+doc: Spotlight volume configuration plist file.
+sources:
+- type: FILE
+  attributes: {paths: ['/.Spotlight-V100/VolumeConfiguration.plist']}
+supported_os: [Darwin]
+---
 name: MacOSStartupItemsPlistFile
 aliases: [MacOSStartupItemsPlistFiles]
 doc: Startup Items property list (plist) files.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '/Library/StartupItems/*.plist'
-    - '/System/Library/StartupItems/*.plist'
+    - '/Library/StartupItems/**/*.plist'
+    - '/System/Library/StartupItems/**/*.plist'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations']
+urls:
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations'
+- 'https://developer.apple.com/library/archive/documentation/MacOSX/Conceptual/BPSystemStartup/Chapters/StartupItems.html'
 ---
 name: MacOSSwapFile
 aliases: [MacOSSwapFiles]
 doc: Swap file
 sources:
 - type: FILE
   attributes:
@@ -950,17 +1087,24 @@
 supported_os: [Darwin]
 ---
 name: MacOSUserLoginItemsPlistFile
 aliases: [MacOSUserLoginItems]
 doc: User login items property list (plist) file.
 sources:
 - type: FILE
-  attributes: {paths: ['%%users.homedir%%/Library/Preferences/com.apple.loginitems.plist']}
+  attributes:
+    paths:
+    - '%%users.homedir%%/Library/Preferences/com.apple.loginitems.plist'
+    - '%%users.homedir%%/Library/Application Support/com.apple.backgroundtaskmanagementagent/backgrounditems.btm'
+    - '/private/var/db/com.apple.backgroundtaskmanagement/BackgroundItems-v*.btm'
+    - '/var/db/com.apple.backgroundtaskmanagement/BackgroundItems-v*.btm'
 supported_os: [Darwin]
-urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations-2']
+urls:
+- 'https://forensics.wiki/mac_os_x_10.9_artifacts_location#autorun-locations-2'
+- 'https://objective-see.org/blog/blog_0x31.html'
 ---
 name: MacOSUserMoviesDirectory
 doc: Contents of the user Movies directories.
 sources:
 - type: PATH
   attributes: {paths: ['%%users.homedir%%/Movies/*']}
 supported_os: [Darwin]
```

### Comparing `artifacts-20230928/data/shell.yaml` & `artifacts-20240518/artifacts/data/shell.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/tomcat.yaml` & `artifacts-20240518/artifacts/data/tomcat.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/triage.yaml` & `artifacts-20240518/artifacts/data/triage.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
   attributes:
     names:
     - MicrosoftOfficeAutosave
     - MicrosoftOfficeMRU
     - WindowsActivitiesCacheDatabase
     - WindowsRDPClientBitmapCache
     - WindowsRecycleBinMetadata
-    - WindowsSearchDatabase
+    - WindowsSearchDatabaseFile
     - WindowsUserAutomaticDestinationsJumpLists
     - WindowsUserCustomDestinationsJumpLists
     - WindowsUserRecentFiles
   supported_os: [Windows]
 supported_os: [Linux, Windows]
 ---
 name: TriageNetwork
```

### Comparing `artifacts-20230928/data/unix_common.yaml` & `artifacts-20240518/artifacts/data/unix_common.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Artifacts common to Unix-based operating systems.
 ---
+name: CupsJobCacheFile
+aliases: [MacOSCupsJobCacheFile]
+doc: Common UNIX Printing System (CUPS) job cache file.
+sources:
+- type: FILE
+  attributes: {paths: ['/var/spool/cups/cache/job.cache']}
+  supported_os: [Darwin]
+- type: FILE
+  attributes: {paths: ['/private/var/spool/cups/cache/job.cache']}
+  supported_os: [Darwin]
+- type: FILE
+  attributes: {paths:['/var/cache/cups/job.cache']}
+  supported_os: [Linux]
+supported_os: [Darwin, Linux]
+urls:
+- 'https://www.cups.org/doc/man-cups-files.conf.html'
+- 'https://www.cups.org/doc/spec-design.html'
+---
 name: UnixGroupsFile
 aliases: [UnixGroups]
 doc: Unix groups file.
 sources:
 - type: FILE
   attributes: {paths: ['/etc/group']}
   supported_os: [Darwin, Linux]
```

### Comparing `artifacts-20230928/data/user.yaml` & `artifacts-20240518/artifacts/data/user.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,9 @@
 # Operating system independent user artifact definitions.
 ---
-name: UsersDirectory
-aliases: [MacOSUsers, MacOSUsersDirectory, OSXUsers, UserHomeDirectory]
-doc: Contents of the Users directory.
-sources:
-- type: PATH
-  attributes: {paths: ['/Users/*']}
-supported_os: [Darwin]
-provides: [users.username]
-urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#users']
----
 name: UserDownloadsDirectory
 aliases: [MacOSUserDownloadsDirectory, UserDownloads, WindowsUserDownloadsDirectory]
 doc: Contents of user Downloads directories.
 sources:
 - type: PATH
   attributes:
     paths: ['%%users.homedir%%/Downloads/*']
@@ -21,7 +11,16 @@
 - type: PATH
   attributes:
     paths: ['%%users.userprofile%%\Downloads\*']
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#user-directories']
+---
+name: UsersDirectory
+aliases: [MacOSUsers, MacOSUsersDirectory, OSXUsers, UserHomeDirectory]
+doc: Contents of the Users directory.
+sources:
+- type: PATH
+  attributes: {paths: ['/Users/*']}
+supported_os: [Darwin, Windows]
+urls: ['https://forensics.wiki/mac_os_x_10.9_artifacts_location#users']
```

### Comparing `artifacts-20230928/data/webbrowser.yaml` & `artifacts-20240518/artifacts/data/webbrowser.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,166 @@
 ---
 name: BrowserCache
 doc: Web browser cache of multiple web browsers.
 sources:
 - type: ARTIFACT_GROUP
   attributes:
     names:
-    - 'ChromeCache'
+    - 'ChromiumBasedBrowsersCache'
     - 'FirefoxCache'
     - 'InternetExplorerCache'
     - 'SafariCacheSQLiteDatabaseFile'
 supported_os: [Darwin, Linux, Windows]
 ---
 name: BrowserHistory
 doc: Web browser history of multiple web browsers.
 sources:
 - type: ARTIFACT_GROUP
   attributes:
     names:
-    - 'ChromiumBasedBrowsersHistory'
+    - 'ChromiumBasedBrowsersHistoryDatabaseFile'
     - 'FirefoxHistory'
     - 'FirefoxDownloads'
     - 'InternetExplorerHistory'
     - 'OperaHistoryFile'
     - 'SafariDownloadsPlistFile'
     - 'SafariHistorySQLiteDatabaseFile'
     - 'SafariHistoryPlistFile'
 supported_os: [Darwin, Linux, Windows]
 ---
+name: ChromeExtensionRegistryKeys
+doc: Chrome extensions installed by writing windows registry keys.
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys:
+    - 'HKEY_LOCAL_MACHINE\Software\Google\Chrome\Extensions\**5'
+    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Google\Chrome\Extensions\**5'
+supported_os: [Windows]
+urls: ['https://developer.chrome.com/extensions/external_extensions#registry']
+---
+name: ChromeFileSystem
+doc: |
+  Google Chrome, Beta, Canary and Chromium File System files.
+
+  The File System directory backs Chrome's fileSystem API. Inside this
+  directory are a mixture of the data files saved using the fileSystem
+  API and LevelDB directories that track the logical structure of the
+  virtual file system.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.localappdata%%\Chromium\User Data\*\File System\**5'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\File System\**5'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\File System\**5'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\File System\**5'
+    separator: '\'
+  supported_os: [Windows]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/.config/google-chrome/*/File System/**5'
+    - '%%users.homedir%%/.config/chromium/*/File System/**5'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/File System/**5'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/File System/**5'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/File System/**5'
+  supported_os: [Linux]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/File System/**5'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/File System/**5'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/File System/**5'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/File System/**5'
+  supported_os: [Darwin]
+supported_os: [Darwin, Linux, Windows]
+urls:
+- 'https://developer.chrome.com/apps/fileSystem'
+- 'https://developer.mozilla.org/en-US/docs/Web/API/FileSystem'
+- 'https://dfir.blog/deciphering-browser-hieroglyphics-leveldb-filesystem/'
+---
+name: ChromeIndexedDB
+doc: |
+  Google Chrome, Beta, Canary and Chromium IndexedDB files.
+
+  The IndexedDB directory contains one directory per origin that uses
+  IndexedDB, named like https_www.example.com_0.indexeddb.leveldb,
+  chrome-extension_app-id-xxx_0.indexeddb.leveldb, or
+  https_www.example.com_0.indexeddb.blob. Inside each of the *.leveldb
+  directories are the files the comprise a LevelDB database, which in turn
+  holds IndexedDB data for that origin. There may be an accompanying .blob
+  directory, which contains a nested folder structure of blobs.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.localappdata%%\Chromium\User Data\*\IndexedDB\**5'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\IndexedDB\**5'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\IndexedDB\**5'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\IndexedDB\**5'
+    separator: '\'
+  supported_os: [Windows]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/.config/google-chrome/*/IndexedDB/**5'
+    - '%%users.homedir%%/.config/chromium/*/IndexedDB/**5'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/IndexedDB/**5'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/IndexedDB/**5'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/IndexedDB/**5'
+  supported_os: [Linux]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/IndexedDB/**5'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/IndexedDB/**5'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/IndexedDB/**5'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/IndexedDB/**5'
+  supported_os: [Darwin]
+supported_os: [Darwin, Linux, Windows]
+urls: ['https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API']
+---
+name: ChromeLocalStorage
+doc: |
+  Google Chrome, Beta, Canary and Chromium Local Storage files.
+
+  Chrome 60 and earlier versions used individual .sqlite files per origin for Local Storage, stored in the Local Storage directory root.
+  In Chrome 61, a leveldb directory was added inside the root Local Storage directory, and new origins saved Local Storage data in a single LevelDB there.
+
+  Existing .sqlite files are kept (not moved to leveldb), so it is possible for a single Chrome profile to use both SQLite and LevelDB for Local Storage.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Local Storage/**'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Local Storage/**'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Local Storage/**'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Local Storage/**'
+  supported_os: [Darwin]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/.config/google-chrome/*/Local Storage/**'
+    - '%%users.homedir%%/.config/chromium/*/Local Storage/**'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Local Storage/**'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Local Storage/**'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Local Storage/**'
+  supported_os: [Linux]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.localappdata%%\Chromium\User Data\*\Local Storage\**'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Local Storage\**'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Local Storage\**'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Local Storage\**'
+    separator: '\'
+  supported_os: [Windows]
+supported_os: [Darwin, Linux, Windows]
+---
 name: ChromeStorage
 doc: |
   Google Chrome, Canary and Chromium browser artifacts for Storage APIs.
 
   Includes Web Storage (sessionStorage for session-only data and
   localStorage for persistent data), IndexedDB (used for structured data),
   and FileSystem (object storage in a virtual file system).
@@ -46,126 +176,151 @@
     - 'ChromeIndexedDB'
 supported_os: [Darwin, Linux, Windows]
 urls:
 - 'https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API'
 - 'https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API'
 - 'https://developer.mozilla.org/en-US/docs/Web/API/FileSystem'
 ---
-name: ChromeCache
-aliases: [ChromiumCache, EdgeCache]
+name: ChromePlatformNotifications
+aliases: [ChromeNotifications, ChromePlatformNotificationsDatabase]
 doc: |
-  Google Chrome, Canary and Chromium browser caches.
+  Google Chrome Platform Notifications LevelDB.
 
-  Canary uses "Chrome SxS" on windows.
-
-  * Disk cache (or Cache)
-  * Media cache
-  * Application cache
-  * GPU shader cache
-  * PNaCl translation cache
+  The Platform Notifications directory contains the files that comprise a LevelDB
+  database, which in turn holds platform notification data.
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%users.homedir%%/Library/Application Support/Google/Chrome/*/Platform Notifications/*']
+  supported_os: [Darwin]
+- type: FILE
+  attributes:
+    paths: ['%%users.homedir%%/.config/google-chrome/*/Platform Notifications/*']
+  supported_os: [Linux]
+- type: FILE
+  attributes:
+    paths: ['%%users.localappdata%%\Google\Chrome\User Data\*\Platform Notifications\*']
+    separator: '\'
+  supported_os: [Windows]
+supported_os: [Darwin, Linux, Windows]
+---
+name: ChromePreferences
+doc: Chrome Preferences file.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Application Cache\Cache\*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Cache\*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Cache\Cache_Data\*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Media Cache\*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\GPUCache\*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Application Cache\Cache\*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cache\*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Cache\Cache_Data\*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Media Cache\*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\GPUCache\*'
-    - '%%users.localappdata%%\Chromium\User Data\*\Application Cache\Cache\*'
-    - '%%users.localappdata%%\Chromium\User Data\*\Cache\*'
-    - '%%users.localappdata%%\Chromium\User Data\*\Cache\Cache_Data\*'
-    - '%%users.localappdata%%\Chromium\User Data\*\Media Cache\*'
-    - '%%users.localappdata%%\Chromium\User Data\*\GPUCache\*'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cache\*'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Cache\Cache_Data\*'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\GPUCache\*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Preferences'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Secure Preferences'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Preferences'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Secure Preferences'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Preferences'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Secure Preferences'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Preferences'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Secure Preferences'
+  supported_os: [Darwin]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Preferences'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Secure Preferences'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Preferences'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Secure Preferences'
+    - '%%users.homedir%%/.config/chromium/*/Preferences'
+    - '%%users.homedir%%/.config/chromium/*/Secure Preferences'
+    - '%%users.homedir%%/.config/google-chrome/*/Preferences'
+    - '%%users.homedir%%/.config/google-chrome/*/Secure Preferences'
+  supported_os: [Linux]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.localappdata%%\Chromium\User Data\*\Preferences'
+    - '%%users.localappdata%%\Chromium\User Data\*\Secure Preferences'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Preferences'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Secure Preferences'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Preferences'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Secure Preferences'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Preferences'
     separator: '\'
   supported_os: [Windows]
+supported_os: [Darwin, Linux, Windows]
+urls: ['https://forensics.wiki/google_chrome#configuration']
+---
+name: ChromeSessionStorage
+doc: |
+  Google Chrome, Beta, Canary and Chromium Sessions and Session Storage files.
+
+  The Sessions directory contains information for restoring tabs and windows
+  from a browsing session.
+
+  The Session Storage directory contains the files that comprise a LevelDB
+  database, which in turn holds the Session Storage data.
+sources:
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/Caches/Google/Chrome/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Application Cache/Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/GPUCache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome/PnaclTranslationCache/*'
-    - '%%users.homedir%%/Caches/Google/Chrome Canary/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Application Cache/Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/GPUCache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/PnaclTranslationCache/*'
-    - '%%users.homedir%%/Caches/Chromium/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Chromium/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Chromium/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Application Cache/Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/GPUCache/*'
-    - '%%users.homedir%%/Library/Caches/Chromium/PnaclTranslationCache/*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Session Storage/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Session Storage/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Session Storage/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Session Storage/*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Sessions/Session_*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Sessions/Session_*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Sessions/Session_*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Sessions/Session_*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Sessions/Tabs_*'
   supported_os: [Darwin]
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/.cache/BraveSoftware/Brave-Browser/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.cache/google-chrome/Cache/*'
-    - '%%users.homedir%%/.cache/google-chrome/*/Cache/*'
-    - '%%users.homedir%%/.cache/google-chrome/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.cache/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/google-chrome/PnaclTranslationCache/*'
-    - '%%users.homedir%%/.config/google-chrome/*/Application Cache/*'
-    - '%%users.homedir%%/.config/google-chrome/*/Cache/*'
-    - '%%users.homedir%%/.config/google-chrome/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.config/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.config/google-chrome/*/GPUCache/*'
-    - '%%users.homedir%%/.cache/chromium/Cache/*'
-    - '%%users.homedir%%/.cache/chromium/*/Cache/*'
-    - '%%users.homedir%%/.cache/chromium/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.cache/chromium/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/chromium/PnaclTranslationCache/*'
-    - '%%users.homedir%%/.config/chromium/*/Application Cache/*'
-    - '%%users.homedir%%/.config/chromium/*/Cache/*'
-    - '%%users.homedir%%/.config/chromium/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.config/chromium/*/Media Cache/*'
-    - '%%users.homedir%%/.config/chromium/*/GPUCache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/PnaclTranslationCache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/PnaclTranslationCache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Application Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/GPUCache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Application Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/GPUCache/*'
-    - '%%users.homedir%%/.cache/microsoft-edge/*/Cache/Cache_Data/*'
+    - '%%users.homedir%%/.config/google-chrome/*/Session Storage/*'
+    - '%%users.homedir%%/.config/chromium/*/Session Storage/*'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Session Storage/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Session Storage/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Session Storage/*'
+    - '%%users.homedir%%/.config/google-chrome/*/Sessions/Session_*'
+    - '%%users.homedir%%/.config/google-chrome/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/.config/chromium/*/Sessions/Session_*'
+    - '%%users.homedir%%/.config/chromium/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Sessions/Session_*'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Sessions/Session_*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Sessions/Session_*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Sessions/Tabs_*'
   supported_os: [Linux]
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.localappdata%%\Chromium\User Data\*\Session Storage\*'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Session Storage\*'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Session Storage\*'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Session Storage\*'
+    - '%%users.localappdata%%\Chromium\User Data\*\Sessions\Session_*'
+    - '%%users.localappdata%%\Chromium\User Data\*\Sessions\Tabs_*'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Sessions\Session_*'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Sessions\Tabs_*'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Sessions\Session_*'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Sessions\Tabs_*'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Sessions\Session_*'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Sessions\Tabs_*'
+    separator: '\'
+  supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
-urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/webbrowser/ChromeCache.html']
 ---
 name: ChromiumBasedBrowsersCache
+aliases: [ChromeCache, ChromiumCache, EdgeCache]
 doc: |
   Caches of multiple Chromium-based browsers (Google Chrome, Brave, Chromium,
   Yandex, Opera, Edge, EdgeBeta).
 
+  Canary uses "Chrome SxS" on windows.
+
   * Disk cache (or Cache)
   * Media cache
   * Application cache
   * GPU shader cache
   * PNaCl translation cache
 sources:
 - type: FILE
@@ -224,167 +379,190 @@
     - '%%users.localappdata%%\Yandex\YandexBrowser\User Data\*\Media Cache\*'
     separator: '\'
   supported_os: [Windows]
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Caches/Chromium/*/Cache/*'
-    - '%%users.homedir%%/Caches/Google/Chrome Canary/*/Cache/*'
     - '%%users.homedir%%/Caches/Google/Chrome/*/Cache/*'
+    - '%%users.homedir%%/Caches/Google/Chrome Beta/*/Cache/*'
+    - '%%users.homedir%%/Caches/Google/Chrome Canary/*/Cache/*'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Application Cache/*'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/Cache/*'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/Cache/*'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/PnaclTranslationCache/*'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Application Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Application Cache/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Chromium/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Chromium/PnaclTranslationCache/*'
+    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Application Cache/*'
+    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/GPUCache/*'
+    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Media Cache/*'
+    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/PnaclTranslationCache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Application Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Application Cache/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Application Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Application Cache/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/GPUCache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Media Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/PnaclTranslationCache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Application Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Application Cache/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/PnaclTranslationCache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Application Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/PnaclTranslationCache/*'
+    - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/Application Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/*/Application Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/PnaclTranslationCache/*'
-    - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/Application Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Microsoft Edge/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Microsoft Edge/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge/PnaclTranslationCache/*'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/*/Application Cache/*'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/*/Cache/*'
+    - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/*/GPUCache/*'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/Cache/*'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/PnaclTranslationCache/*'
-    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Application Cache/*'
-    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Cache/*'
-    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/GPUCache/*'
-    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/Cache/*'
-    - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/PnaclTranslationCache/*'
     - '%%users.homedir%%/Library/Caches/Chromium/*/Application Cache/*'
     - '%%users.homedir%%/Library/Caches/Chromium/*/Cache/*'
+    - '%%users.homedir%%/Library/Caches/Chromium/Cache/*'
     - '%%users.homedir%%/Library/Caches/Chromium/*/GPUCache/*'
     - '%%users.homedir%%/Library/Caches/Chromium/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Caches/Chromium/Cache/*'
     - '%%users.homedir%%/Library/Caches/Chromium/PnaclTranslationCache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome/*/Cache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome/Cache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome Beta/*/Cache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome Beta/Cache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome Beta/*/Media Cache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome Beta/PnaclTranslationCache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/*/Cache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/*/Media Cache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/Cache/*'
+    - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/*/Media Cache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome Canary/PnaclTranslationCache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome/*/Cache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome/*/Media Cache/*'
-    - '%%users.homedir%%/Library/Caches/Google/Chrome/Cache/*'
     - '%%users.homedir%%/Library/Caches/Google/Chrome/PnaclTranslationCache/*'
   supported_os: [Darwin]
 - type: FILE
   attributes:
     paths:
+    - '%%users.homedir%%/.cache/BraveSoftware/Brave-Browser/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/BraveSoftware/Brave-Browser/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-config/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/*'
+    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/Cache/*'
     - '%%users.homedir%%/.cache/chrome-remote-desktop/chrome-profile/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/chromium/*/Cache/*'
+    - '%%users.homedir%%/.cache/chromium/Cache/*'
     - '%%users.homedir%%/.cache/chromium/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/chromium/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/chromium/Cache/*'
     - '%%users.homedir%%/.cache/chromium/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.cache/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.cache/google-chrome/Cache/*'
     - '%%users.homedir%%/.cache/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.cache/microsoft-edge/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.cache/opera/*/Cache_Data/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Application Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Cache/*'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/GPUCache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Media Cache/*'
-    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/Cache/*'
     - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Application Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/GPUCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Application Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cache/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/Cache/*'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/GPUCache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Media Cache/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/Cache/*'
     - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/chromium/*/Application Cache/*'
     - '%%users.homedir%%/.config/chromium/*/Cache/*'
+    - '%%users.homedir%%/.config/chromium/Cache/*'
+    - '%%users.homedir%%/.config/chromium/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/chromium/*/GPUCache/*'
     - '%%users.homedir%%/.config/chromium/*/Media Cache/*'
-    - '%%users.homedir%%/.config/chromium/Cache/*'
     - '%%users.homedir%%/.config/chromium/PnaclTranslationCache/*'
+    - '%%users.homedir%%/.config/google-chrome/*/Application Cache/*'
     - '%%users.homedir%%/.config/google-chrome-beta/*/Application Cache/*'
     - '%%users.homedir%%/.config/google-chrome-beta/*/Cache/*'
+    - '%%users.homedir%%/.config/google-chrome-beta/Cache/*'
     - '%%users.homedir%%/.config/google-chrome-beta/*/GPUCache/*'
     - '%%users.homedir%%/.config/google-chrome-beta/*/Media Cache/*'
-    - '%%users.homedir%%/.config/google-chrome-beta/Cache/*'
     - '%%users.homedir%%/.config/google-chrome-beta/PnaclTranslationCache/*'
-    - '%%users.homedir%%/.config/google-chrome/*/Application Cache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Cache/*'
+    - '%%users.homedir%%/.config/google-chrome/Cache/*'
+    - '%%users.homedir%%/.config/google-chrome/*/Cache/Cache_Data/*'
     - '%%users.homedir%%/.config/google-chrome/*/GPUCache/*'
     - '%%users.homedir%%/.config/google-chrome/*/Media Cache/*'
-    - '%%users.homedir%%/.config/google-chrome/Cache/*'
     - '%%users.homedir%%/.config/google-chrome/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/microsoft-edge/*/GPUCache/*'
     - '%%users.homedir%%/.config/opera/*/Application Cache/*'
     - '%%users.homedir%%/.config/opera/*/Cache/*'
-    - '%%users.homedir%%/.config/opera/*/GPUCache/*'
-    - '%%users.homedir%%/.config/opera/*/Media Cache/*'
     - '%%users.homedir%%/.config/opera/Cache/*'
+    - '%%users.homedir%%/.config/opera/*/GPUCache/*'
     - '%%users.homedir%%/.config/opera/GPUCache/*'
+    - '%%users.homedir%%/.config/opera/*/Media Cache/*'
     - '%%users.homedir%%/.config/opera/PnaclTranslationCache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Application Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Cache/*'
+    - '%%users.homedir%%/.config/yandex-browser-beta/Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/GPUCache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/*/Media Cache/*'
-    - '%%users.homedir%%/.config/yandex-browser-beta/Cache/*'
     - '%%users.homedir%%/.config/yandex-browser-beta/PnaclTranslationCache/*'
     - '%%users.homedir%%/snap/chromium/common/chromium/*/Application Cache/*'
     - '%%users.homedir%%/snap/chromium/common/chromium/*/Cache/*'
+    - '%%users.homedir%%/snap/chromium/common/chromium/Cache/*'
     - '%%users.homedir%%/snap/chromium/common/chromium/*/GPUCache/*'
     - '%%users.homedir%%/snap/chromium/common/chromium/*/Media Cache/*'
-    - '%%users.homedir%%/snap/chromium/common/chromium/Cache/*'
     - '%%users.homedir%%/snap/chromium/common/chromium/PnaclTranslationCache/*'
   supported_os: [Linux]
 supported_os: [Darwin, Linux, Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/webbrowser/ChromeCache.html']
 ---
-name: ChromeCookies
-doc: Chrome Cookies database.
+name: ChromiumBasedBrowsersCookiesDatabaseFile
+aliases: [ChromeCookies]
+doc: |
+  Cookies database file for multiple Chromium-based browsers, such as Google
+  Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Cookies'
     - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Cookies-journal'
     - '%%users.localappdata%%\Chromium\User Data\*\Cookies'
@@ -440,14 +618,18 @@
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Cookies'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Cookies-journal'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Cookies'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Cookies-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Cookies'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Cookies-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Cookies'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Cookies-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Cookies'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Cookies-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Cookies'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Cookies-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Cookies'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Cookies-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Cookies'
@@ -462,14 +644,15 @@
   Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Extensions/**10'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/*/Extensions/**10'
     - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Extensions/**10'
   supported_os: [Darwin]
@@ -512,14 +695,15 @@
   such as Google Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Extension Activity'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge Beta/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/Microsoft Edge/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/Yandex/YandexBrowser/*/Extension Activity'
     - '%%users.homedir%%/Library/Application Support/com.operasoftware.Opera/*/Extension Activity'
   supported_os: [Darwin]
@@ -551,82 +735,117 @@
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls:
 - 'https://forensics.wiki/google_chrome#chromium-based-browsers'
 - 'https://forensics.wiki/google_chrome#extension-activity-database'
 ---
-name: ChromeExtensionRegistryKeys
-doc: Chrome extensions installed by writing windows registry keys.
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys:
-    - 'HKEY_LOCAL_MACHINE\Software\Google\Chrome\Extensions\**5'
-    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Google\Chrome\Extensions\**5'
-supported_os: [Windows]
-urls: ['https://developer.chrome.com/extensions/external_extensions#registry']
----
-name: ChromeFileSystem
+name: ChromiumBasedBrowsersFaviconsDatabaseFile
 doc: |
-  Google Chrome, Canary and Chromium File System files.
-
-  The File System directory backs Chrome's fileSystem API. Inside this
-  directory are a mixture of the data files saved using the fileSystem
-  API and LevelDB directories that track the logical structure of the
-  virtual file system.
+  Favicons database file for multiple Chromium-based browsers, such as Google
+  Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '%%users.localappdata%%\Chromium\User Data\*\File System\**5'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\File System\**5'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\File System\**5'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\File System\**5'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Favicons'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Favicons-journal'
+    - '%%users.localappdata%%\Chromium\User Data\*\Favicons'
+    - '%%users.localappdata%%\Chromium\User Data\*\Favicons-journal'
+    - '%%users.localappdata%%\Chromium\User Data\*\Network\Favicons'
+    - '%%users.localappdata%%\Chromium\User Data\*\Network\Favicons-journal'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Favicons'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Favicons-journal'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Favicons'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Favicons-journal'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Favicons'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Favicons-journal'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Favicons'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Favicons-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Favicons'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Favicons-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Favicons'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Favicons-journal'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Favicons'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Favicons-journal'
     separator: '\'
   supported_os: [Windows]
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/.config/google-chrome/*/File System/**5'
-    - '%%users.homedir%%/.config/chromium/*/File System/**5'
-    - '%%users.homedir%%/.config/google-chrome-beta/*/File System/**5'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/File System/**5'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/File System/**5'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Favicons'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Favicons-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Favicons'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Favicons-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Favicons'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Favicons-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Favicons'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Favicons-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Favicons'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Favicons-journal'
+    - '%%users.homedir%%/.config/chromium/*/Favicons'
+    - '%%users.homedir%%/.config/chromium/*/Favicons-journal'
+    - '%%users.homedir%%/.config/chromium/*/Network/Favicons'
+    - '%%users.homedir%%/.config/chromium/*/Network/Favicons-journal'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Favicons'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Favicons-journal'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Favicons'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Favicons-journal'
+    - '%%users.homedir%%/.config/google-chrome/*/Favicons'
+    - '%%users.homedir%%/.config/google-chrome/*/Favicons-journal'
+    - '%%users.homedir%%/.config/google-chrome/*/Network/Favicons'
+    - '%%users.homedir%%/.config/google-chrome/*/Network/Favicons-journal'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Favicons'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Favicons-journal'
+    - '%%users.homedir%%/.config/opera/Favicons'
+    - '%%users.homedir%%/.config/opera/Favicons-journal'
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/File System/**5'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/File System/**5'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/File System/**5'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Favicons-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Favicons'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Favicons-journal'
   supported_os: [Darwin]
 supported_os: [Darwin, Linux, Windows]
-urls:
-- 'https://developer.chrome.com/apps/fileSystem'
-- 'https://developer.mozilla.org/en-US/docs/Web/API/FileSystem'
-- 'https://dfir.blog/deciphering-browser-hieroglyphics-leveldb-filesystem/'
 ---
-name: ChromiumBasedBrowsersHistory
-aliases: [ChromeHistory]
+name: ChromiumBasedBrowsersHistoryDatabaseFile
+aliases: [ChromeHistory, ChromiumBasedBrowsersHistory]
 doc: |
-  Browsing history for multiple Chromium-based browsers (Google Chrome,
-  Brave, Chromium, Yandex, Opera, Edge, EdgeBeta).
+  Browsing history database file for multiple Chromium-based browsers, such as
+  Google Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Archived History'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/Archived History-journal'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/History'
     - '%%users.homedir%%/Library/Application Support/BraveSoftware/Brave-Browser/*/History-journal'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Archived History'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/Archived History-journal'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/History'
     - '%%users.homedir%%/Library/Application Support/Chromium/*/History-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Archived History'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Archived History-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/History'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/History-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Archived History'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Archived History-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/History'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/History-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Archived History'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Archived History-journal'
     - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/History'
@@ -736,189 +955,176 @@
     separator: '\'
   supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 urls:
 - 'https://forensics.wiki/google_chrome'
 - 'https://forensics.wiki/google_chrome#chromium-based-browsers'
 ---
-name: ChromeIndexedDB
+name: ChromiumBasedBrowsersLoginDataDatabaseFile
 doc: |
-  Google Chrome, Canary and Chromium IndexedDB files.
-
-  The IndexedDB directory contains one directory per origin that uses
-  IndexedDB, named like https_www.example.com_0.indexeddb.leveldb,
-  chrome-extension_app-id-xxx_0.indexeddb.leveldb, or
-  https_www.example.com_0.indexeddb.blob. Inside each of the *.leveldb
-  directories are the files the comprise a LevelDB database, which in turn
-  holds IndexedDB data for that origin. There may be an accompanying .blob
-  directory, which contains a nested folder structure of blobs.
+  Login Data database file for multiple Chromium-based browsers, such as Google
+  Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '%%users.localappdata%%\Chromium\User Data\*\IndexedDB\**5'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\IndexedDB\**5'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\IndexedDB\**5'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\IndexedDB\**5'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Login Data'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Login Data-journal'
+    - '%%users.localappdata%%\Chromium\User Data\*\Login Data'
+    - '%%users.localappdata%%\Chromium\User Data\*\Login Data-journal'
+    - '%%users.localappdata%%\Chromium\User Data\*\Network\Login Data'
+    - '%%users.localappdata%%\Chromium\User Data\*\Network\Login Data-journal'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Login Data'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Login Data-journal'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Login Data'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Login Data-journal'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Login Data'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Login Data-journal'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Login Data'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Login Data-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Login Data'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Login Data-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Login Data'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Login Data-journal'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Login Data'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Login Data-journal'
     separator: '\'
   supported_os: [Windows]
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/.config/google-chrome/*/IndexedDB/**5'
-    - '%%users.homedir%%/.config/chromium/*/IndexedDB/**5'
-    - '%%users.homedir%%/.config/google-chrome-beta/*/IndexedDB/**5'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/IndexedDB/**5'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/IndexedDB/**5'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Login Data'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Login Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Login Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Login Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Login Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Login Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Login Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Login Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Login Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Login Data-journal'
+    - '%%users.homedir%%/.config/chromium/*/Login Data'
+    - '%%users.homedir%%/.config/chromium/*/Login Data-journal'
+    - '%%users.homedir%%/.config/chromium/*/Network/Login Data'
+    - '%%users.homedir%%/.config/chromium/*/Network/Login Data-journal'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Login Data'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Login Data-journal'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Login Data'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Login Data-journal'
+    - '%%users.homedir%%/.config/google-chrome/*/Login Data'
+    - '%%users.homedir%%/.config/google-chrome/*/Login Data-journal'
+    - '%%users.homedir%%/.config/google-chrome/*/Network/Login Data'
+    - '%%users.homedir%%/.config/google-chrome/*/Network/Login Data-journal'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Login Data'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Login Data-journal'
+    - '%%users.homedir%%/.config/opera/Login Data'
+    - '%%users.homedir%%/.config/opera/Login Data-journal'
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/IndexedDB/**5'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/IndexedDB/**5'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/IndexedDB/**5'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Login Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Login Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Login Data-journal'
   supported_os: [Darwin]
 supported_os: [Darwin, Linux, Windows]
-urls: ['https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API']
 ---
-name: ChromeLocalStorage
+name: ChromiumBasedBrowsersWebDataDatabaseFile
 doc: |
-  Google Chrome, Canary and Chromium Local Storage files.
-
-  Chrome 60 and earlier versions used individual .sqlite files per origin for Local Storage, stored in the Local Storage directory root.
-  In Chrome 61, a leveldb directory was added inside the root Local Storage directory, and new origins saved Local Storage data in a single LevelDB there.
-
-  Existing .sqlite files are kept (not moved to leveldb), so it is possible for a single Chrome profile to use both SQLite and LevelDB for Local Storage.
+  Web Data database file for multiple Chromium-based browsers, such as Google
+  Chrome, Brave, Chromium, Yandex, Opera, Edge, EdgeBeta.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Local Storage/**'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Local Storage/**'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Local Storage/**'
-  supported_os: [Darwin]
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.homedir%%/.config/google-chrome/*/Local Storage/**'
-    - '%%users.homedir%%/.config/chromium/*/Local Storage/**'
-    - '%%users.homedir%%/.config/google-chrome-beta/*/Local Storage/**'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Local Storage/**'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Local Storage/**'
-  supported_os: [Linux]
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.localappdata%%\Chromium\User Data\*\Local Storage\**'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Local Storage\**'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Local Storage\**'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Local Storage\**'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Web Data'
+    - '%%users.localappdata%%\BraveSoftware\Brave-Browser\User Data\*\Network\Web Data-journal'
+    - '%%users.localappdata%%\Chromium\User Data\*\Web Data'
+    - '%%users.localappdata%%\Chromium\User Data\*\Web Data-journal'
+    - '%%users.localappdata%%\Chromium\User Data\*\Network\Web Data'
+    - '%%users.localappdata%%\Chromium\User Data\*\Network\Web Data-journal'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Web Data'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Web Data-journal'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Web Data'
+    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Network\Web Data-journal'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Web Data'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Web Data-journal'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Web Data'
+    - '%%users.localappdata%%\Google\Chrome\User Data\*\Network\Web Data-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Web Data'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Web Data-journal'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Web Data'
+    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Network\Web Data-journal'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Web Data'
+    - '%%users.appdata%%\Opera Software\Opera Stable\Network\Web Data-journal'
     separator: '\'
   supported_os: [Windows]
-supported_os: [Darwin, Linux, Windows]
----
-name: ChromePreferences
-doc: Chrome Preferences file.
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Preferences'
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Secure Preferences'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Preferences'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Secure Preferences'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Preferences'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Secure Preferences'
-  supported_os: [Darwin]
 - type: FILE
   attributes:
     paths:
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Preferences'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Secure Preferences'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Preferences'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Secure Preferences'
-    - '%%users.homedir%%/.config/chromium/*/Preferences'
-    - '%%users.homedir%%/.config/chromium/*/Secure Preferences'
-    - '%%users.homedir%%/.config/google-chrome/*/Preferences'
-    - '%%users.homedir%%/.config/google-chrome/*/Secure Preferences'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Web Data'
+    - '%%users.homedir%%/.config/BraveSoftware/Brave-Browser/*/Web Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Web Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Web Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Web Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Network/Web Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Web Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Web Data-journal'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Web Data'
+    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Network/Web Data-journal'
+    - '%%users.homedir%%/.config/chromium/*/Web Data'
+    - '%%users.homedir%%/.config/chromium/*/Web Data-journal'
+    - '%%users.homedir%%/.config/chromium/*/Network/Web Data'
+    - '%%users.homedir%%/.config/chromium/*/Network/Web Data-journal'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Web Data'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Web Data-journal'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Web Data'
+    - '%%users.homedir%%/.config/google-chrome-beta/*/Network/Web Data-journal'
+    - '%%users.homedir%%/.config/google-chrome/*/Web Data'
+    - '%%users.homedir%%/.config/google-chrome/*/Web Data-journal'
+    - '%%users.homedir%%/.config/google-chrome/*/Network/Web Data'
+    - '%%users.homedir%%/.config/google-chrome/*/Network/Web Data-journal'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Web Data'
+    - '%%users.homedir%%/.config/microsoft-edge/*/Web Data-journal'
+    - '%%users.homedir%%/.config/opera/Web Data'
+    - '%%users.homedir%%/.config/opera/Web Data-journal'
   supported_os: [Linux]
 - type: FILE
   attributes:
     paths:
-    - '%%users.localappdata%%\Chromium\User Data\*\Preferences'
-    - '%%users.localappdata%%\Chromium\User Data\*\Secure Preferences'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Preferences'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Secure Preferences'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Preferences'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Secure Preferences'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Preferences'
-    separator: '\'
-  supported_os: [Windows]
-supported_os: [Darwin, Linux, Windows]
-urls: ['https://forensics.wiki/google_chrome#configuration']
----
-name: ChromeSessionStorage
-doc: |
-  Google Chrome, Canary and Chromium Sessions and Session Storage files.
-
-  The Sessions directory contains information for restoring tabs and windows
-  from a browsing session.
-
-  The Session Storage directory contains the files that comprise a LevelDB
-  database, which in turn holds the Session Storage data.
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Session Storage/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Session Storage/*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Session Storage/*'
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Sessions/Session_*'
-    - '%%users.homedir%%/Library/Application Support/Chromium/*/Sessions/Tabs_*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Sessions/Session_*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Sessions/Tabs_*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Sessions/Session_*'
-    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Sessions/Tabs_*'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Chromium/*/Network/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Beta/*/Network/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome Canary/*/Network/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Web Data-journal'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Web Data'
+    - '%%users.homedir%%/Library/Application Support/Google/Chrome/*/Network/Web Data-journal'
   supported_os: [Darwin]
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.homedir%%/.config/google-chrome/*/Session Storage/*'
-    - '%%users.homedir%%/.config/chromium/*/Session Storage/*'
-    - '%%users.homedir%%/.config/google-chrome-beta/*/Session Storage/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Session Storage/*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Session Storage/*'
-    - '%%users.homedir%%/.config/google-chrome/*/Sessions/Session_*'
-    - '%%users.homedir%%/.config/google-chrome/*/Sessions/Tabs_*'
-    - '%%users.homedir%%/.config/chromium/*/Sessions/Session_*'
-    - '%%users.homedir%%/.config/chromium/*/Sessions/Tabs_*'
-    - '%%users.homedir%%/.config/google-chrome-beta/*/Sessions/Session_*'
-    - '%%users.homedir%%/.config/google-chrome-beta/*/Sessions/Tabs_*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Sessions/Session_*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-profile/*/Sessions/Tabs_*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Sessions/Session_*'
-    - '%%users.homedir%%/.config/chrome-remote-desktop/chrome-config/google-chrome/*/Sessions/Tabs_*'
-  supported_os: [Linux]
-- type: FILE
-  attributes:
-    paths:
-    - '%%users.localappdata%%\Chromium\User Data\*\Session Storage\*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Session Storage\*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Session Storage\*'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Session Storage\*'
-    - '%%users.localappdata%%\Chromium\User Data\*\Sessions\Session_*'
-    - '%%users.localappdata%%\Chromium\User Data\*\Sessions\Tabs_*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Sessions\Session_*'
-    - '%%users.localappdata%%\Google\Chrome SxS\User Data\*\Sessions\Tabs_*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Sessions\Session_*'
-    - '%%users.localappdata%%\Google\Chrome\User Data\*\Sessions\Tabs_*'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Sessions\Session_*'
-    - '%%users.localappdata%%\Microsoft\Edge\User Data\*\Sessions\Tabs_*'
-    separator: '\'
-  supported_os: [Windows]
 supported_os: [Darwin, Linux, Windows]
 ---
 name: FirefoxCache
 doc: Mozilla Firefox browser caches.
 sources:
 - type: FILE
   attributes:
@@ -1134,26 +1340,46 @@
 name: InternetExplorerHistory
 doc: |
   Microsoft Internet Explorer (MSIE) browser history.
 
   * MSIE 4 - 9 Cache files (index.dat);
   * MSIE 10 WebCacheV*.dat files.
 sources:
+- type: ARTIFACT_GROUP
+  attributes:
+    names:
+    - 'InternetExplorerHistoryDatabaseFile'
+    - 'InternetExplorerIndexDatFiles'
+supported_os: [Windows]
+urls: ['https://forensics.wiki/internet_explorer']
+---
+name: InternetExplorerHistoryDatabaseFile
+doc: Microsoft Internet Explorer (MSIE) 10 browser history database file (WebCacheV*.dat).
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%users.localappdata%%\Microsoft\Windows\WebCache\WebCacheV*.dat']
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://forensics.wiki/internet_explorer']
+---
+name: InternetExplorerIndexDatFiles
+doc: Microsoft Internet Explorer (MSIE) 4 - 9 cache and history files (index.dat).
+sources:
 - type: FILE
   attributes:
     paths:
     - '%%users.appdata%%\Microsoft\Windows\IEDownloadHistory\index.dat'
     - '%%users.localappdata%%\Microsoft\Feeds Cache\index.dat'
     - '%%users.localappdata%%\Microsoft\Windows\History\History.IE5\*\index.dat'
     - '%%users.localappdata%%\Microsoft\Windows\History\History.IE5\index.dat'
     - '%%users.localappdata%%\Microsoft\Windows\History\Low\History.IE5\*\index.dat'
     - '%%users.localappdata%%\Microsoft\Windows\History\Low\History.IE5\index.dat'
     - '%%users.localappdata%%\Microsoft\Windows\Temporary Internet Files\Content.IE5\index.dat'
     - '%%users.localappdata%%\Microsoft\Windows\Temporary Internet Files\Low\Content.IE5\index.dat'
-    - '%%users.localappdata%%\Microsoft\Windows\WebCache\WebCacheV*.dat'
     - '%%users.userprofile%%\Local Settings\History\History.IE5\index.dat'
     separator: '\'
 supported_os: [Windows]
 urls: ['https://forensics.wiki/internet_explorer']
 ---
 name: InternetExplorerProtectedModeElevationPolicies
 doc: |
```

### Comparing `artifacts-20230928/data/webservers.yaml` & `artifacts-20240518/artifacts/data/webservers.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,9 @@
 # Webserver related artifacts.
 ---
-name: ApacheConfigurationFolder
-doc: Location where Apache keeps configuration files
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '/etc/apache2/*.conf'
-    - '/etc/httpd/*.conf'
-    - '/etc/httpd/conf.d/*.conf'
-    - '/etc/httpd/conf.modules.d/*.conf'
-supported_os: [Linux]
----
-name: ApacheDefaultSiteConfigurationFile
-doc: Location where Apache keeps the default site configuration file.
-sources:
-- type: FILE
-  attributes: {paths: ['/etc/apache2/sites-available/000-default.conf']}
-supported_os: [Linux]
----
 name: ApacheAccessLogs
 doc: Location where Apache access logs are stored
 sources:
 - type: FILE
   attributes:
     paths:
     - '/var/log/apache/access_log*'
@@ -37,14 +18,33 @@
 - type: FILE
   attributes:
     paths: ['%%environ_systemdrive%%\**6\logs\access.log*']
     separator: '\'
   supported_os: [Windows]
 supported_os: [Linux, Windows]
 ---
+name: ApacheConfigurationFolder
+doc: Location where Apache keeps configuration files
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '/etc/apache2/*.conf'
+    - '/etc/httpd/*.conf'
+    - '/etc/httpd/conf.d/*.conf'
+    - '/etc/httpd/conf.modules.d/*.conf'
+supported_os: [Linux]
+---
+name: ApacheDefaultSiteConfigurationFile
+doc: Location where Apache keeps the default site configuration file.
+sources:
+- type: FILE
+  attributes: {paths: ['/etc/apache2/sites-available/000-default.conf']}
+supported_os: [Linux]
+---
 name: ApacheErrorLogs
 doc: Location where Apache error logs are stored
 sources:
 - type: FILE
   attributes:
     paths:
     - '/var/log/apache/error*'
@@ -96,12 +96,13 @@
 ---
 name: MicrosoftIISLogs
 doc: Internet Information Services (IIS) web server's log files.
 sources:
 - type: FILE
   attributes:
     paths:
-    - '%%environ_systemroot%%\System32\LogFiles\W3SVC*\*.log'
     - '%%environ_systemdrive%%\inetpub\logs\LogFiles\*.log'
+    - '%%environ_systemdrive%%\inetpub\logs\LogFiles\W3SVC*\*.log'
     - '%%environ_systemdrive%%\Resources\Directory\*\LogFiles\Web\W3SVC*\*.log'
+    - '%%environ_systemroot%%\System32\LogFiles\W3SVC*\*.log'
     separator: '\'
 supported_os: [Windows]
```

### Comparing `artifacts-20230928/data/windows.yaml` & `artifacts-20240518/artifacts/data/windows.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,69 @@
 # Windows specific artifacts.
 ---
+name: WindowsActionCenterSettings
+doc: |
+  Windows Action Center Settings
+
+  Malware can modify these keys to disable notifications that occur
+  when various security features are disabled. One malware family
+  known to modify these keys is Kovter, a well-known trojan.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Action Center\Checks\{e8433b72-5842-4d43-8645-bc2c35960837}.check.*', value: 'CheckSetting'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Action Center\Checks\{e8433b72-5842-4d43-8645-bc2c35960837}.check.*', value: 'CheckSetting'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Notifications\Settings\Windows.SystemToast.SecurityAndMaintenance', value: 'Enabled'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Notifications\Settings\Windows.SystemToast.SecurityAndMaintenance', value: 'Enabled'}
+supported_os: [Windows]
+urls:
+- 'https://winaero.com/blog/registry-tweak-to-disable-action-center-notifications-in-windows-7/'
+- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0517-0524.html'
+- 'https://blogs.technet.microsoft.com/platforms_lync_cloud/2017/05/05/disabling-windows-10-action-center-notifications/'
+---
 name: WindowsActiveDesktop
 doc: Windows Active Desktop settings and components.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
     - 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Internet Explorer\Desktop\Components\*'
     - 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Internet Explorer\Desktop\General'
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/ActiveDesktop.html']
 ---
-name: WindowsActiveDirectoryDatabase
-doc: Windows Active Directory data store file.
+name: WindowsActiveDirectoryDatabaseFile
+aliases: [WindowsActiveDirectoryDatabase]
+doc: Windows Active Directory database file (ntds.dit).
 sources:
 - type: FILE
   attributes:
-    paths: ['%%environ_systemroot%%\ntds\ntds.dit']
+    paths:
+    - '%%environ_systemroot%%\ntds\ntds.dit'
+    - '%%environ_systemroot%%\ServicePackFiles\*\ntds.dit*'
+    - '%%environ_systemroot%%\SoftwareDistribution\Download\*\*\ntds.dit*'
+    - '%%environ_systemroot%%\System32\ntds.dit'
     separator: '\'
 supported_os: [Windows]
 urls: ['https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2003/cc772829(v=ws.10)']
 ---
+name: WindowsActiveSyncAutoStart
+doc: Windows ActiveSync AutoStart entries
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys:
+    - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows CE Services\AutoStartOnConnect\*'
+    - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows CE Services\AutoStartOnDisconnect\*'
+    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows CE Services\AutoStartOnConnect\*'
+    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows CE Services\AutoStartOnDisconnect\*'
+supported_os: [Windows]
+urls: ['https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2']
+---
 name: WindowsActivitiesCacheDatabase
 doc: SQLite database containing the Windows activities cache.
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.localappdata%%\ConnectedDevicesPlatform\L.%%users.username%%\ActivitiesCache.db']
     separator: '\'
@@ -195,15 +234,16 @@
 - type: ARTIFACT_GROUP
   attributes:
     names:
     - 'WindowsApplicationCompatibilityInstalledShimDatabases'
     - 'WindowsApplicationCompatibilityShimDatabaseMappings'
 supported_os: [Windows]
 ---
-name: WinAppXRT
+name: WindowsAppXRT
+aliases: [WinAppXRT]
 doc: WinAppXRT DLL loaded by .Net applications when the APPX_PROCESS environment variable is set.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%environ_systemroot%%\system32\WinAppXRT.dll'
     - '%%environ_systemroot%%\WinAppXRT.dll'
@@ -318,14 +358,25 @@
   attributes:
     key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\BootVerificationProgram', value: 'ImagePath'}]
 supported_os: [Windows]
 urls:
 - 'https://technet.microsoft.com/en-us/library/cc786702(WS.10).aspx'
 - 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
 ---
+name: WindowsBootConfigurationSettings
+doc: Windows Boot Configuration Settings
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\BCD00000000\Objects\*\Elements\16000009', value: 'Element'}
+    - {key: 'HKEY_LOCAL_MACHINE\BCD00000000\Objects\*\Elements\250000e0', value: 'Element'}
+supported_os: [Windows]
+urls: ['https://forensics.wiki/windows_boot_configuration_data']
+---
 name: WindowsCIMRepositoryFiles
 doc: |
   Windows Common Information Model (CIM) repository.
 
   Persistent database that holds the schema, also called the object repository or class store,
   that models the managed environment and defines every piece of data exposed by WMI.
 
@@ -377,15 +428,14 @@
 aliases: [WinCodePage]
 doc: The system code page.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\Nls\CodePage', value: 'ACP'}
-provides: [code_page]
 supported_os: [Windows]
 urls: ['https://winreg-kb.readthedocs.io/en/latest/sources/system-keys/Codepage.html']
 ---
 name: WindowsComputerName
 doc: The name of the system.
 sources:
 - type: REGISTRY_VALUE
@@ -717,17 +767,35 @@
 name: WindowsDomainName
 doc: The domain the system is connected to.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\Tcpip\Parameters', value: 'Domain'}
-provides: [domain]
 supported_os: [Windows]
 ---
+name: WindowsDisallowedSystemCertificates
+doc: |
+  Windows Disallowed System Certificates
+
+  Malware can add code-signing certificates associated with
+  antivirus programs to the disallowed list to prevent the
+  AV programs from running.
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys:
+    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
+    - 'HKEY_USERS\%%users.sid%%\Software\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
+    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
+    - 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
+supported_os: [Windows]
+urls:
+- 'https://blog.malwarebytes.com/detections/pum-optional-misplacedcertificate/'
+---
 name: WindowsEnvironmentUserLoginScripts
 doc: User login scripts configured via Windows environment variables.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_USERS\%%users.sid%%\Environment', value: 'UserInitLogonServer'}
@@ -741,15 +809,14 @@
 name: WindowsEnvironmentVariableAllUsersProfile
 doc: The system-wide %AllUsersProfile% environment variable contains the path of the of the "All Users" or "Common" profile directory.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList', value: 'AllUsersProfile'}
-provides: [environ_allusersprofile]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableAppxProcess
 doc: |
   The user-specific %APPX_PROCESS% environment variable is used for .NET applications.
 
@@ -765,82 +832,75 @@
 name: WindowsEnvironmentVariableCommonProgramFiles
 doc: The %COMMONPROGRAMFILES% environment variable contains the path of the common program files folder.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion', value: 'CommonFilesDir'}
-provides: [environ_commonprogramfiles]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableCommonProgramFilesX86
 doc: The %COMMONPROGRAMFILES(X86)% environment variable contains the path of the 32-bit common program files folder on a 64-bit Windows installation.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion', value: 'CommonFilesDir (x86)'}
-provides: [environ_commonprogramfilesx86]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableComSpec
 doc: The %ComSpec% environment variable contains the path of the command processor, typically "cmd.exe".
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Environment', value: 'ComSpec'}
-provides: [environ_comspec]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableDriverData
 doc: The %DriverData% environment variable contains the path of the directory used for temporary state files of user-mode drivers.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Environment', value: 'DriverData'}
-provides: [environ_driverdata]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariablePath
 aliases: [WinPathEnvironmentVariable]
 doc: The %PATH% environment variable contains an ordered list of paths of directories that will be searched on execution request without a specific path.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\Session Manager\Environment', value: 'Path'}
-provides: [environ_path]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableProfilesDirectory
 doc: The %ProfilesDirectory% environment variable contain a path of a directory that contains the users' profile directories, typically "%SystemDrive%\Users".
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList', value: 'ProfilesDirectory'}
-provides: [environ_profilesdirectory]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableProgramData
 doc: The %ProgramData% environment variable contains a path of the "Program Data" directory.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList', value: 'ProgramData'}
-provides: [environ_programdata]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableProgramFiles
 aliases: [ProgramFiles]
 doc: The %ProgramFiles% environment variable contains a path of the "Program Files" directory.
 sources:
@@ -848,15 +908,14 @@
   attributes:
     paths: ['\Program Files']
     separator: '\'
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion', value: 'ProgramFilesDir'}
-provides: [environ_programfiles]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableProgramFilesX86
 aliases: [ProgramFilesx86]
 doc: The %ProgramFiles(x86)% environment variable contains a path of the 32-bit "Program Files" directory on a 64-bit Windows installation.
 sources:
@@ -864,27 +923,25 @@
   attributes:
     paths: ['\Program Files (x86)']
     separator: '\'
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion', value: 'ProgramFilesDir (x86)'}
-provides: [environ_programfilesx86]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableSystemDrive
 doc: |
   The %SystemDrive% environment variable contains the letter of the drive in which the system directory is located, typically "C:".
 
   This value is not present in the Windows Registry but can be derived from %SystemRoot%.
 sources:
 - type: ARTIFACT_GROUP
   attributes: {names: ['WindowsEnvironmentVariableSystemRoot']}
-provides: [environ_systemdrive]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableSystemRoot
 aliases: [SystemRoot]
 doc: The %SystemRoot%, environment variable contains the path of the system directory, typically "C:\Windows".
 sources:
@@ -896,27 +953,25 @@
     - '\WINNT35'
     - '\WTSRV'
     separator: '\'
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion', value: 'SystemRoot'}
-provides: [environ_systemroot]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableTemp
 aliases: [TempEnvironmentVariable]
 doc: The %TEMP% environment variable.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\Session Manager\Environment', value: 'TEMP'}
-provides: [environ_temp]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEnvironmentVariableWinDir
 aliases: [WinDirEnvironmentVariable]
 doc: The %WinDir%, environment variable contains the path of the Windows directory, typically "C:\Windows".
 sources:
@@ -928,15 +983,14 @@
     - '\WINNT35'
     - '\WTSRV'
     separator: '\'
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\Session Manager\Environment', value: 'windir'}
-provides: [environ_windir]
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EnvironmentVariables.html']
 ---
 name: WindowsEventLogApplication
 doc: Application Windows Event Log.
 sources:
 - type: FILE
@@ -1222,14 +1276,72 @@
     - 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\PrintersAndFaxes\NameSpace\DelegateFolders'
     - 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\SessionInfo\*\PrintersAndFaxes\NameSpace'
     - 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\SessionInfo\*\PrintersAndFaxes\NameSpace\DelegateFolders'
 supported_os: [Windows]
 urls:
 - 'http://www.geoffchappell.com/studies/windows/shell/shell32/classes/printers.htm'
 ---
+name: WindowsExplorerSettings
+doc: |
+  Windows Explorer Settings
+
+  Malware can modify these keys to make it more difficult for the
+  user to detect and remove malicious software.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
+supported_os: [Windows]
+urls:
+- 'https://www.sdkhere.com/2016/02/analysis-of-malware-using-wmi-query.html'
+- 'https://www.trendmicro.com/vinfo/us/threat-encyclopedia/malware/troj_mandrom.e'
+- 'https://www.trendmicro.com/vinfo/us/threat-encyclopedia/malware/troj_deleter.ah'
+- 'https://blog.malwarebytes.com/detections/pum-optional-disabledrightclick/'
+- 'https://blog.malwarebytes.com/detections/pum-optional-disableshowcontrolpanel/'
+---
 name: WindowsFileTypeAutorunAssociations
 doc: |
   Registry value for what application class identifier (CLSID) to launch for a file extension.
 
   Extension subkeys start with a dot. The '(Default)' value will be a ProgID,
   which points to another entry in HKCR specifying the command to run to open
   a file of the given type. The WindowsShellOpenCommand artifact is associated
@@ -1288,14 +1400,112 @@
     - '%%environ_systemroot%%\System32\GroupPolicy\Machine\Scripts\psscripts.ini'
     - '%%environ_systemroot%%\System32\GroupPolicy\Machine\Scripts\scripts.ini'
     - '%%environ_systemroot%%\System32\GroupPolicy\Machine\Scripts\Shutdown\*'
     - '%%environ_systemroot%%\System32\GroupPolicy\Machine\Scripts\Startup\*'
     separator: '\'
 supported_os: [Windows]
 ---
+name: WindowsFirewallAuthorizedApplications
+doc: |
+  Windows Firewall Authorized Applications
+
+  Malware can add paths to this list to more easily communicate
+  over the network on an infected machine. For instance, Emotet
+  modifies some these settings after gaining execution.
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys:
+    # Windows XP and 2003
+    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\DomainProfile\AuthorizedApplications\List\*'
+    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\StandardProfile\AuthorizedApplications\List\*'
+    # Windows Vista and later
+    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile\AuthorizedApplications\List\*'
+    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile\AuthorizedApplications\List\*'
+    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile\AuthorizedApplications\List\*'
+supported_os: [Windows]
+urls:
+- 'https://threatvector.cylance.com/en_us/home/threat-spotlight-eyepyramid-malware.html'
+- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0524-0531.html'
+---
+name: WindowsFirewallGloballyOpenPorts
+doc: |
+  Windows Firewall Globally Open Ports
+
+  Malware can add to the list of open ports to avoid
+  having to create Windows Firewall exceptions tied
+  to specific applications.
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys:
+    # Windows XP and 2003
+    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\DomainProfile\GloballyOpenPorts\List\*'
+    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\StandardProfile\GloballyOpenPorts\List\*'
+    # Windows Vista and later
+    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile\GloballyOpenPorts\List\*'
+    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile\GloballyOpenPorts\List\*'
+    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile\GloballyOpenPorts\List\*'
+supported_os: [Windows]
+urls:
+- 'https://qaforce.wordpress.com/2009/10/06/windows-firewall-registry-keys/'
+- 'https://github.com/steeve85/Malwares/wiki/Registry'
+---
+name: WindowsFirewallPolicySettings
+doc: |
+  Windows Firewall Policy Settings
+
+  Malware can modify these settings to more easily communicate
+  over the network on an infected machine. For instance, Emotet
+  modifies some these settings after gaining execution.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'EnableFirewall'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DisableNotifications'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DoNotAllowExceptions'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DefaultInboundAction'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DefaultOutboundAction'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'EnableFirewall'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DisableNotifications'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DoNotAllowExceptions'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DefaultInboundAction'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DefaultOutboundAction'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'EnableFirewall'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DisableNotifications'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DoNotAllowExceptions'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DefaultInboundAction'}
+    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DefaultOutboundAction'}
+supported_os: [Windows]
+urls:
+- 'https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/networking-mpssvc-svc-privateprofile-enablefirewall'
+- 'https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/networking-mpssvc-svc-privateprofile-disablenotifications'
+- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
+---
+name: WindowsFontDrivers
+doc: Windows font drivers from the Registry.
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys:
+    - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\Font Drivers\*'
+supported_os: [Windows]
+urls:
+- 'https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2'
+---
+name: WindowsHelpCenterDatabaseFile
+doc: Windows Help Center database file (HCdata.edb).
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_systemroot%%\PCHEALTH\HELPCTR\Database\HCdata.edb']
+    separator: '\'
+supported_os: [Windows]
+---
 name: WindowsHostsFiles
 doc: The Windows hosts and lmhosts file.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%environ_systemroot%%\System32\Drivers\etc\Lmhosts'
@@ -1798,14 +2008,35 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Internet Settings', value: 'ProxyServer'}
     - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Internet Settings', value: 'ProxyServer'}
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\NlaSvc\Parameters\Internet\ManualProxies', value: 'ProxyServer'}
     - {key: 'HKEY_USERS\%%users.sid%%\System\CurrentControlSet\Services\NlaSvc\Parameters\Internet\ManualProxies', value: 'ProxyServer'}
 supported_os: [Windows]
 urls: ['https://blog.malwarebytes.com/detections/pum-optional-proxyhijacker/']
 ---
+name: WindowsPushNotificationDatabaseFile
+doc: The Windows Push Notification (WPN) database file.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%users.localappdata%%\Microsoft\Windows\Notifications\wpndatabase.db'
+    - '%%environ_systemroot%%\System32\config\ystemprofile\AppData\Local\Microsoft\Windows\Notifications\wpndatabase.db'
+    separator: '\'
+supported_os: [Windows]
+---
+name: WindowsRDPClientBitmapCache
+doc: Artifacts of RDP connection contents
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%users.localappdata%%\Microsoft\Terminal Server Client\Cache\*.*']
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://forensics.wiki/windows#rdp-bitmap-cache']
+---
 name: WindowsRecentFileCacheBCF
 doc: The RecentFileCache.bcf file.
 sources:
 - type: FILE
   attributes:
     paths: ['%%environ_systemroot%%\AppCompat\Programs\RecentFileCache.bcf']
     separator: '\'
@@ -1838,15 +2069,14 @@
 ---
 name: WindowsRegistryCurrentControlSet
 aliases: [CurrentControlSet]
 doc: The current control set of the Windows Registry.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\Select', value: 'Current'}]}
-provides: [current_control_set]
 supported_os: [Windows]
 urls: ['https://github.com/libyal/winreg-kb/blob/main/documentation/System%20keys.asciidoc']
 ---
 name: WindowsRegistryFilesAndTransactionLogs
 doc: Windows user and system Registry files and transaction logs.
 sources:
 - type: ARTIFACT_GROUP
@@ -1864,15 +2094,14 @@
   Get SIDs for all users on the system with profiles present in the Registry.
 
   This looks in the Windows Registry where the profiles are stored and retrieves
   the paths for each profile.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList\*', value: 'ProfileImagePath'}]}
-provides: [users.sid, users.userprofile, users.homedir, users.username]
 supported_os: [Windows]
 urls: ['http://msdn.microsoft.com/en-us/library/windows/desktop/bb776892(v=vs.85).aspx']
 ---
 name: WindowsReleaseIdentifier
 doc: |
   The Windows 10 release identifier (or version number).
 
@@ -2001,15 +2230,16 @@
     - {key: 'HKEY_USERS\%%users.sid%%\Control Panel\Desktop', value: 'scrnsave.exe'}
 supported_os: [Windows]
 urls:
 - 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
 - 'https://technet.microsoft.com/en-us/library/cc737855(v=ws.10).aspx'
 - 'https://technet.microsoft.com/en-us/library/cc957840.aspx'
 ---
-name: WindowsSearchDatabase
+name: WindowsSearchDatabaseFile
+aliases: [WindowsSearchDatabase]
 doc: Windows Search database (Windows.edb).
 sources:
 - type: FILE
   attributes:
     paths: ['%%environ_allusersappdata%%\Microsoft\Search\Data\Applications\Windows\Windows.edb']
     separator: '\'
 supported_os: [Windows]
@@ -2049,274 +2279,14 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Classes\Wow6432Node\CLSID\*\PersistentAddinsRegistered\{89BCB740-6119-101A-BCB7-00DD010655AF}', value: ''}
 supported_os: [Windows]
 urls:
 - 'https://docs.microsoft.com/en-us/windows/desktop/search/-search-ifilter-about'
 - 'https://docs.microsoft.com/en-us/windows/desktop/search/-search-ifilter-implementations'
 - 'https://docs.microsoft.com/en-us/windows/desktop/search/-search-ifilter-registering-filters'
 ---
-name: WindowsSecurityProviders
-doc: Security Providers DLLs
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys: ['HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\SecurityProviders\*']
-supported_os: [Windows]
-urls:
-- 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
-- 'https://github.com/wmark/security-configuration/blob/master/Windows/disable-weak-ciphers-and-enable-TLS1.x.reg'
----
-name: WindowsServiceControlManagerExtension
-doc: Windows service control manager extension
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control', value: 'ServiceControlManagerExtension'}]
-supported_os: [Windows]
-urls:
-- 'http://forum.sysinternals.com/autoruns-and-windows-7_topic19770.html'
-- 'https://support.microsoft.com/en-us/kb/102985'
-- 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
-- 'http://www.silentrunners.org/Silent%20Runners.vbs'
----
-name: WindowsServices
-doc: Windows service and driver configurations.
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys: ['HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\*']
-supported_os: [Windows]
-urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/ServicesAndDrivers.html']
----
-name: WindowsActionCenterSettings
-doc: |
-  Windows Action Center Settings
-
-  Malware can modify these keys to disable notifications that occur
-  when various security features are disabled. One malware family
-  known to modify these keys is Kovter, a well-known trojan.
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs:
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Action Center\Checks\{e8433b72-5842-4d43-8645-bc2c35960837}.check.*', value: 'CheckSetting'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Action Center\Checks\{e8433b72-5842-4d43-8645-bc2c35960837}.check.*', value: 'CheckSetting'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Notifications\Settings\Windows.SystemToast.SecurityAndMaintenance', value: 'Enabled'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Notifications\Settings\Windows.SystemToast.SecurityAndMaintenance', value: 'Enabled'}
-supported_os: [Windows]
-urls:
-- 'https://winaero.com/blog/registry-tweak-to-disable-action-center-notifications-in-windows-7/'
-- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0517-0524.html'
-- 'https://blogs.technet.microsoft.com/platforms_lync_cloud/2017/05/05/disabling-windows-10-action-center-notifications/'
----
-name: WindowsBootConfigurationSettings
-doc: Windows Boot Configuration Settings
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\BCD00000000\Objects\*\Elements\16000009', value: 'Element'}
-    - {key: 'HKEY_LOCAL_MACHINE\BCD00000000\Objects\*\Elements\250000e0', value: 'Element'}
-supported_os: [Windows]
-urls: ['https://forensics.wiki/windows_boot_configuration_data']
----
-name: WindowsDisallowedSystemCertificates
-doc: |
-  Windows Disallowed System Certificates
-
-  Malware can add code-signing certificates associated with
-  antivirus programs to the disallowed list to prevent the
-  AV programs from running.
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys:
-    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
-    - 'HKEY_USERS\%%users.sid%%\Software\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
-    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
-    - 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Policies\Microsoft\SystemCertificates\Disallowed\Certificates\*'
-supported_os: [Windows]
-urls:
-- 'https://blog.malwarebytes.com/detections/pum-optional-misplacedcertificate/'
----
-name: WindowsExplorerSettings
-doc: |
-  Windows Explorer Settings
-
-  Malware can modify these keys to make it more difficult for the
-  user to detect and remove malicious software.
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'Hidden'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'HideFileExt'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowSuperHidden'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'HideSCAHealth'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoControlPanel'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoFolderOptions'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoRun'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'NoViewContextMenu'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Advanced', value: 'ShowControlPanel'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\Explorer', value: 'TaskbarNoNotification'}
-supported_os: [Windows]
-urls:
-- 'https://www.sdkhere.com/2016/02/analysis-of-malware-using-wmi-query.html'
-- 'https://www.trendmicro.com/vinfo/us/threat-encyclopedia/malware/troj_mandrom.e'
-- 'https://www.trendmicro.com/vinfo/us/threat-encyclopedia/malware/troj_deleter.ah'
-- 'https://blog.malwarebytes.com/detections/pum-optional-disabledrightclick/'
-- 'https://blog.malwarebytes.com/detections/pum-optional-disableshowcontrolpanel/'
----
-name: WindowsSystemSettings
-doc: |
-  Windows System Settings
-
-  Malware can modify these keys to make it more difficult for the
-  user to detect and remove malicious software.
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
-    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
-supported_os: [Windows]
-urls:
-- 'https://www.sdkhere.com/2016/02/analysis-of-malware-using-wmi-query.html'
-- 'https://www.thewindowsclub.com/enable-disable-command-prompt-windows'
-- 'https://blog.malwarebytes.com/detections/pum-optional-disableregistrytools/'
-- 'https://blog.malwarebytes.com/detections/pum-optional-disabletaskmgr/'
-- 'https://www.stigviewer.com/stig/windows_7/2014-04-02/finding/V-1154'
-- 'https://blog.malwarebytes.com/detections/pum-optional-nodispcpl/'
-- 'https://blog.malwarebytes.com/detections/pum-optional-disablecmdprompt/'
----
-name: WindowsFirewallAuthorizedApplications
-doc: |
-  Windows Firewall Authorized Applications
-
-  Malware can add paths to this list to more easily communicate
-  over the network on an infected machine. For instance, Emotet
-  modifies some these settings after gaining execution.
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys:
-    # Windows XP and 2003
-    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\DomainProfile\AuthorizedApplications\List\*'
-    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\StandardProfile\AuthorizedApplications\List\*'
-    # Windows Vista and later
-    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile\AuthorizedApplications\List\*'
-    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile\AuthorizedApplications\List\*'
-    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile\AuthorizedApplications\List\*'
-supported_os: [Windows]
-urls:
-- 'https://threatvector.cylance.com/en_us/home/threat-spotlight-eyepyramid-malware.html'
-- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0524-0531.html'
----
-name: WindowsFirewallGloballyOpenPorts
-doc: |
-  Windows Firewall Globally Open Ports
-
-  Malware can add to the list of open ports to avoid
-  having to create Windows Firewall exceptions tied
-  to specific applications.
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys:
-    # Windows XP and 2003
-    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\DomainProfile\GloballyOpenPorts\List\*'
-    - 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\WindowsFirewall\StandardProfile\GloballyOpenPorts\List\*'
-    # Windows Vista and later
-    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile\GloballyOpenPorts\List\*'
-    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile\GloballyOpenPorts\List\*'
-    - 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile\GloballyOpenPorts\List\*'
-supported_os: [Windows]
-urls:
-- 'https://qaforce.wordpress.com/2009/10/06/windows-firewall-registry-keys/'
-- 'https://github.com/steeve85/Malwares/wiki/Registry'
----
-name: WindowsFirewallPolicySettings
-doc: |
-  Windows Firewall Policy Settings
-
-  Malware can modify these settings to more easily communicate
-  over the network on an infected machine. For instance, Emotet
-  modifies some these settings after gaining execution.
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'EnableFirewall'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DisableNotifications'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DoNotAllowExceptions'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DefaultInboundAction'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\DomainProfile', value: 'DefaultOutboundAction'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'EnableFirewall'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DisableNotifications'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DoNotAllowExceptions'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DefaultInboundAction'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\PublicProfile', value: 'DefaultOutboundAction'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'EnableFirewall'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DisableNotifications'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DoNotAllowExceptions'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DefaultInboundAction'}
-    - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\SharedAccess\Parameters\FirewallPolicy\StandardProfile', value: 'DefaultOutboundAction'}
-supported_os: [Windows]
-urls:
-- 'https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/networking-mpssvc-svc-privateprofile-enablefirewall'
-- 'https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/networking-mpssvc-svc-privateprofile-disablenotifications'
-- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
----
 name: WindowsSecurityCenterSettings
 doc: |
   Windows Security Center Settings
 
   Malware can modify these settings to avoid detection on
   an infected machine. For instance, Emotet modifies some of
   these settings after gaining execution.
@@ -2344,103 +2314,57 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Security Center', value: 'UacDisableNotify'}
 supported_os: [Windows]
 urls:
 - 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
 - 'https://blog.appriver.com/phorphiex/trik-botnet-campaign-leads-to-multiple-infections-ransomware-banking-trojan-cryptojacking'
 - 'https://ccm.net/faq/1446-disabling-security-alerts-under-vista'
 ---
-name: WindowsSystemRestoreSettings
-doc: |
-  Windows System Restore Settings
-
-  Some malware, especially ransomware, will disable system restore
-  to make system recovery more difficult.
-sources:
-- type: REGISTRY_VALUE
-  attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableConfig'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableConfig'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableConfig'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableConfig'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableSR'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableSR'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableSR'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableSR'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\Installer', value: 'LimitSystemRestoreCheckpointing'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\Installer', value: 'LimitSystemRestoreCheckpointing'}
-supported_os: [Windows]
-urls:
-- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
-- 'https://www.windows-commandline.com/enable-disable-system-restore-service/'
-- 'https://docs.microsoft.com/en-us/windows/desktop/msi/limitsystemrestorecheckpointing'
----
-name: WindowsUserAccountControlSettings
-doc: |
-  Windows User Account Control Settings
-
-  Malware sometimes disables UAC to make it easier to perform
-  actions on an infected machine.
+name: WindowsSecurityProviders
+doc: Security Providers DLLs
 sources:
-- type: REGISTRY_VALUE
+- type: REGISTRY_KEY
   attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'EnableLUA'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'EnableLUA'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'ConsentPromptBehaviorAdmin'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'ConsentPromptBehaviorAdmin'}
+    keys: ['HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\SecurityProviders\*']
 supported_os: [Windows]
 urls:
-- 'https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-gpsb/958053ae-5397-4f96-977f-b7700ee461ec'
-- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
-- 'https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-gpsb/341747f5-6b5d-4d30-85fc-fa1cc04038d4'
+- 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
+- 'https://github.com/wmark/security-configuration/blob/master/Windows/disable-weak-ciphers-and-enable-TLS1.x.reg'
 ---
-name: WindowsUpgradeSettings
-doc: |
-  Windows Upgrade Settings
-
-  Malware sometimes disables a machine ability to upgrade from
-  previous versions of Windows to Windows 10. One malware family
-  known to modify these keys is Kovter, a well-known trojan.
+name: WindowsSecuritySettingsDatabases
+doc: Windows security settings databases (secedit.sdb and spsecupd.sdb)
 sources:
-- type: REGISTRY_VALUE
+- type: FILE
   attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\WindowsUpdate', value: 'DisableOSUpgrade'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\WindowsUpdate', value: 'DisableOSUpgrade'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\WindowsUpdate\OSUpgrade', value: 'ReservationsAllowed'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\WindowsUpdate\OSUpgrade', value: 'ReservationsAllowed'}
+    paths:
+    - '%%environ_systemroot%%\security\Database\secedit.sdb'
+    - '%%environ_systemroot%%\security\templates\spsecupd.sdb'
+    separator: '\'
 supported_os: [Windows]
-urls:
-- 'https://www.ghacks.net/2016/01/08/disableosupgrade-prevents-the-upgrade-to-windows-10/'
-- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0517-0524.html'
 ---
-name: WindowsUpdateSettings
-doc: Windows Update Settings
+name: WindowsServiceControlManagerExtension
+doc: Windows service control manager extension
 sources:
 - type: REGISTRY_VALUE
   attributes:
-    key_value_pairs:
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\WindowsUpdate\AU', value: 'NoAutoUpdate'}
-    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\WindowsUpdate\AU', value: 'NoAutoUpdate'}
+    key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control', value: 'ServiceControlManagerExtension'}]
 supported_os: [Windows]
 urls:
-- 'https://docs.microsoft.com/en-us/windows/deployment/update/waas-wu-settings'
-- 'https://blog.talosintelligence.com/2019/06/threat-roundup-0531-0607.html'
+- 'http://forum.sysinternals.com/autoruns-and-windows-7_topic19770.html'
+- 'https://support.microsoft.com/en-us/kb/102985'
+- 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
+- 'http://www.silentrunners.org/Silent%20Runners.vbs'
 ---
-name: WindowsFontDrivers
-doc: Windows font drivers from the Registry.
+name: WindowsServices
+doc: Windows service and driver configurations.
 sources:
 - type: REGISTRY_KEY
   attributes:
-    keys:
-    - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\Font Drivers\*'
+    keys: ['HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\*']
 supported_os: [Windows]
-urls:
-- 'https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2'
+urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/ServicesAndDrivers.html']
 ---
 name: WindowsSessionManagerBootExecute
 doc: Windows Session Manager BootExecute persistence.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\Session Manager', value: 'BootExecute'}]
@@ -2708,14 +2632,23 @@
   attributes:
     keys:
     - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\ShellServiceObjectDelayLoad'
     - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\ShellServiceObjectDelayLoad'
 supported_os: [Windows]
 urls: ['http://www.microsoft.com/security/portal/threat/encyclopedia/Entry.aspx?Name=TrojanClicker:Win32/Zirit.X#tab=2']
 ---
+name: WindowsSmsRouterInterceptStoreDatabaseFile
+doc: Windows SmsRouter intercept store database file (SmsInterceptStore.db)
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_programdata%%\Microsoft\SmsRouter\MessageStore\SmsInterceptStore.db']
+    separator: '\'
+supported_os: [Windows]
+---
 name: WindowsSetupApiLogs
 doc: Windows setup API logs.
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%environ_systemroot%%\setupapi.log'
@@ -2738,14 +2671,32 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Group Policy\State\Machine\Scripts\Shutdown\*\*', value: 'Script'}
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Group Policy\State\Machine\Scripts\Shutdown\*\*', value: 'Parameters'}
 supported_os: [Windows]
 urls:
 - 'https://technet.microsoft.com/en-us/library/ff404236.aspx'
 - 'https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2'
 ---
+name: WindowsStateRepositoryDeploymentDatabaseFile
+doc: The State Reposistory deployment database file (StateRepository-Deployment.srd).
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_programdata%%\Microsoft\Windows\AppRepository\StateRepository-Deployment.srd']
+    separator: '\'
+supported_os: [Windows]
+---
+name: WindowsStateRepositoryMachineDatabaseFile
+doc: The State Reposistory machine database file (StateRepository-Machine.srd).
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_programdata%%\Microsoft\Windows\AppRepository\StateRepository-Machine.srd']
+    separator: '\'
+supported_os: [Windows]
+---
 name: WindowsStartupFolderModification
 doc: Windows startup folder Registry values.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders', value: 'Common Startup'}
@@ -2827,14 +2778,80 @@
     paths:
     - '%%environ_systemroot%%\Prefetch\Ag*.db'
     - '%%environ_systemroot%%\Prefetch\Ag*.db.trx'
     separator: '\'
 supported_os: [Windows]
 urls: ['https://forensics.wiki/superfetch']
 ---
+name: WindowsSystemRestoreSettings
+doc: |
+  Windows System Restore Settings
+
+  Some malware, especially ransomware, will disable system restore
+  to make system recovery more difficult.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableConfig'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableConfig'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableConfig'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableConfig'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableSR'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableSR'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows NT\SystemRestore', value: 'DisableSR'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\SystemRestore', value: 'DisableSR'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\Installer', value: 'LimitSystemRestoreCheckpointing'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\Installer', value: 'LimitSystemRestoreCheckpointing'}
+supported_os: [Windows]
+urls:
+- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
+- 'https://www.windows-commandline.com/enable-disable-system-restore-service/'
+- 'https://docs.microsoft.com/en-us/windows/desktop/msi/limitsystemrestorecheckpointing'
+---
+name: WindowsSystemSettings
+doc: |
+  Windows System Settings
+
+  Malware can modify these keys to make it more difficult for the
+  user to detect and remove malicious software.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableCAD'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableRegistryTools'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'DisableTaskMgr'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'NoDispCPL'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
+    - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Policies\Microsoft\Windows\System', value: 'DisableCMD'}
+supported_os: [Windows]
+urls:
+- 'https://www.sdkhere.com/2016/02/analysis-of-malware-using-wmi-query.html'
+- 'https://www.thewindowsclub.com/enable-disable-command-prompt-windows'
+- 'https://blog.malwarebytes.com/detections/pum-optional-disableregistrytools/'
+- 'https://blog.malwarebytes.com/detections/pum-optional-disabletaskmgr/'
+- 'https://www.stigviewer.com/stig/windows_7/2014-04-02/finding/V-1154'
+- 'https://blog.malwarebytes.com/detections/pum-optional-nodispcpl/'
+- 'https://blog.malwarebytes.com/detections/pum-optional-disablecmdprompt/'
+---
 name: WindowsSystemIniFiles
 doc: Windows system ini files
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%environ_systemdrive%%\system.ini'
@@ -2958,14 +2975,31 @@
 - type: FILE
   attributes:
     paths: ['%%environ_systemroot%%\System32\sru\SRUDB.dat']
     separator: '\'
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/SystemResourceUsageMonitor.html']
 ---
+name: WindowsStartupInfo
+doc: |
+  StartupInfo XML files.
+
+  The files include the user account's Security Identifier (SID) in the name
+  and there could be up to 5 per user account. They contain a list of processes
+  that were executed within the first 90 seconds from the time the user logged
+  in. The info includes start time, the full command line and the parent
+  process info, among other things.
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_systemroot%%\System32\WDI\LogFiles\StartupInfo\*.xml']
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://forensics.wiki/windows#startup-info']
+---
 name: WindowsTempDirectories
 doc: Contents of the Windows temporary directories
 sources:
 - type: FILE
   attributes:
     paths:
     - '%%environ_systemdrive%%\Temp\*'
@@ -3015,47 +3049,33 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows NT\Terminal Services', value: 'InitialProgram'}
     - {key: 'HKEY_USERS\%%users.sid%%\Software\Policies\Microsoft\Windows NT\Terminal Services', value: 'InitialProgram'}
     - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows NT\Terminal Services', value: 'InitialProgram'}
     - {key: 'HKEY_USERS\%%users.sid%%\Software\Wow6432Node\Policies\Microsoft\Windows NT\Terminal Services', value: 'InitialProgram'}
 supported_os: [Windows]
 urls: ['https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2']
 ---
-name: WindowsRDPClientBitmapCache
-doc: Artifacts of RDP connection contents
+name: WindowsThumbcacheDatabaseFiles
+doc: Windows thumbcache_*.db files.
 sources:
 - type: FILE
   attributes:
-    paths: ['%%users.localappdata%%\Microsoft\Terminal Server Client\Cache\*.*']
+    paths: ['%%users.localappdata%%\Microsoft\Windows\Explorer\thumbcache_*.db']
     separator: '\'
 supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#rdp-bitmap-cache']
----
-name: WindowsActiveSyncAutoStart
-doc: Windows ActiveSync AutoStart entries
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys:
-    - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows CE Services\AutoStartOnConnect\*'
-    - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows CE Services\AutoStartOnDisconnect\*'
-    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows CE Services\AutoStartOnConnect\*'
-    - 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows CE Services\AutoStartOnDisconnect\*'
-supported_os: [Windows]
-urls: ['https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2']
+urls: ['https://forensics.wiki/vista_thumbcache/']
 ---
 name: WindowsTimezone
 aliases: [WinTimeZone]
 doc: The time zone of the system as a Windows time zone name or in MUI form.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\TimeZoneInformation', value: 'StandardName'}
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\TimeZoneInformation', value: 'TimeZoneKeyName'}
-provides: [time_zone]
 supported_os: [Windows]
 urls: ['https://winreg-kb.readthedocs.io/en/latest/sources/system-keys/Time-zones.html']
 ---
 name: WindowsToolPaths
 doc: Paths to windows tools such as defrag, chkdsk.
 sources:
 - type: REGISTRY_KEY
@@ -3066,14 +3086,27 @@
     - 'HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\MyComputer\cleanuppath'
     - 'HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\MyComputer\DefragPath'
 supported_os: [Windows]
 urls:
 - 'http://gladiator-antivirus.com/forum/index.php?showtopic=24610'
 - 'http://www.liutilities.com/products/registrybooster/tweaklibrary/tweaks/11118/'
 ---
+name: WindowsTileDataLayerDatabase
+doc: |
+  Windows tile data layer database (vedatamodel.edb)
+
+  The tile data layer database is used to store information about Start Tiles.
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%users.localappdata%%\TileDataLayer\Database\vedatamodel.edb']
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://forensics.wiki/extensible_storage_engine_(ese)_database_file_(edb)_format#tile-data-layer-database']
+---
 name: WindowsUninstallKeys
 doc: Uninstall Registry keys
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
     - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Uninstall\*\*'
@@ -3089,14 +3122,59 @@
   This Windows Registry value contains the monthly rollup patch version.
 sources:
 - type: REGISTRY_VALUE
   attributes: {key_value_pairs: [{key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion', value: 'UBR'}]}
 supported_os: [Windows]
 urls: ['https://social.technet.microsoft.com/Forums/en-US/cadee4de-24d0-403e-9f3e-75868abf8f34']
 ---
+name: WindowsUpdateCatalogDatabaseFile
+doc: Windows Update catalog package signatures database file (catdb).
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_systemroot%%\System32\catroot2\{*-*-*-*-*}\catdb']
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://learn.microsoft.com/en-us/windows-hardware/drivers/install/catalog-files']
+---
+name: WindowsUpdateDataStoreDatabaseFile
+doc: Windows Update data store database file (DataStore.edb).
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_windir%%\SoftwareDistribution\DataStore\DataStore.edb']
+    separator: '\'
+supported_os: [Windows]
+---
+name: WindowsUpdateLogFile
+doc: Windows Update log files.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%environ_programdata%%\USOShared\Logs\System\*.etl'
+    - '%%environ_systemroot%%\Logs\CBS\CBS*.log'
+    - '%%environ_systemroot%%\Logs\WindowsUpdate\WindowsUpdate*.etl'
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://learn.microsoft.com/en-us/windows/deployment/update/windows-update-logs']
+---
+name: WindowsUpdateSettings
+doc: Windows Update Settings
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\WindowsUpdate\AU', value: 'NoAutoUpdate'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\WindowsUpdate\AU', value: 'NoAutoUpdate'}
+supported_os: [Windows]
+urls:
+- 'https://docs.microsoft.com/en-us/windows/deployment/update/waas-wu-settings'
+- 'https://blog.talosintelligence.com/2019/06/threat-roundup-0531-0607.html'
+---
 name: WindowsUpdateStatus
 doc: Windows auto update status.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\WindowsUpdate\Auto Update\Results\Detect', value: 'LastError'}
@@ -3106,14 +3184,80 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\WindowsUpdate\Auto Update\Results\Install', value: 'LastError'}
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\WindowsUpdate\Auto Update\Results\Install', value: 'LastSuccessTime'}
 supported_os: [Windows]
 urls:
 - 'https://forensics.wiki/windows_update'
 - 'http://blogs.msdn.com/b/aruns_blog/archive/2011/06/20/active-setup-registry-key-what-it-is-and-how-to-create-in-the-package-using-admin-studio-install-shield.aspx'
 ---
+name: WindowsUpdateStoreDatabaseFile
+doc: The Update Service Orchestrator (USO) private update store database file.
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_programdata%%\USOPrivate\UpdateStore\store.db']
+    separator: '\'
+supported_os: [Windows]
+---
+name: WindowsUpgradeSettings
+doc: |
+  Windows Upgrade Settings
+
+  Malware sometimes disables a machine ability to upgrade from
+  previous versions of Windows to Windows 10. One malware family
+  known to modify these keys is Kovter, a well-known trojan.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\WindowsUpdate', value: 'DisableOSUpgrade'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\WindowsUpdate', value: 'DisableOSUpgrade'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Policies\Microsoft\Windows\WindowsUpdate\OSUpgrade', value: 'ReservationsAllowed'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Policies\Microsoft\Windows\WindowsUpdate\OSUpgrade', value: 'ReservationsAllowed'}
+supported_os: [Windows]
+urls:
+- 'https://www.ghacks.net/2016/01/08/disableosupgrade-prevents-the-upgrade-to-windows-10/'
+- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0517-0524.html'
+---
+name: WindowsUserAccessLogging
+doc: |
+  User Access Logging (UAL) databases.
+
+  UAL is a local data aggregation feature (enabled by default) on Windows
+  Servers 2012 and above, recording client usage by role and product on each
+  system providing the resource. It's typically between 2 and 4 extensible
+  storage engine (ESE) databases ("Current.mdb", "SystemIdentity.mdb, and
+  "<GUID>.mdb").
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%environ_systemroot%%\System32\LogFiles\SUM\*.mdb']
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://forensics.wiki/windows#user-access-logging-ual']
+---
+name: WindowsUserAccountControlSettings
+doc: |
+  Windows User Account Control Settings
+
+  Malware sometimes disables UAC to make it easier to perform
+  actions on an infected machine.
+sources:
+- type: REGISTRY_VALUE
+  attributes:
+    key_value_pairs:
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'EnableLUA'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'EnableLUA'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Policies\System', value: 'ConsentPromptBehaviorAdmin'}
+    - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Policies\System', value: 'ConsentPromptBehaviorAdmin'}
+supported_os: [Windows]
+urls:
+- 'https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-gpsb/958053ae-5397-4f96-977f-b7700ee461ec'
+- 'https://blog.talosintelligence.com/2019/05/threat-roundup-0503-0510.html'
+- 'https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-gpsb/341747f5-6b5d-4d30-85fc-fa1cc04038d4'
+---
 name: WindowsUserAutomaticDestinationsJumpLists
 doc: Windows user AutomaticDestinations Jump Lists.
 sources:
 - type: FILE
   attributes:
     paths: ['%%users.appdata%%\Microsoft\Windows\Recent\AutomaticDestinations\*.automaticDestinations-ms']
     separator: '\'
@@ -3198,27 +3342,23 @@
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
     - 'HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders\*'
     - 'HKEY_USERS\%%users.sid%%\Environment\*'
     - 'HKEY_USERS\%%users.sid%%\Volatile Environment\*'
-provides:
-- users.cookies
-- users.appdata
-- users.personal
-- users.startup
-- users.homedir
-- users.desktop
-- users.internet_cache
-- users.localappdata
-- users.localappdata_low
-- users.recent
-- users.userprofile
-- users.temp
+supported_os: [Windows]
+---
+name: WindowsWebCacheStorageQuotaDatabaseFile
+doc: Windows WebCache storage quota database file (CacheStorage.edb)
+sources:
+- type: FILE
+  attributes:
+    paths: ['%%users.localappdata%%\Packages\*\AppData\CacheStorage\CacheStorage.edb']
+    separator: '\'
 supported_os: [Windows]
 ---
 name: WindowsWinlogonGinaDLL
 doc: Windows Gina DLL replacement.
 sources:
 - type: REGISTRY_VALUE
   attributes:
@@ -3362,24 +3502,46 @@
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\Winlogon\GPExtensions\*', value: ''}
     - {key: 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\Winlogon\GPExtensions\*', value: 'DllName'}
     - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Winlogon\GPExtensions\*', value: ''}
     - {key: 'HKEY_LOCAL_MACHINE\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Winlogon\GPExtensions\*', value: 'DllName'}
 supported_os: [Windows]
 urls: ['https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2']
 ---
+name: WindowsWordWheelQueryRegistryKey
+doc: Keywords searched in from the Windows start menu, potentially resulting in files or folders access or program executions.
+sources:
+- type: REGISTRY_KEY
+  attributes:
+    keys: ['HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\WordWheelQuery\*']
+supported_os: [Windows]
+---
 name: WindowsXMLEventLogApplication
 doc: Application Windows XML Event Log.
 sources:
 - type: FILE
   attributes:
     paths: ['%%environ_systemroot%%\System32\winevt\Logs\Application.evtx']
     separator: '\'
 supported_os: [Windows]
 urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EventLog.html']
 ---
+name: WindowsXMLEventLogPowerShell
+doc: PowerShell Windows XML Event Logs.
+sources:
+- type: FILE
+  attributes:
+    paths:
+    - '%%environ_systemroot%%\System32\winevt\Logs\Microsoft-Windows-PowerShell%4Admin.evtx'
+    - '%%environ_systemroot%%\System32\winevt\Logs\Microsoft-Windows-PowerShell%4Operational.evtx'
+    - '%%environ_systemroot%%\System32\winevt\Logs\PowerShellCore Operational.evtx'
+    - '%%environ_systemroot%%\System32\winevt\Logs\Windows PowerShell.evtx'
+    separator: '\'
+supported_os: [Windows]
+urls: ['https://artifacts-kb.readthedocs.io/en/latest/sources/windows/EventLog.html']
+---
 name: WindowsXMLEventLogSecurity
 doc: Security Windows XML Event Log.
 sources:
 - type: FILE
   attributes:
     paths: ['%%environ_systemroot%%\System32\winevt\Logs\Security.evtx']
     separator: '\'
@@ -3440,86 +3602,7 @@
     - {key: 'HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\WinSock2\Parameters\NameSpace_Catalog5\Catalog_Entries64\*', value: 'LibraryPath'}
 supported_os: [Windows]
 urls:
 - 'https://www.symantec.com/security_response/writeup.jsp?docid=2012-020609-4221-99&tabid=2'
 - 'http://www.nirsoft.net/utils/winsock_service_providers.html'
 - 'https://msdn.microsoft.com/en-us/library/windows/desktop/ms739923(v=vs.85).aspx'
 - 'https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2'
----
-name: WindowsSecuritySettingsDatabases
-doc: Windows security settings databases (secedit.sdb and spsecupd.sdb)
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '%%environ_systemroot%%\security\Database\secedit.sdb'
-    - '%%environ_systemroot%%\security\templates\spsecupd.sdb'
-    separator: '\'
-supported_os: [Windows]
----
-name: WindowsStartupInfo
-doc: |
-  StartupInfo XML files.
-
-  The files include the user account's Security Identifier (SID) in the name
-  and there could be up to 5 per user account. They contain a list of processes
-  that were executed within the first 90 seconds from the time the user logged
-  in. The info includes start time, the full command line and the parent
-  process info, among other things.
-sources:
-- type: FILE
-  attributes:
-    paths: ['%%environ_systemroot%%\System32\WDI\LogFiles\StartupInfo\*.xml']
-    separator: '\'
-supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#startup-info']
----
-name: WindowsTileDataLayerDatabase
-doc: |
-  Windows tile data layer database (vedatamodel.edb)
-
-  The tile data layer database is used to store information about Start Tiles.
-sources:
-- type: FILE
-  attributes:
-    paths: ['%%users.localappdata%%\TileDataLayer\Database\vedatamodel.edb']
-    separator: '\'
-supported_os: [Windows]
-urls: ['https://forensics.wiki/extensible_storage_engine_(ese)_database_file_(edb)_format#tile-data-layer-database']
----
-name: WindowsUpdateLogFile
-doc: Windows Update log files.
-sources:
-- type: FILE
-  attributes:
-    paths:
-    - '%%environ_programdata%%\USOShared\Logs\System\*.etl'
-    - '%%environ_systemroot%%\Logs\CBS\CBS*.log'
-    - '%%environ_systemroot%%\Logs\WindowsUpdate\WindowsUpdate*.etl'
-    separator: '\'
-supported_os: [Windows]
-urls: ['https://learn.microsoft.com/en-us/windows/deployment/update/windows-update-logs']
----
-name: WindowsUserAccessLogging
-doc: |
-  User Access Logging (UAL) databases.
-
-  UAL is a local data aggregation feature (enabled by default) on Windows
-  Servers 2012 and above, recording client usage by role and product on each
-  system providing the resource. It's typically between 2 and 4 extensible
-  storage engine (ESE) databases ("Current.mdb", "SystemIdentity.mdb, and
-  "<GUID>.mdb").
-sources:
-- type: FILE
-  attributes:
-    paths: ['%%environ_systemroot%%\System32\LogFiles\SUM\*.mdb']
-    separator: '\'
-supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#user-access-logging-ual']
----
-name: WindowsWordWheelQueryRegistryKey
-doc: Keywords searched in from the Windows start menu, potentially resulting in files or folders access or program executions.
-sources:
-- type: REGISTRY_KEY
-  attributes:
-    keys: ['HKEY_USERS\%%users.sid%%\Software\Microsoft\Windows\CurrentVersion\Explorer\WordWheelQuery\*']
-supported_os: [Windows]
```

### Comparing `artifacts-20230928/data/windows_dll_hijacking.yaml` & `artifacts-20240518/artifacts/data/windows_dll_hijacking.yaml`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/data/wmi.yaml` & `artifacts-20240518/artifacts/data/wmi.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,32 @@
   accounts which means a large data transfer from an Active Directory server.
   This artifact relies on having the users.username field populated in the knowledge
   base. Unfortunately even limiting by username this query can be slow, and
   this artifact runs it for each user present on the system.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM Win32_UserAccount WHERE name='%%users.username%%'}
-provides: [users.userdomain]
 supported_os: [Windows]
 urls: ['http://msdn.microsoft.com/en-us/library/windows/desktop/aa394507(v=vs.85).aspx']
 ---
 name: WMIAntivirusProduct
 doc: Enumerate the registered antivirus.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM AntivirusProduct, base_object: 'winmgmts:\root\SecurityCenter2'}
 supported_os: [Windows]
 ---
+name: WMICCMRUA
+doc: Enumerate instances of CCM_RecentlyUsedApps.
+sources:
+- type: WMI
+  attributes: {query: SELECT * FROM CCM_RecentlyUsedApps, base_object: 'winmgmts:\root\ccm\SoftwareMeteringAgent'}
+supported_os: [Windows]
+urls: ['https://forensics.wiki/windows#ccm-recentlyusedapps']
+---
 name: WMIComputerSystemProduct
 doc: Computer System Product including Identifiying number queried from WMI.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM Win32_ComputerSystemProduct}
 supported_os: [Windows]
 urls: ['http://msdn.microsoft.com/en-us/library/aa394105(v=vs.85).aspx']
@@ -172,15 +179,14 @@
 
   This artifact relies on having the SID field users.sid populated in the knowledge
   base. We expect it to be collected with WindowsRegistryProfiles to
   supply the rest of the user information.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM Win32_UserProfile WHERE SID='%%users.sid%%'}
-provides: [users.homedir]
 supported_os: [Windows]
 urls: ['http://msdn.microsoft.com/en-us/library/windows/desktop/ee886409(v=vs.85).aspx']
 ---
 name: WMIScheduledTasks
 doc: Scheduled tasks that are registered on the computer via Windows Management Instrumentation (WMI).
 sources:
 - type: WMI
@@ -218,15 +224,7 @@
 ---
 name: WMIVolumeShadowCopies
 doc: A List of Volume Shadow Copies from WMI.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM Win32_ShadowCopy}
 supported_os: [Windows]
----
-name: WMICCMRUA
-doc: Enumerate instances of CCM_RecentlyUsedApps.
-sources:
-- type: WMI
-  attributes: {query: SELECT * FROM CCM_RecentlyUsedApps, base_object: 'winmgmts:\root\ccm\SoftwareMeteringAgent'}
-supported_os: [Windows]
-urls: ['https://forensics.wiki/windows#ccm-recentlyusedapps']
```

### Comparing `artifacts-20230928/docs/conf.py` & `artifacts-20240518/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 autodoc_mock_imports = sorted(modules_to_mock)
 
 # Options for the Sphinx Napoleon extension, which reads Google-style
 # docstrings.
 napoleon_google_docstring = True
 napoleon_numpy_docstring = False
+napoleon_include_init_with_doc = True
 napoleon_include_private_with_doc = False
 napoleon_include_special_with_doc = True
 
 # General information about the project.
 # pylint: disable=redefined-builtin
 project = 'Digital Forensics Artifacts Repository'
 copyright = 'The Digital Forensics Artifacts Repository authors'
```

### Comparing `artifacts-20230928/docs/index.rst` & `artifacts-20240518/docs/index.rst`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/docs/sources/Format-specification.md` & `artifacts-20240518/docs/sources/Format-specification.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 The artifact definition can have the following values:
 
 Value | Description
 --- | ---
 aliases | Optional list of alternate names to identify the artifact definition. Also see: See section: [Name](#name).
 doc | The description (or documentation). A human readable string that describes the artifact definition. See section: [Description](#description).
 name | The name. An unique string that identifies the artifact definition. See section: [Name](#name).
-provides | Optional list of *TODO*
 sources | A list of source definitions. See section: [Sources](#sources).
 supported_os | Optional list that indicates which operating systems the artifact definition applies to. See section: [Supported operating system](#supported-operating-system).
 urls | Optional list of URLs with more contextual information. Ideally the artifact definition links to an article that discusses the artifact in more depth for example on [Digital Forensics Artifact Knowledge Base](https://github.com/ForensicArtifacts/artifacts-kb).
 
 ## Deprecated values
 
 Value | Description
 --- | ---
 conditions | Optional list of conditions that describe when the artifact definition should apply. Note that conditions have been deprecated as of version 20220710.
 labels | Optional list of predefined labels. Note that labels have been deprecated as of version 20220311.
+provides | Optional list of placeholder values that the artifact provides.
 
 ## Name
 
 The name of an artifact definition should be in CamelCase name without spaces.
 
 Prefix platform specific artifact definitions with the name of the operating
 system using "Linux", "MacOS" or "Windows".
@@ -45,15 +45,17 @@
 * prefix with the application name, for example "ChromeHistory".
 * prefix with the name of the subsystem, for example "WMIComputerSystemProduct".
 
 Commonly used prefixes:
 
 Prefix | Description
 --- | ---
+Android | Android operating system specific artifact definition.
 Darwin | Mac OS (or Darwin) operating system specific artifact definition.
+iOS | iOS operating system specific artifact definition.
 Linux | Linux operating system specific artifact definition.
 Shell | Shell user-interface specific artifact definition.
 User | User specific artifact definition.
 Unix | Unix operating system (or POSIX) specific artifact definition.
 Windows | Windows operating system specific artifact definition.
 
 Suffix artifact definitions with the type of artifact, for example are files use
@@ -282,26 +284,28 @@
 
 ## Supported operating system
 
 Since operating system (OS) are a very common constraint, this has been provided
 as a separate option "supported_os" to simplify syntax. For supported_os no
 quotes are required. The currently supported operating systems are:
 
+* Android
 * Darwin (also used for Mac OS X)
+* iOS
 * Linux
 * Windows
 
 ```yaml
-supported_os: [Darwin, Linux, Windows]
+supported_os: [Android, Darwin, iOS, Linux, Windows]
 ```
 
 This can be translated to objectfilter as:
 
 ```yaml
-["os =='Darwin'" OR "os=='Linux'" OR "os == 'Windows'"]
+["os =='Android'" OR "os =='Darwin'" OR "os =='iOS'" "os=='Linux'" OR "os == 'Windows'"]
 ```
 
 ## Parameter expansion and globs
 
 Artifact definitions can use different types of parameters that need to be
 expanded at runtime, such as:
```

### Comparing `artifacts-20230928/docs/sources/api/artifacts.rst` & `artifacts-20240518/docs/sources/api/artifacts.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 artifacts package
 =================
 
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   artifacts.scripts
+
 Submodules
 ----------
 
 artifacts.artifact module
 -------------------------
 
 .. automodule:: artifacts.artifact
```

### Comparing `artifacts-20230928/docs/sources/background/Stats.md` & `artifacts-20240518/docs/sources/background/Stats.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 ## Statistics
 
 The artifact definitions can be found in the
-[data directory](https://github.com/ForensicArtifacts/artifacts/tree/main/data) and the format is described in detail
-in the [Style Guide](https://artifacts.readthedocs.io/en/latest/sources/Format-specification.html).
+[artifacts/data directory](https://github.com/ForensicArtifacts/artifacts/tree/main/artifacts/data) and the format is described
+in detail in the [Style Guide](https://artifacts.readthedocs.io/en/latest/sources/Format-specification.html).
 
-Status of the repository as of 2023-09-28
+Status of the repository as of 2024-05-18
 
 Description | Number
 --- | ---
-Number of artifact definitions: | 801
-Number of file paths: | 2047
+Number of artifact definitions: | 836
+Number of file paths: | 2290
 Number of Windows Registry key paths: | 677
 
 ### Artifact definition source types
 
 Identifier | Number
 --- | ---
-ARTIFACT_GROUP | 47
+ARTIFACT_GROUP | 48
 COMMAND | 10
-FILE | 516
+FILE | 550
 PATH | 28
 REGISTRY_KEY | 57
 REGISTRY_VALUE | 116
 WMI | 27
 
 ### Operating systems
 
 Identifier | Number
 --- | ---
-Darwin | 200
+Darwin | 213
 ESXi | 16
-Linux | 243
-Windows | 367
+Linux | 248
+Windows | 384
```

### Comparing `artifacts-20230928/docs/sources/background/Terminology.md` & `artifacts-20240518/docs/sources/background/Terminology.md`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/docs/sources/background/index.rst` & `artifacts-20240518/docs/sources/background/index.rst`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/docs/sources/user/Installation-instructions.md` & `artifacts-20240518/docs/sources/user/Installation-instructions.md`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 To deactivate the virtualenv run:
 
 ```bash
 deactivate
 ```
 
-## Ubuntu 18.04 and 20.04 LTS
+## Ubuntu 22.04 LTS
 
 To install Forensics Artifacts from the [GIFT Personal Package Archive (PPA)](https://launchpad.net/~gift):
 
 ```bash
 sudo add-apt-repository ppa:gift/stable
 ```
 
@@ -45,22 +45,22 @@
 ## Windows
 
 The [l2tbinaries](https://github.com/log2timeline/l2tbinaries) contains the
 necessary packages for running Forensics Artifacts. l2tbinaries provides the following
 branches:
 
 * main; branch intended for the "packaged release" of Forensics Artifacts and dependencies;
+* staging; branch intended for testing pre-releases of Forensics Artifacts;
 * dev; branch intended for the "development release" of Forensics Artifacts;
 * testing; branch intended for testing newly created packages.
 
 The l2tdevtools project provides [an update script](https://github.com/log2timeline/l2tdevtools/wiki/Update-script)
 to ease the process of keeping the dependencies up to date.
 
-The script requires [pywin32](https://github.com/mhammond/pywin32/releases) and
-[Python WMI](https://pypi.org/project/WMI/).
+The script requires [pywin32](https://github.com/mhammond/pywin32/releases).
 
 To install the release versions of the dependencies run:
 
 ```
 set PYTHONPATH=.
 
 C:\Python38\python.exe tools\update.py --preset artifacts
```

### Comparing `artifacts-20230928/run_tests.py` & `artifacts-20240518/run_tests.py`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/test_data/definitions.json` & `artifacts-20240518/test_data/definitions.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {'1': "{delete: ['provides']}", '2': "{delete: ['provides']}", '3': "{delete: ['provides']}"}*

```diff
@@ -18,17 +18,14 @@
         "urls": [
             "http://www.forensicswiki.org/wiki/Windows_XML_Event_Log_(EVTX)"
         ]
     },
     {
         "doc": "The %AllUsersProfile% environment variable.",
         "name": "AllUsersProfileEnvironmentVariable",
-        "provides": [
-            "environ_allusersprofile"
-        ],
         "sources": [
             {
                 "attributes": {
                     "keys": [
                         "HKEY_LOCAL_MACHINE\\Software\\Microsoft\\Windows NT\\CurrentVersion\\ProfileList\\ProfilesDirectory",
                         "HKEY_LOCAL_MACHINE\\Software\\Microsoft\\Windows NT\\CurrentVersion\\ProfileList\\AllUsersProfile"
                     ]
@@ -42,17 +39,14 @@
         "urls": [
             "http://support.microsoft.com/kb//214653"
         ]
     },
     {
         "doc": "The control set the system is currently using.",
         "name": "CurrentControlSet",
-        "provides": [
-            "current_control_set"
-        ],
         "sources": [
             {
                 "attributes": {
                     "key_value_pairs": [
                         {
                             "key": "HKEY_LOCAL_MACHINE\\SYSTEM\\Select",
                             "value": "Current"
@@ -68,17 +62,14 @@
         "urls": [
             "https://code.google.com/p/winreg-kb/wiki/SystemKeys"
         ]
     },
     {
         "doc": "Get user homedir from Win32_UserProfile based on a known user's SID.\n\nThis artifact relies on having the SID field users.sid populated in the knowledge\nbase. We expect it to be collected with WindowsRegistryProfiles to\nsupply the rest of the user information.\n",
         "name": "WMIProfileUsersHomeDir",
-        "provides": [
-            "users.homedir"
-        ],
         "sources": [
             {
                 "attributes": {
                     "query": "SELECT * FROM Win32_UserProfile WHERE SID='%%users.sid%%'"
                 },
                 "type": "WMI"
             }
```

### Comparing `artifacts-20230928/test_data/definitions.yaml` & `artifacts-20240518/test_data/definitions.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -13,40 +13,37 @@
 doc: The %AllUsersProfile% environment variable.
 sources:
 - type: REGISTRY_KEY
   attributes:
     keys:
     - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList\ProfilesDirectory'
     - 'HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\ProfileList\AllUsersProfile'
-provides: [environ_allusersprofile]
 supported_os: [Windows]
 urls: ['http://support.microsoft.com/kb//214653']
 ---
 name: CurrentControlSet
 doc: The control set the system is currently using.
 sources:
 - type: REGISTRY_VALUE
   attributes:
     key_value_pairs:
     - {key: 'HKEY_LOCAL_MACHINE\SYSTEM\Select', value: 'Current'}
-provides: [current_control_set]
 supported_os: [Windows]
 urls: ['https://code.google.com/p/winreg-kb/wiki/SystemKeys']
 ---
 name: WMIProfileUsersHomeDir
 doc: |
   Get user homedir from Win32_UserProfile based on a known user's SID.
 
   This artifact relies on having the SID field users.sid populated in the knowledge
   base. We expect it to be collected with WindowsRegistryProfiles to
   supply the rest of the user information.
 sources:
 - type: WMI
   attributes: {query: SELECT * FROM Win32_UserProfile WHERE SID='%%users.sid%%'}
-provides: [users.homedir]
 supported_os: [Windows]
 urls: ['http://msdn.microsoft.com/en-us/library/windows/desktop/ee886409(v=vs.85).aspx']
 ---
 name: EventLogs
 doc: Windows Event logs.
 sources:
 - type: ARTIFACT_GROUP
```

### Comparing `artifacts-20230928/tests/reader_test.py` & `artifacts-20240518/tests/reader_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,17 +174,14 @@
     self.assertEqual(key_value_pair['key'], expected_key)
     self.assertEqual(key_value_pair['value'], 'Current')
 
     # Artifact with WMI query source type.
     artifact_definition = artifact_definitions[3]
     self.assertEqual(artifact_definition.name, 'WMIProfileUsersHomeDir')
 
-    expected_provides = sorted(['users.homedir'])
-    self.assertEqual(sorted(artifact_definition.provides), expected_provides)
-
     self.assertEqual(len(artifact_definition.sources), 1)
     source_type = artifact_definition.sources[0]
     self.assertIsNotNone(source_type)
     self.assertEqual(
         source_type.type_indicator, definitions.TYPE_INDICATOR_WMI_QUERY)
 
     expected_query = (
@@ -314,18 +311,16 @@
             artifact_definition)
         self.assertEqual(artifact_definition, artifact_object.AsDict())
 
   def testDefinitionsAsDict(self):
     """Tests the AsDict function."""
     artifact_reader = reader.YamlArtifactsReader()
 
-    artifact_definitions = list(artifact_reader.ReadDirectory('data'))
-
     last_artifact_definition = None
-    for artifact in artifact_definitions:
+    for artifact in artifact_reader.ReadDirectory(self._DATA_PATH):
       try:
         artifact_definition = artifact.AsDict()
       except errors.FormatError:
         error_location = 'At start'
         if last_artifact_definition:
           error_location = f'After: {last_artifact_definition.name:s}'
         self.fail(f'{error_location:s} failed to convert to dict')
```

### Comparing `artifacts-20230928/tests/registry_test.py` & `artifacts-20240518/tests/registry_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 
     artifact_reader = reader.YamlArtifactsReader()
 
     for artifact_definition in artifact_reader.ReadFile(test_file):
       artifact_registry.RegisterDefinition(artifact_definition)
 
     # Make sure the test file got turned into artifacts.
-    self.assertEqual(len(artifact_registry.GetDefinitions()), 7)
+    definitions = list(artifact_registry.GetDefinitions())
+    self.assertEqual(len(definitions), 7)
 
     artifact_definition = artifact_registry.GetDefinitionByName('EventLogs')
     self.assertIsNotNone(artifact_definition)
 
     # Try to register something already registered
     with self.assertRaises(KeyError):
       artifact_registry.RegisterDefinition(artifact_definition)
@@ -71,15 +72,16 @@
     # Deregister
     artifact_registry.DeregisterDefinition(artifact_definition)
 
     # Check it is gone
     with self.assertRaises(KeyError):
       artifact_registry.DeregisterDefinition(artifact_definition)
 
-    self.assertEqual(len(artifact_registry.GetDefinitions()), 6)
+    definitions = list(artifact_registry.GetDefinitions())
+    self.assertEqual(len(definitions), 6)
 
     test_artifact_definition = artifact_registry.GetDefinitionByName(
         'SecurityEventLogEvtxFile')
     self.assertIsNotNone(test_artifact_definition)
 
     self.assertEqual(test_artifact_definition.name, 'SecurityEventLogEvtxFile')
     self.assertEqual(test_artifact_definition.aliases, ['SecurityEventLogEvtx'])
```

### Comparing `artifacts-20230928/tests/source_type_test.py` & `artifacts-20240518/tests/source_type_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/tests/test_lib.py` & `artifacts-20240518/tests/test_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import tempfile
 import unittest
 
 
 class BaseTestCase(unittest.TestCase):
   """The base test case."""
 
-  _DATA_PATH = os.path.join(os.getcwd(), 'data')
+  _DATA_PATH = os.path.join(os.getcwd(), 'artifacts', 'data')
   _TEST_DATA_PATH = os.path.join(os.getcwd(), 'test_data')
 
   # Show full diff results, part of TestCase so does not follow our naming
   # conventions.
   maxDiff = None
 
   def _GetTestFilePath(self, path_segments):
```

### Comparing `artifacts-20230928/tests/validator_test.py` & `artifacts-20240518/tests/validator_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 """Tests for the artifact definitions validator."""
 
 import glob
 import os
 import unittest
 
 from artifacts import errors
-from tools import validator
+from artifacts.scripts import validator
 
 from tests import test_lib
 
 
 class ArtifactDefinitionsValidatorTest(test_lib.BaseTestCase):
   """Class to test the validator."""
 
   def testArtifactDefinitionsValidator(self):
     """Runs the validator over all the YAML artifact definitions files."""
     validator_object = validator.ArtifactDefinitionsValidator()
 
-    for definitions_file in glob.glob(os.path.join('data', '*.yaml')):
+    data_files_glob = os.path.join(self._DATA_PATH, '*.yaml')
+    for definitions_file in glob.glob(data_files_glob):
       result = validator_object.CheckFile(definitions_file)
       self.assertTrue(
           result, msg=f'in definitions file: {definitions_file:s}')
 
     undefined_artifacts = validator_object.GetUndefinedArtifacts()
     if undefined_artifacts:
+      undefined_artifacts = ', '.join(undefined_artifacts)
       raise errors.MissingDependencyError((
           f'Artifacts group referencing undefined artifacts: '
           f'{undefined_artifacts:s}'))
 
   # TODO: add tests that deliberately provide invalid definitions to see
   # if the validator works correctly.
```

### Comparing `artifacts-20230928/tests/writer_test.py` & `artifacts-20240518/tests/writer_test.py`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/tools/stats.py` & `artifacts-20240518/artifacts/scripts/stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-"""Report statistics about the artifact collection."""
+"""Console script to collect statistics about definitions."""
 
 import collections
+import os
 import sys
 import time
 
 from artifacts import definitions
 from artifacts import reader
 
 
@@ -66,15 +67,16 @@
     artifact_reader = reader.YamlArtifactsReader()
     self._os_counts = collections.Counter()
     self._path_count = 0
     self._reg_key_count = 0
     self._source_type_counts = {}
     self._total_count = 0
 
-    for artifact_definition in artifact_reader.ReadDirectory('data'):
+    data_files_path = os.path.join('artifacts', 'data')
+    for artifact_definition in artifact_reader.ReadDirectory(data_files_path):
       sources_supported_os = set()
       for source in artifact_definition.sources:
         self._total_count += 1
         source_type = source.type_indicator
         self._source_type_counts[source_type] = self._source_type_counts.get(
             source_type, 0) + 1
 
@@ -95,42 +97,40 @@
 
       for os_str in sources_supported_os:
         self._os_counts[os_str] += 1
 
   def PrintStats(self):
     """Build stats and print in MarkDown format."""
     data_directory_url = (
-        'https://github.com/ForensicArtifacts/artifacts/tree/main/data')
+        'https://github.com/ForensicArtifacts/artifacts/tree/main/artifacts/'
+        'data')
 
     style_guide_url = (
         'https://artifacts.readthedocs.io/en/latest/sources/'
         'Format-specification.html')
 
     print(f"""## Statistics
 
 The artifact definitions can be found in the
-[data directory]({data_directory_url:s}) and the format is described in detail
-in the [Style Guide]({style_guide_url:s}).
+[artifacts/data directory]({data_directory_url:s}) and the format is described
+in detail in the [Style Guide]({style_guide_url:s}).
 """)
 
     self.BuildStats()
     self.PrintSummaryTable()
     self.PrintSourceTypeTable()
     self.PrintOSTable()
 
 
 def Main():
-  """The main program function.
+  """Entry point of console script to collect statistics about definitions.
 
   Returns:
-    bool: True if successful or False if not.
+    int: exit code that is provided to sys.exit().
   """
   statsbuilder = ArtifactStatistics()
   statsbuilder.PrintStats()
-  return True
+  return 0
 
 
 if __name__ == '__main__':
-  if not Main():
-    sys.exit(1)
-  else:
-    sys.exit(0)
+  sys.exit(Main())
```

### Comparing `artifacts-20230928/tools/validator.py` & `artifacts-20240518/artifacts/scripts/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-"""Tool to validate artifact definitions."""
+"""Console script to validate artifact definitions."""
 
 import argparse
 import glob
+import heapq
 import logging
 import os
 import sys
 
 from artifacts import definitions
 from artifacts import errors
 from artifacts import reader
 from artifacts import registry
 
 
 class ArtifactDefinitionsValidator(object):
   """Artifact definitions validator."""
 
-  LEGACY_PATH = os.path.join('data', 'legacy.yaml')
+  LEGACY_PATH = os.path.join('artifacts', 'data', 'legacy.yaml')
 
   _MACOS_PRIVATE_SUB_PATHS = ('etc', 'tftpboot', 'tmp', 'var')
 
   _SUPPORTED_POSIX_USERS_VARIABLES = [
       '%%users.homedir%%']
 
   _SUPPORTED_WINDOWS_ENVIRONMENT_VARIABLES = [
@@ -439,24 +440,37 @@
 
     Returns:
       bool: True if the file contains valid artifacts definitions.
     """
     result = True
     artifact_reader = reader.YamlArtifactsReader()
 
+    sorted_names = []
+
     try:
       for artifact_definition in artifact_reader.ReadFile(filename):
         try:
           self._artifact_registry.RegisterDefinition(artifact_definition)
         except KeyError:
           logging.warning((
               f'Duplicate artifact definition: {artifact_definition.name:s} in '
               f'file: {filename:s}'))
           result = False
 
+        current_name_lower = artifact_definition.name.lower()
+        heapq.heappush(sorted_names, (
+            current_name_lower, artifact_definition.name))
+
+        last_name_lower, last_name = sorted_names[-1]
+        if last_name_lower != current_name_lower:
+          logging.warning((
+              f'Artifact definition: {last_name:s} and '
+              f'{artifact_definition.name:s} in file: {filename:s} not '
+              f'in sort order'))
+
         artifact_definition_supports_macos = (
             definitions.SUPPORTED_OS_DARWIN in (
                 artifact_definition.supported_os))
         artifact_definition_supports_windows = (
             definitions.SUPPORTED_OS_WINDOWS in (
                 artifact_definition.supported_os))
 
@@ -538,18 +552,18 @@
     Returns:
       set[str]: undefined artifacts names.
     """
     return self._artifact_registry.GetUndefinedArtifacts()
 
 
 def Main():
-  """The main program function.
+  """Entry point of console script to collect statistics about definitions.
 
   Returns:
-    bool: True if successful or False if not.
+    int: exit code that is provided to sys.exit().
   """
   args_parser = argparse.ArgumentParser(
       description='Validates an artifact definitions file.')
 
   args_parser.add_argument(
       'definitions', nargs='?', action='store', metavar='PATH', default=None,
       help=('path of the file or directory that contains the artifact '
@@ -558,37 +572,34 @@
   options = args_parser.parse_args()
 
   if not options.definitions:
     print('Source value is missing.')
     print('')
     args_parser.print_help()
     print('')
-    return False
+    return 1
 
   if not os.path.exists(options.definitions):
     print(f'No such file or directory: {options.definitions:s}')
     print('')
-    return False
+    return 1
 
   validator = ArtifactDefinitionsValidator()
 
   if os.path.isdir(options.definitions):
     print(f'Validating definitions in: {options.definitions:s}/*.yaml')
     result = validator.CheckDirectory(options.definitions)
 
   elif os.path.isfile(options.definitions):
     print(f'Validating definitions in: {options.definitions:s}')
     result = validator.CheckFile(options.definitions)
 
   if not result:
     print('FAILURE')
-    return False
+    return 1
 
   print('SUCCESS')
-  return True
+  return 0
 
 
 if __name__ == '__main__':
-  if not Main():
-    sys.exit(1)
-  else:
-    sys.exit(0)
+  sys.exit(Main())
```

### Comparing `artifacts-20230928/utils/dependencies.py` & `artifacts-20240518/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/utils/pylintrc` & `artifacts-20240518/utils/pylintrc`

 * *Files identical despite different names*

### Comparing `artifacts-20230928/utils/update_release.sh` & `artifacts-20240518/utils/update_release.sh`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 
 VERSION=`date -u +"%Y%m%d"`
 DPKG_DATE=`date -R`
 
 # Update the Python module version.
 sed "s/__version__ = '[0-9]*'/__version__ = '${VERSION}'/" -i artifacts/__init__.py
 
+# Update the version in the setuptools configuration.
+sed "s/version = [0-9]*/version = ${VERSION}/" -i setup.cfg
+
 # Update the version in the dpkg configuration files.
 cat > config/dpkg/changelog << EOT
 artifacts (${VERSION}-1) unstable; urgency=low
 
   * Auto-generated
 
  -- Forensic artifacts <forensicartifacts@googlegroups.com>  ${DPKG_DATE}
 EOT
 
 # Regenerate the statistics documentation.
-PYTHONPATH=. ./tools/stats.py > docs/sources/background/Stats.md
+PYTHONPATH=. ./artifacts/scripts/stats.py > docs/sources/background/Stats.md
 
 # Regenerate the API documentation.
 tox -edocs
 
 exit ${EXIT_SUCCESS};
```


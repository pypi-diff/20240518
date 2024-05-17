# Comparing `tmp/surfactant-0.0.0rc5.tar.gz` & `tmp/surfactant-0.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfactant-0.0.0rc5.tar", last modified: Fri Apr 19 01:26:51 2024, max compression
+gzip compressed data, was "surfactant-0.0.0rc6.tar", last modified: Fri May 17 23:11:55 2024, max compression
```

## Comparing `surfactant-0.0.0rc5.tar` & `surfactant-0.0.0rc6.tar`

### file list

```diff
@@ -1,239 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.370040 surfactant-0.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.338040 surfactant-0.0.0rc5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.338040 surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.338040 surfactant-0.0.0rc5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-04-19 01:26:51.370040 surfactant-0.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/Surfactant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/Surfactant.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/configuration_files.md
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/contribution_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.342040 surfactant-0.0.0rc5/docs/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    32676 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark-250px.png
--rw-r--r--   0 runner    (1001) docker     (127)   117613 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31219 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-light-250px.png
--rw-r--r--   0 runner    (1001) docker     (127)   119482 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/logos/surfactant-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/docs/windows_installer_tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9767 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md
--rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/execinstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)   111741 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/fsfilter.patch
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/docs/windows_installer_tutorial/setupstepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/example-configs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/example-configs/helics-archive-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/example-configs/helics-installprefix-config.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/example-configs/multiple-archives-config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/angrimportfinder/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/angrimportfinder/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/angrimportfinder/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/binary2strings/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/binary2strings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/binary2strings/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/binary2strings/surfactantplugin_binary2strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/checksec.py/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/checksec.py/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/checksec.py/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/checksec.py/surfactantplugin_checksec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/fuzzyhashes/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/fuzzyhashes/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/fuzzyhashes/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/fuzzyhashes/surfactantplugin_fuzzyhashes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.346040 surfactant-0.0.0rc5/plugins/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/syft/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/syft/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/plugins/syft/surfactantplugin_syft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/README-merge_sbom.md
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/merge_additional_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/merge_config.json
--rwxr-xr-x   0 runner    (1001) docker     (127)    21205 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/scripts/merge_sbom.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:26:51.370040 surfactant-0.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/surfactant/
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1583 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 01:26:51.000000 surfactant-0.0.0rc5/surfactant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/surfactant/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/createconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/cmd/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2183 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/fileinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.350040 surfactant-0.0.0rc5/surfactant/filetypeid/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/id_extension.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2304 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/id_hex.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7283 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/filetypeid/id_magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/infoextractors/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/a_out_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/coff_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9202 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/elf_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/java_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/ole_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26619 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/infoextractors/pe_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/input_readers/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/input_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/input_readers/cytrics_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/output/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12782 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/cyclonedx_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/cytrics_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/output/spdx_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/plugin/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/relationships/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.354040 surfactant-0.0.0rc5/surfactant/relationships/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/_internal/posix_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/_internal/windows_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/dotnet_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/elf_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/java_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/relationships/pe_relationship.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/surfactant/sbomtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_analysisdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_sbom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_software.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/surfactant/sbomtypes/_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/cmd/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/cmd/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/cmd/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    16424 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/bin/hello_world
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/ConsoleApp2.dll.config
--rw-r--r--   0 runner    (1001) docker     (127)   147968 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/ConsoleApp2.exe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)    58880 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/hello_world.exe
--rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/testlib.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.358040 surfactant-0.0.0rc5/tests/data/a_out_files/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/big_m68020.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/big_netbsd_i386.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/big_netbsd_sparc.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/little_386.aout
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/a_out_files/little_unknown.aout
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/coff_files/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/coff_files/intel_80386_coff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/java_class_no1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/java_class_no1/HelloWorld.class
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.334040 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    55672 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/bin/hello_world
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)    51128 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/msitest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/msitest_no1/test.msi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/sample_sboms/
--rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/sample_sboms/helics_binaries_sbom.json
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/sample_sboms/helics_libs_sbom.json
--rw-r--r--   0 runner    (1001) docker     (127)    21305 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/sample_sboms/helics_sbom.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data/srectest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data/srectest_no1/HexFile.hex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/App.config
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/ConsoleApp2.csproj
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/Program.cs
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.cs
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.csproj
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.sln
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.362040 surfactant-0.0.0rc5/tests/data_src/java_class_no1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.class
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.jar
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/java_class_no1/helloworld.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/msitest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/hello.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)    16376 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/hello.exe
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/msitest_no1/test.wxs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/hello_world.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/lib/testlib.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/lib/testlib.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/data_src/srectest_no1/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/srectest_no1/BinaryFile.bin
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/srectest_no1/HexFile.hex
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/data_src/srectest_no1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/file_types/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/file_types/test_a_out_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/file_types/test_file_magic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/relationships/
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-19 01:26:40.000000 surfactant-0.0.0rc5/tests/relationships/test_dotnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_elf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_java.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/relationships/test_posix_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:26:51.366040 surfactant-0.0.0rc5/tests/symlink/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-19 01:26:41.000000 surfactant-0.0.0rc5/tests/symlink/test_resolve_links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.359395 surfactant-0.0.0rc6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.359395 surfactant-0.0.0rc6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.359395 surfactant-0.0.0rc6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/Surfactant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/Surfactant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/Surfactant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/Surfactant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/Surfactant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/Surfactant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/Surfactant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/configuration_files.md
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/contribution_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/docs/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    32676 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/logos/surfactant-logo-dark-250px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   117613 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/logos/surfactant-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31219 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/logos/surfactant-logo-light-250px.png
+-rw-r--r--   0 runner    (1001) docker     (127)   119482 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/logos/surfactant-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/docs/windows_installer_tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9767 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/windows_installer_tutorial/execinstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111741 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/windows_installer_tutorial/fsfilter.patch
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/docs/windows_installer_tutorial/setupstepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/example-configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/example-configs/helics-archive-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/example-configs/helics-installprefix-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/example-configs/multiple-archives-config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.363395 surfactant-0.0.0rc6/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/plugins/angrimportfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/angrimportfinder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/angrimportfinder/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/plugins/binary2strings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/binary2strings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/binary2strings/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/binary2strings/surfactantplugin_binary2strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/plugins/checksec.py/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/checksec.py/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/checksec.py/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/checksec.py/surfactantplugin_checksec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/plugins/fuzzyhashes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/fuzzyhashes/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/fuzzyhashes/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/fuzzyhashes/surfactantplugin_fuzzyhashes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/plugins/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/syft/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/syft/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/plugins/syft/surfactantplugin_syft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/README-merge_sbom.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.367395 surfactant-0.0.0rc6/scripts/js_libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/js_libraries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/js_libraries/get_retirejs_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/js_libraries/match_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/merge_additional_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/merge_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21205 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/scripts/merge_sbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.371395 surfactant-0.0.0rc6/surfactant/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1637 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-17 23:11:55.000000 surfactant-0.0.0rc6/surfactant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.371395 surfactant-0.0.0rc6/surfactant/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/cmd/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/cmd/createconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/cmd/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/cmd/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/cmd/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/cmd/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2183 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/fileinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.371395 surfactant-0.0.0rc6/surfactant/filetypeid/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/filetypeid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/filetypeid/id_extension.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2304 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/filetypeid/id_hex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7283 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/filetypeid/id_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.371395 surfactant-0.0.0rc6/surfactant/infoextractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/a_out_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/coff_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9202 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/elf_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/java_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/js_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22407 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/js_library_patterns.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/ole_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26619 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/infoextractors/pe_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.371395 surfactant-0.0.0rc6/surfactant/input_readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/input_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/input_readers/cytrics_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.375395 surfactant-0.0.0rc6/surfactant/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/output/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12817 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/output/cyclonedx_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/output/cytrics_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/output/spdx_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.375395 surfactant-0.0.0rc6/surfactant/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/plugin/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.375395 surfactant-0.0.0rc6/surfactant/relationships/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.375395 surfactant-0.0.0rc6/surfactant/relationships/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/_internal/posix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/_internal/windows_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/dotnet_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/elf_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/java_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/relationships/pe_relationship.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.375395 surfactant-0.0.0rc6/surfactant/sbomtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_analysisdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_sbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/sbomtypes/_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/surfactant/web-files/
+-rw-r--r--   0 runner    (1001) docker     (127)    31347 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/surfactant/web-files/ui.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.355395 surfactant-0.0.0rc6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/cmd/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/cmd/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/cmd/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.351395 surfactant-0.0.0rc6/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.351395 surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16424 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/bin/hello_world
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/ConsoleApp2.dll.config
+-rw-r--r--   0 runner    (1001) docker     (127)   147968 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/ConsoleApp2.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.351395 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/bin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.351395 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/bin/Debug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/Windows_dll_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)    58880 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/Windows_dll_test_no1/hello_world.exe
+-rw-r--r--   0 runner    (1001) docker     (127)    53248 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/Windows_dll_test_no1/testlib.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/a_out_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/a_out_files/big_m68020.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/a_out_files/big_netbsd_i386.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/a_out_files/big_netbsd_sparc.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/a_out_files/little_386.aout
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/a_out_files/little_unknown.aout
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/coff_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/coff_files/intel_80386_coff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/java_class_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/java_class_no1/HelloWorld.class
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.351395 surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55672 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/bin/hello_world
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51128 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.379396 surfactant-0.0.0rc6/tests/data/msitest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/msitest_no1/test.msi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data/sample_sboms/
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/sample_sboms/helics_binaries_sbom.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/sample_sboms/helics_libs_sbom.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21305 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/sample_sboms/helics_sbom.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data/srectest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data/srectest_no1/HexFile.hex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/App.config
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/ConsoleApp2.csproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/Program.cs
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/hello.cs
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/hello.csproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/hello.sln
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data_src/java_class_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/java_class_no1/HelloWorld.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/java_class_no1/HelloWorld.jar
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/java_class_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/java_class_no1/helloworld.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data_src/msitest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/msitest_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/msitest_no1/hello.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16376 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/msitest_no1/hello.exe
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/msitest_no1/test.wxs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.383396 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/hello_world.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/lib/testlib.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/lib/testlib.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/tests/data_src/srectest_no1/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/srectest_no1/BinaryFile.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/srectest_no1/HexFile.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/data_src/srectest_no1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/tests/file_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/file_types/test_a_out_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/file_types/test_file_magic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/tests/relationships/
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/relationships/test_dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/relationships/test_elf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/relationships/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/relationships/test_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/relationships/test_posix_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:11:55.387396 surfactant-0.0.0rc6/tests/symlink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-17 23:11:46.000000 surfactant-0.0.0rc6/tests/symlink/test_resolve_links.py
```

### Comparing `surfactant-0.0.0rc5/.github/CODE_OF_CONDUCT.md` & `surfactant-0.0.0rc6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md` & `surfactant-0.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.github/ISSUE_TEMPLATE/feature_request.md` & `surfactant-0.0.0rc6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.github/PULL_REQUEST_TEMPLATE.md` & `surfactant-0.0.0rc6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.github/workflows/pytest.yml` & `surfactant-0.0.0rc6/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.github/workflows/release.yml` & `surfactant-0.0.0rc6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.gitignore` & `surfactant-0.0.0rc6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 tests/symlink/test_dir/
 # setuptools_scm auto-generated version file
 surfactant/_version.py
 
 # Test directories
 tests/symlink/test_dir/
 
+# Result files from web UI
+results/
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `surfactant-0.0.0rc5/.gitlab-ci.yml` & `surfactant-0.0.0rc6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/.pre-commit-config.yaml` & `surfactant-0.0.0rc6/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 exclude: ^(.gitignore|generate_sbom.py|extract_file_info.py|pe_info.py)
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.7
+    rev: v0.4.4
     hooks:
       # Run the linter
       - id: ruff
         args: [ --fix ]
       # Run the formatter
       - id: ruff-format
   - repo: https://github.com/pycqa/pylint
```

### Comparing `surfactant-0.0.0rc5/.readthedocs.yaml` & `surfactant-0.0.0rc6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/CONTRIBUTING.md` & `surfactant-0.0.0rc6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/LICENSE` & `surfactant-0.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/NOTICE` & `surfactant-0.0.0rc6/NOTICE`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/PKG-INFO` & `surfactant-0.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Surfactant
-Version: 0.0.0rc5
+Version: 0.0.0rc6
 Summary: Modular framework to gather file information, analyze dependencies, and generate an SBOM
 Author-email: Ryan Mast <mast9@llnl.gov>, Levi Lloyd <lloyd27@llnl.gov>, Micaela Gallegos <gallegos31@llnl.gov>, Alexander Armstrong <armstrong48@llnl.gov>, Shayna Kapadia <kapadia2@llnl.gov>
 Maintainer-email: Ryan Mast <mast9@llnl.gov>
 License: MIT License
 Project-URL: Homepage, https://github.com/LLNL/Surfactant
 Project-URL: Discussions, https://github.com/LLNL/Surfactant/discussions
 Project-URL: Documentation, https://surfactant.readthedocs.io/en/latest/
@@ -31,23 +31,24 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: dataclasses_json
 Requires-Dist: pyelftools
 Requires-Dist: pefile
-Requires-Dist: dnfile
+Requires-Dist: dnfile==0.14.1
 Requires-Dist: olefile
 Requires-Dist: defusedxml
 Requires-Dist: spdx-tools==0.8.*
-Requires-Dist: cyclonedx-python-lib==6.4.4
+Requires-Dist: cyclonedx-python-lib==7.3.4
 Requires-Dist: pluggy
 Requires-Dist: click
 Requires-Dist: javatools>=1.6.0
 Requires-Dist: loguru
+Requires-Dist: flask
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `surfactant-0.0.0rc5/README.md` & `surfactant-0.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/Surfactant.egg-info/PKG-INFO` & `surfactant-0.0.0rc6/Surfactant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Surfactant
-Version: 0.0.0rc5
+Version: 0.0.0rc6
 Summary: Modular framework to gather file information, analyze dependencies, and generate an SBOM
 Author-email: Ryan Mast <mast9@llnl.gov>, Levi Lloyd <lloyd27@llnl.gov>, Micaela Gallegos <gallegos31@llnl.gov>, Alexander Armstrong <armstrong48@llnl.gov>, Shayna Kapadia <kapadia2@llnl.gov>
 Maintainer-email: Ryan Mast <mast9@llnl.gov>
 License: MIT License
 Project-URL: Homepage, https://github.com/LLNL/Surfactant
 Project-URL: Discussions, https://github.com/LLNL/Surfactant/discussions
 Project-URL: Documentation, https://surfactant.readthedocs.io/en/latest/
@@ -31,23 +31,24 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: dataclasses_json
 Requires-Dist: pyelftools
 Requires-Dist: pefile
-Requires-Dist: dnfile
+Requires-Dist: dnfile==0.14.1
 Requires-Dist: olefile
 Requires-Dist: defusedxml
 Requires-Dist: spdx-tools==0.8.*
-Requires-Dist: cyclonedx-python-lib==6.4.4
+Requires-Dist: cyclonedx-python-lib==7.3.4
 Requires-Dist: pluggy
 Requires-Dist: click
 Requires-Dist: javatools>=1.6.0
 Requires-Dist: loguru
+Requires-Dist: flask
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
```

### Comparing `surfactant-0.0.0rc5/Surfactant.egg-info/SOURCES.txt` & `surfactant-0.0.0rc6/Surfactant.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -68,33 +68,39 @@
 plugins/syft/README.md
 plugins/syft/pyproject.toml
 plugins/syft/surfactantplugin_syft.py
 scripts/README-merge_sbom.md
 scripts/merge_additional_metadata.py
 scripts/merge_config.json
 scripts/merge_sbom.py
+scripts/js_libraries/README.md
+scripts/js_libraries/get_retirejs_db.py
+scripts/js_libraries/match_javascript.py
 surfactant/__init__.py
 surfactant/__main__.py
 surfactant/_version.py
 surfactant/config.py
 surfactant/fileinfo.py
 surfactant/cmd/cli.py
 surfactant/cmd/createconfig.py
 surfactant/cmd/generate.py
 surfactant/cmd/merge.py
 surfactant/cmd/stat.py
+surfactant/cmd/ui.py
 surfactant/filetypeid/__init__.py
 surfactant/filetypeid/id_extension.py
 surfactant/filetypeid/id_hex.py
 surfactant/filetypeid/id_magic.py
 surfactant/infoextractors/__init__.py
 surfactant/infoextractors/a_out_file.py
 surfactant/infoextractors/coff_file.py
 surfactant/infoextractors/elf_file.py
 surfactant/infoextractors/java_file.py
+surfactant/infoextractors/js_file.py
+surfactant/infoextractors/js_library_patterns.json
 surfactant/infoextractors/ole_file.py
 surfactant/infoextractors/pe_file.py
 surfactant/input_readers/__init__.py
 surfactant/input_readers/cytrics_reader.py
 surfactant/output/__init__.py
 surfactant/output/csv_writer.py
 surfactant/output/cyclonedx_writer.py
@@ -116,14 +122,15 @@
 surfactant/sbomtypes/_hardware.py
 surfactant/sbomtypes/_observation.py
 surfactant/sbomtypes/_provenance.py
 surfactant/sbomtypes/_relationship.py
 surfactant/sbomtypes/_sbom.py
 surfactant/sbomtypes/_software.py
 surfactant/sbomtypes/_system.py
+surfactant/web-files/ui.html
 tests/cmd/test_cli.py
 tests/cmd/test_generate.py
 tests/cmd/test_merge.py
 tests/data/ELF_shared_obj_test_no1/bin/hello_world
 tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so
 tests/data/NET_app_config_test_no1/ConsoleApp2.dll.config
 tests/data/NET_app_config_test_no1/ConsoleApp2.exe
```

### Comparing `surfactant-0.0.0rc5/docs/Makefile` & `surfactant-0.0.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/basic_usage.md` & `surfactant-0.0.0rc6/docs/basic_usage.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/conf.py` & `surfactant-0.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/configuration_files.md` & `surfactant-0.0.0rc6/docs/configuration_files.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/getting_started.md` & `surfactant-0.0.0rc6/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/index.md` & `surfactant-0.0.0rc6/docs/index.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark-250px.png` & `surfactant-0.0.0rc6/docs/logos/surfactant-logo-dark-250px.png`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/logos/surfactant-logo-dark.png` & `surfactant-0.0.0rc6/docs/logos/surfactant-logo-dark.png`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/logos/surfactant-logo-light-250px.png` & `surfactant-0.0.0rc6/docs/logos/surfactant-logo-light-250px.png`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/logos/surfactant-logo-light.png` & `surfactant-0.0.0rc6/docs/logos/surfactant-logo-light.png`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/make.bat` & `surfactant-0.0.0rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/plugins.md` & `surfactant-0.0.0rc6/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md` & `surfactant-0.0.0rc6/docs/windows_installer_tutorial/AutomatedInstallerWorkflowSetup.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/windows_installer_tutorial/execinstaller.py` & `surfactant-0.0.0rc6/docs/windows_installer_tutorial/execinstaller.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/windows_installer_tutorial/fsfilter.patch` & `surfactant-0.0.0rc6/docs/windows_installer_tutorial/fsfilter.patch`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/docs/windows_installer_tutorial/setupstepper.py` & `surfactant-0.0.0rc6/docs/windows_installer_tutorial/setupstepper.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/README.md` & `surfactant-0.0.0rc6/plugins/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/angrimportfinder/README.md` & `surfactant-0.0.0rc6/plugins/angrimportfinder/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/angrimportfinder/pyproject.toml` & `surfactant-0.0.0rc6/plugins/angrimportfinder/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py` & `surfactant-0.0.0rc6/plugins/angrimportfinder/surfactantplugin_angrimportfinder.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/binary2strings/README.md` & `surfactant-0.0.0rc6/plugins/binary2strings/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/binary2strings/pyproject.toml` & `surfactant-0.0.0rc6/plugins/binary2strings/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/binary2strings/surfactantplugin_binary2strings.py` & `surfactant-0.0.0rc6/plugins/binary2strings/surfactantplugin_binary2strings.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/checksec.py/README.md` & `surfactant-0.0.0rc6/plugins/checksec.py/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/checksec.py/pyproject.toml` & `surfactant-0.0.0rc6/plugins/checksec.py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/checksec.py/surfactantplugin_checksec.py` & `surfactant-0.0.0rc6/plugins/checksec.py/surfactantplugin_checksec.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/fuzzyhashes/README.md` & `surfactant-0.0.0rc6/plugins/fuzzyhashes/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/fuzzyhashes/pyproject.toml` & `surfactant-0.0.0rc6/plugins/fuzzyhashes/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/fuzzyhashes/surfactantplugin_fuzzyhashes.py` & `surfactant-0.0.0rc6/plugins/fuzzyhashes/surfactantplugin_fuzzyhashes.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/syft/README.md` & `surfactant-0.0.0rc6/plugins/syft/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/syft/pyproject.toml` & `surfactant-0.0.0rc6/plugins/syft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/plugins/syft/surfactantplugin_syft.py` & `surfactant-0.0.0rc6/plugins/syft/surfactantplugin_syft.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/pyproject.toml` & `surfactant-0.0.0rc6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,23 +38,24 @@
     "Topic :: Utilities",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "dataclasses_json",
     "pyelftools",
     "pefile",
-    "dnfile",
+    "dnfile==0.14.1",
     "olefile",
     "defusedxml",
     "spdx-tools==0.8.*",
-    "cyclonedx-python-lib==6.4.4",
+    "cyclonedx-python-lib==7.3.4",
     "pluggy",
     "click",
     "javatools>=1.6.0",
-    "loguru"
+    "loguru",
+    "flask"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 dev = ["build", "pre-commit"]
 docs = ["sphinx", "myst-parser"]
```

### Comparing `surfactant-0.0.0rc5/scripts/README-merge_sbom.md` & `surfactant-0.0.0rc6/scripts/README-merge_sbom.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/scripts/merge_additional_metadata.py` & `surfactant-0.0.0rc6/scripts/merge_additional_metadata.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/scripts/merge_sbom.py` & `surfactant-0.0.0rc6/scripts/merge_sbom.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/__main__.py` & `surfactant-0.0.0rc6/surfactant/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from loguru import logger
 
 from surfactant.cmd.cli import add, edit, find
 from surfactant.cmd.createconfig import create_config
 from surfactant.cmd.generate import sbom as generate
 from surfactant.cmd.merge import merge_command
 from surfactant.cmd.stat import stat
+from surfactant.cmd.ui import ui
 
 
 @click.group()
 @click.version_option(
     importlib.metadata.version("surfactant"),
     "--version",
     "-v",
@@ -53,14 +54,15 @@
 
 # Main Commands
 main.add_command(generate)
 main.add_command(version)
 main.add_command(stat)
 main.add_command(merge_command)
 main.add_command(create_config)
+main.add_command(ui)
 
 # CLI Subcommands
 cli.add_command(find)
 cli.add_command(edit)
 cli.add_command(add)
 
 if __name__ == "__main__":
```

### Comparing `surfactant-0.0.0rc5/surfactant/cmd/cli.py` & `surfactant-0.0.0rc6/surfactant/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/cmd/createconfig.py` & `surfactant-0.0.0rc6/surfactant/cmd/createconfig.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/cmd/generate.py` & `surfactant-0.0.0rc6/surfactant/cmd/generate.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/cmd/merge.py` & `surfactant-0.0.0rc6/surfactant/cmd/merge.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/cmd/stat.py` & `surfactant-0.0.0rc6/surfactant/cmd/stat.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/fileinfo.py` & `surfactant-0.0.0rc6/surfactant/fileinfo.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/filetypeid/id_extension.py` & `surfactant-0.0.0rc6/surfactant/filetypeid/id_extension.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/filetypeid/id_hex.py` & `surfactant-0.0.0rc6/surfactant/filetypeid/id_hex.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/filetypeid/id_magic.py` & `surfactant-0.0.0rc6/surfactant/filetypeid/id_magic.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/infoextractors/a_out_file.py` & `surfactant-0.0.0rc6/surfactant/infoextractors/a_out_file.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/infoextractors/coff_file.py` & `surfactant-0.0.0rc6/surfactant/infoextractors/coff_file.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/infoextractors/elf_file.py` & `surfactant-0.0.0rc6/surfactant/infoextractors/elf_file.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/infoextractors/java_file.py` & `surfactant-0.0.0rc6/surfactant/infoextractors/java_file.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/infoextractors/ole_file.py` & `surfactant-0.0.0rc6/surfactant/infoextractors/ole_file.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/infoextractors/pe_file.py` & `surfactant-0.0.0rc6/surfactant/infoextractors/pe_file.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/output/csv_writer.py` & `surfactant-0.0.0rc6/surfactant/output/csv_writer.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/output/cyclonedx_writer.py` & `surfactant-0.0.0rc6/surfactant/output/cyclonedx_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pathlib
 from collections.abc import Iterable
 from typing import Dict, List, Optional, Tuple
 
 import cyclonedx.output
-from cyclonedx.model import HashAlgorithm, HashType, OrganizationalEntity, Tool
+from cyclonedx.model import HashAlgorithm, HashType, Tool
 from cyclonedx.model.bom import Bom, BomMetaData
 from cyclonedx.model.bom_ref import BomRef
 from cyclonedx.model.component import Component, ComponentType
+from cyclonedx.model.contact import OrganizationalEntity
 from cyclonedx.model.dependency import Dependency
 
 import surfactant.plugin
 from surfactant import __version__ as surfactant_version
 from surfactant.sbomtypes import SBOM, Software, System
```

### Comparing `surfactant-0.0.0rc5/surfactant/output/spdx_writer.py` & `surfactant-0.0.0rc6/surfactant/output/spdx_writer.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/plugin/hookspecs.py` & `surfactant-0.0.0rc6/surfactant/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/plugin/manager.py` & `surfactant-0.0.0rc6/surfactant/plugin/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     # don't want all these imports as part of the file-level scope
     from surfactant.filetypeid import id_extension, id_hex, id_magic
     from surfactant.infoextractors import (
         a_out_file,
         coff_file,
         elf_file,
         java_file,
+        js_file,
         ole_file,
         pe_file,
     )
     from surfactant.input_readers import cytrics_reader
     from surfactant.output import (
         csv_writer,
         cyclonedx_writer,
@@ -40,14 +41,15 @@
         id_magic,
         id_hex,
         id_extension,
         a_out_file,
         coff_file,
         elf_file,
         java_file,
+        js_file,
         pe_file,
         ole_file,
         dotnet_relationship,
         elf_relationship,
         java_relationship,
         pe_relationship,
         csv_writer,
```

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/__init__.py` & `surfactant-0.0.0rc6/surfactant/relationships/__init__.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/_internal/posix_utils.py` & `surfactant-0.0.0rc6/surfactant/relationships/_internal/posix_utils.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/_internal/windows_utils.py` & `surfactant-0.0.0rc6/surfactant/relationships/_internal/windows_utils.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/dotnet_relationship.py` & `surfactant-0.0.0rc6/surfactant/relationships/dotnet_relationship.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/elf_relationship.py` & `surfactant-0.0.0rc6/surfactant/relationships/elf_relationship.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/java_relationship.py` & `surfactant-0.0.0rc6/surfactant/relationships/java_relationship.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/relationships/pe_relationship.py` & `surfactant-0.0.0rc6/surfactant/relationships/pe_relationship.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/__init__.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_analysisdata.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_analysisdata.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_hardware.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_hardware.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_observation.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_observation.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_provenance.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_provenance.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_sbom.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_sbom.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_software.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_software.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/surfactant/sbomtypes/_system.py` & `surfactant-0.0.0rc6/surfactant/sbomtypes/_system.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/cmd/test_cli.py` & `surfactant-0.0.0rc6/tests/cmd/test_cli.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/cmd/test_generate.py` & `surfactant-0.0.0rc6/tests/cmd/test_generate.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/cmd/test_merge.py` & `surfactant-0.0.0rc6/tests/cmd/test_merge.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/bin/hello_world` & `surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/bin/hello_world`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so` & `surfactant-0.0.0rc6/tests/data/ELF_shared_obj_test_no1/lib/libtestlib.so`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/ConsoleApp2.exe` & `surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/ConsoleApp2.exe`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll` & `surfactant-0.0.0rc6/tests/data/NET_app_config_test_no1/bin/Debug/net6.0/hello.dll`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/hello_world.exe` & `surfactant-0.0.0rc6/tests/data/Windows_dll_test_no1/hello_world.exe`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/Windows_dll_test_no1/testlib.dll` & `surfactant-0.0.0rc6/tests/data/Windows_dll_test_no1/testlib.dll`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/java_class_no1/HelloWorld.class` & `surfactant-0.0.0rc6/tests/data/java_class_no1/HelloWorld.class`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/bin/hello_world` & `surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/bin/hello_world`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib` & `surfactant-0.0.0rc6/tests/data/mach_o_dylib_test_no1/lib/libtestlib.dylib`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/msitest_no1/test.msi` & `surfactant-0.0.0rc6/tests/data/msitest_no1/test.msi`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/sample_sboms/helics_binaries_sbom.json` & `surfactant-0.0.0rc6/tests/data/sample_sboms/helics_binaries_sbom.json`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/sample_sboms/helics_libs_sbom.json` & `surfactant-0.0.0rc6/tests/data/sample_sboms/helics_libs_sbom.json`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data/sample_sboms/helics_sbom.json` & `surfactant-0.0.0rc6/tests/data/sample_sboms/helics_sbom.json`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln` & `surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/ConsoleApp2.sln`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/README.md` & `surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/NET_app_config_test_no1/hello.sln` & `surfactant-0.0.0rc6/tests/data_src/NET_app_config_test_no1/hello.sln`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/README.md` & `surfactant-0.0.0rc6/tests/data_src/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.class` & `surfactant-0.0.0rc6/tests/data_src/java_class_no1/HelloWorld.class`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/java_class_no1/HelloWorld.jar` & `surfactant-0.0.0rc6/tests/data_src/java_class_no1/HelloWorld.jar`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/msitest_no1/hello.exe` & `surfactant-0.0.0rc6/tests/data_src/msitest_no1/hello.exe`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/msitest_no1/test.wxs` & `surfactant-0.0.0rc6/tests/data_src/msitest_no1/test.wxs`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt` & `surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/data_src/native_shared_lib_test_no1/README.md` & `surfactant-0.0.0rc6/tests/data_src/native_shared_lib_test_no1/README.md`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/file_types/test_a_out_files.py` & `surfactant-0.0.0rc6/tests/file_types/test_a_out_files.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/file_types/test_file_magic.py` & `surfactant-0.0.0rc6/tests/file_types/test_file_magic.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/relationships/test_dotnet.py` & `surfactant-0.0.0rc6/tests/relationships/test_dotnet.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/relationships/test_elf.py` & `surfactant-0.0.0rc6/tests/relationships/test_elf.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/relationships/test_java.py` & `surfactant-0.0.0rc6/tests/relationships/test_java.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/relationships/test_pe.py` & `surfactant-0.0.0rc6/tests/relationships/test_pe.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/relationships/test_posix_utils.py` & `surfactant-0.0.0rc6/tests/relationships/test_posix_utils.py`

 * *Files identical despite different names*

### Comparing `surfactant-0.0.0rc5/tests/symlink/test_resolve_links.py` & `surfactant-0.0.0rc6/tests/symlink/test_resolve_links.py`

 * *Files identical despite different names*


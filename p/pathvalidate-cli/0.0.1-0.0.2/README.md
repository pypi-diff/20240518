# Comparing `tmp/pathvalidate-cli-0.0.1.tar.gz` & `tmp/pathvalidate_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathvalidate-cli-0.0.1.tar", last modified: Sun Sep 17 09:44:04 2023, max compression
+gzip compressed data, was "pathvalidate_cli-0.0.2.tar", last modified: Sat May 18 08:25:25 2024, max compression
```

## Comparing `pathvalidate-cli-0.0.1.tar` & `pathvalidate_cli-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-17 09:44:04.882371 pathvalidate-cli-0.0.1/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      161 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     3507 2023-09-17 09:44:04.882371 pathvalidate-cli-0.0.1/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     2110 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-17 09:44:04.872371 pathvalidate-cli-0.0.1/pathvalidate_cli/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/pathvalidate_cli/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/pathvalidate_cli/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)       72 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/pathvalidate_cli/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)      989 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/pathvalidate_cli/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7766 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/pathvalidate_cli/main.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-17 09:44:04.882371 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     3507 2023-09-17 09:44:04.000000 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      624 2023-09-17 09:44:04.000000 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-09-17 09:44:04.000000 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       59 2023-09-17 09:44:04.000000 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      110 2023-09-17 09:44:04.000000 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-09-17 09:44:04.000000 pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1015 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-17 09:44:04.882371 pathvalidate-cli-0.0.1/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       68 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       34 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-09-17 09:44:04.882371 pathvalidate-cli-0.0.1/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2559 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-09-17 09:44:04.882371 pathvalidate-cli-0.0.1/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     1073 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/test/test_error_subcommand.py
--rw-r--r--   0 toor      (1000) toor      (1000)      460 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/test/test_help.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1065 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/test/test_sanitize_subcommand.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1159 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/test/test_validate_subcommand.py
--rw-r--r--   0 toor      (1000) toor      (1000)      999 2023-09-17 09:43:35.000000 pathvalidate-cli-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.484754 pathvalidate_cli-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.480754 pathvalidate_cli-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.480754 pathvalidate_cli-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-18 08:25:25.484754 pathvalidate_cli-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.480754 pathvalidate_cli-0.0.2/pathvalidate_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/pathvalidate_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/pathvalidate_cli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/pathvalidate_cli/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/pathvalidate_cli/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/pathvalidate_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.484754 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-18 08:25:25.000000 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-18 08:25:25.000000 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 08:25:25.000000 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-18 08:25:25.000000 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-18 08:25:25.000000 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 08:25:25.000000 pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.484754 pathvalidate_cli-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 08:25:25.484754 pathvalidate_cli-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:25:25.484754 pathvalidate_cli-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/test/test_error_subcommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/test/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/test/test_sanitize_subcommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/test/test_validate_subcommand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-18 08:24:56.000000 pathvalidate_cli-0.0.2/tox.ini
```

### Comparing `pathvalidate-cli-0.0.1/LICENSE` & `pathvalidate_cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pathvalidate-cli-0.0.1/PKG-INFO` & `pathvalidate_cli-0.0.2/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,64 @@
-Metadata-Version: 2.1
-Name: pathvalidate-cli
-Version: 0.0.1
-Summary: pathvalidate-cli is a command line interface for pathvalidate library.
-Home-page: https://github.com/thombashi/pathvalidate-cli
-Author: Tsuyoshi Hombashi
-Author-email: tsuyoshi.hombashi@gmail.com
-License: MIT License
-Project-URL: Source, https://github.com/thombashi/pathvalidate-cli
-Project-URL: Tracker, https://github.com/thombashi/pathvalidate-cli/issues
-Keywords: file,path,validate,sanitize
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Terminals
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: click<9,>=6.2
-Requires-Dist: loguru<1,>=0.4.1
-Requires-Dist: msgfy<1,>=0.2
-Requires-Dist: pathvalidate<4,>=3.2.0
-Provides-Extra: test
-Requires-Dist: pytest>=7; extra == "test"
-Requires-Dist: pytest-md-report>=0.4.1; extra == "test"
-
 .. contents:: **pathvalidate-cli**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
 
-pathvalidate-cli is a command line interface for `pathvalidate <https://github.com/thombashi/pathvalidate>`__ library.
+``pathvalidate-cli`` is a command line interface for `pathvalidate <https://github.com/thombashi/pathvalidate>`__ library.
+The tool can sanitize/validate strings such as file-names/file-paths.
+
+|PyPI pkg ver| |Supported Python ver| |CI status| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pathvalidate-cli.svg
+    :target: https://badge.fury.io/py/pathvalidate-cli
+    :alt: PyPI package version
+
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pathvalidate-cli.svg
+    :target: https://pypi.org/project/pathvalidate-cli
+    :alt: Supported Python versions
+
+.. |CI status| image:: https://github.com/thombashi/pathvalidate-cli/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/pathvalidate-cli/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/pathvalidate-cli/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pathvalidate-cli/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
 
 
 Installation
 ============================================
 ::
 
     pip install pathvalidate-cli
 
 
 Usage
 ============================================
 
+Sanitize file paths
+--------------------------------------------
+
 ::
 
     $ pathvalidate sanitize 'fi:l*e/p"a?t>h|.t<xt'
     file/path.txt
     $ pathvalidate --filename sanitize 'fi:l*e/p"a?t>h|.t<xt'
     filepath.txt
 
+Validate file paths
+--------------------------------------------
+
+::
+
+    $ pathvalidate validate file/path.txt
+    $ 
     $ pathvalidate validate 'fi:l*e/p"a?t>h|.t<xt'
     [PV1100] invalid characters found: invalids=(':', '*', '"', '?', '>', '|', '<'), value='fi:l*e/p"a?t>h|.t<xt', platform=Windows
 
 Command Help
 --------------------------------------------
 
 ::
@@ -73,27 +67,35 @@
 
     Options:
       --version                     Show the version and exit.
       --debug                       For debug print.
       -q, --quiet                   Suppress execution log messages.
       --filename                    Consider inputs as filenames.
       --max-len, --max-bytes BYTES  Maximum byte counts of file paths. -1: same
-                                    value with the platform limitation.  [default:
+                                    value as the platform limitation.  [default:
                                     -1]
-      --platform PLATFORM           Execution platform name (case-insensitive).
-                                    Valid platform specifiers are
-                                    Linux/Windows/macOS. Valid special values are:
-                                    POSIX, universal (a) auto: automatically
-                                    detects the execution platform. (b) universal:
-                                    platform independent.  [default: universal]
+      --platform PLATFORM           Target platform name (case-insensitive). Valid
+                                    platform specifiers are Linux/Windows/macOS.
+                                    Valid special values are: auto, universal,
+                                    POSIX (a) auto: automatically detects the
+                                    execution platform. (b) universal: platform
+                                    independent. (c) POSIX: POSIX-compliant
+                                    platform.  [default: universal]
+      --security-check              Enable security checks.
       -v, --verbose                 Verbosity level  [default: 0]
       -h, --help                    Show this message and exit.
 
     Commands:
       error     Print error reasons.
       sanitize  Sanitize file paths.
       validate  Validate file paths.
 
 
 Dependencies
 ============================================
 Python 3.8+
+
+
+Related Project
+============================================
+
+- `pathvalidate <https://github.com/thombashi/pathvalidate>`__
```

### Comparing `pathvalidate-cli-0.0.1/pathvalidate_cli/_logger.py` & `pathvalidate_cli-0.0.2/pathvalidate_cli/_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from loguru import logger
 
 from ._const import MODULE_NAME
 
 
 class LogLevel:
-    DEBUG: Final[str] = "DEBUG"
-    INFO: Final[str] = "INFO"
-    QUIET: Final[str] = "QUIET"
+    DEBUG: Final = "DEBUG"
+    INFO: Final = "INFO"
+    QUIET: Final = "QUIET"
 
 
 logger.disable(MODULE_NAME)
 
 
 def set_logger(is_enable: bool, propagation_depth: int = 1) -> None:
     if is_enable:
```

### Comparing `pathvalidate-cli-0.0.1/pathvalidate_cli/main.py` & `pathvalidate_cli-0.0.2/pathvalidate_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from pathvalidate.error import ErrorReason, ValidationError
 
 from .__version__ import __version__
 from ._const import MODULE_NAME
 from ._logger import LogLevel, initialize_logger, logger
 
 
-COMMAND_EPILOG: Final[str] = dedent(
+COMMAND_EPILOG: Final = dedent(
     f"""\
     Issue tracker: https://github.com/thombashi/{MODULE_NAME}/issues
     """
 )
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"], obj={})
 
 
@@ -73,31 +73,32 @@
 @click.option(
     "--max-len",
     "--max-bytes",
     metavar="BYTES",
     type=int,
     show_default=True,
     default=-1,
-    help="Maximum byte counts of file paths. -1: same value with the platform limitation.",
+    help="Maximum byte counts of file paths. -1: same value as the platform limitation.",
 )
 @click.option(
     "--platform",
     metavar="PLATFORM",
     default="universal",
     show_default=True,
     help=" ".join(
         [
-            "Execution platform name (case-insensitive).",
+            "Target platform name (case-insensitive).",
             "Valid platform specifiers are Linux/Windows/macOS.",
-            "Valid special values are: POSIX, universal\n",
+            "Valid special values are: auto, universal, POSIX\n",
         ]
     )
     + """\
     (a) auto: automatically detects the execution platform.
     (b) universal: platform independent.
+    (c) POSIX: POSIX-compliant platform.
 """,
 )
 @click.option(
     "-v", "--verbose", "verbosity_level", help="Verbosity level", show_default=True, count=True
 )
 @click.pass_context
 def cmd(
```

### Comparing `pathvalidate-cli-0.0.1/pathvalidate_cli.egg-info/SOURCES.txt` & `pathvalidate_cli-0.0.2/pathvalidate_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+.gitignore
 LICENSE
 MANIFEST.in
+Makefile
 README.rst
 pyproject.toml
 setup.py
 tox.ini
+.github/dependabot.yml
+.github/workflows/ci.yml
+.github/workflows/release.yml
 pathvalidate_cli/__init__.py
 pathvalidate_cli/__version__.py
 pathvalidate_cli/_const.py
 pathvalidate_cli/_logger.py
 pathvalidate_cli/main.py
 pathvalidate_cli.egg-info/PKG-INFO
 pathvalidate_cli.egg-info/SOURCES.txt
```

### Comparing `pathvalidate-cli-0.0.1/setup.py` & `pathvalidate_cli-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os.path
 from typing import Dict, Final, Type
 
 import setuptools
 
 
-MODULE_NAME: Final[str] = "pathvalidate-cli"
-MODULE_NAME_UNDERSCORE: Final[str] = MODULE_NAME.replace("-", "_")
-REPOSITORY_URL: Final[str] = f"https://github.com/thombashi/{MODULE_NAME:s}"
-REQUIREMENT_DIR: Final[str] = "requirements"
-ENCODING: Final[str] = "utf8"
+MODULE_NAME: Final = "pathvalidate-cli"
+MODULE_NAME_UNDERSCORE: Final = MODULE_NAME.replace("-", "_")
+REPOSITORY_URL: Final = f"https://github.com/thombashi/{MODULE_NAME:s}"
+REQUIREMENT_DIR: Final = "requirements"
+ENCODING: Final = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
 def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
@@ -32,26 +32,26 @@
     INSTALL_REQUIRES = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description="pathvalidate-cli is a command line interface for pathvalidate library.",
     include_package_data=True,
     keywords=["file", "path", "validate", "sanitize"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     project_urls={
+        "Changelog": f"{REPOSITORY_URL:s}/releases",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
     python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require={
         "test": TESTS_REQUIRES,
@@ -63,14 +63,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Terminals",
         "Topic :: Utilities",
     ],
     cmdclass=get_release_command_class(),
     entry_points={"console_scripts": [f"pathvalidate={MODULE_NAME_UNDERSCORE}.main:cmd"]},
 )
```

### Comparing `pathvalidate-cli-0.0.1/test/test_error_subcommand.py` & `pathvalidate_cli-0.0.2/test/test_error_subcommand.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-cli-0.0.1/test/test_sanitize_subcommand.py` & `pathvalidate_cli-0.0.2/test/test_sanitize_subcommand.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-cli-0.0.1/test/test_validate_subcommand.py` & `pathvalidate_cli-0.0.2/test/test_validate_subcommand.py`

 * *Files identical despite different names*

### Comparing `pathvalidate-cli-0.0.1/tox.ini` & `pathvalidate_cli-0.0.2/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 [tox]
 envlist =
-    py{38,39,310,311}
+    py{38,39,310,311,312}
     build
     cov
     fmt
     lint
 
 [testenv]
 passenv = *
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
-    build>=0.10
+    build>=1
     twine
     wheel
 commands =
     python -m build
     twine check dist/*.whl dist/*.tar.gz
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
 [testenv:cov]
-passenv = *
+passenv = GITHUB_*
 extras =
     test
 deps =
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv} test/
     coverage report -m
 
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
-    black>=23.1
     isort>=5
+    ruff>=0.3.5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
-    black setup.py test pathvalidate_cli
+    ruff format
 
 [testenv:lint]
-skip_install = true
+extras =
+    test
 deps =
-    black>=23.1
+    codespell
     mypy>=1
-    pylama>=8.4.1
-    types-click
+    releasecmd
+    pyright>=1.1
+    ruff>=0.3.5
 commands =
-    black --check setup.py test pathvalidate_cli
+    codespell pathvalidate_cli test README.rst -q2 --check-filenames
     mypy pathvalidate_cli setup.py
-    pylama
+    pyright
+    ruff format --check
+    ruff check
+
+[testenv:release]
+deps =
+    releasecmd
+commands =
+    python setup.py release --sign --skip-uploading --verbose
```


# Comparing `tmp/oooenv-0.2.3.tar.gz` & `tmp/oooenv-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooenv-0.2.3.tar", max compression
+gzip compressed data, was "oooenv-0.2.4.tar", max compression
```

## Comparing `oooenv-0.2.3.tar` & `oooenv-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-05-10 19:38:38.177533 oooenv-0.2.3/LICENSE
--rw-r--r--   0        0        0     2681 2024-05-10 19:38:38.177533 oooenv-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-05-10 19:38:38.177533 oooenv-0.2.3/oooenv/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cli/__init__.py
--rw-r--r--   0        0        0     8225 2024-05-10 19:46:21.704519 oooenv-0.2.3/oooenv/cli/main.py
--rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/__init__.py
--rw-r--r--   0        0        0     1181 2024-05-10 20:04:23.963339 oooenv-0.2.3/oooenv/cmds/install.py
--rw-r--r--   0        0        0     5767 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/manage_env_cfg.py
--rw-r--r--   0        0        0     4627 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/uno_lnk.py
--rw-r--r--   0        0        0     1216 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/cmds/updater.py
--rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/__init__.py
--rw-r--r--   0        0        0     3573 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/local_paths.py
--rw-r--r--   0        0        0      773 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/sys_info.py
--rw-r--r--   0        0        0    10430 2024-05-10 19:38:38.181533 oooenv-0.2.3/oooenv/utils/uno_paths.py
--rw-r--r--   0        0        0     1419 2024-05-10 20:04:34.035423 oooenv-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3791 1970-01-01 00:00:00.000000 oooenv-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-10 19:38:38.177533 oooenv-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2681 2024-05-10 19:38:38.177533 oooenv-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.177533 oooenv-0.2.4/oooenv/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/cli/__init__.py
+-rw-r--r--   0        0        0     8066 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/cmds/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5103 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
+-rw-r--r--   0        0        0     2841 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
+-rw-r--r--   0        0        0      883 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/cmds/install.py
+-rw-r--r--   0        0        0     5767 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/cmds/manage_env_cfg.py
+-rw-r--r--   0        0        0     4627 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/cmds/uno_lnk.py
+-rw-r--r--   0        0        0     1216 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/cmds/updater.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/utils/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3710 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     1146 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
+-rw-r--r--   0        0        0     5887 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     3708 2024-05-18 19:14:09.727605 oooenv-0.2.4/oooenv/utils/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0     3573 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/utils/local_paths.py
+-rw-r--r--   0        0        0      773 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/utils/sys_info.py
+-rw-r--r--   0        0        0    10430 2024-05-10 19:38:38.181533 oooenv-0.2.4/oooenv/utils/uno_paths.py
+-rw-r--r--   0        0        0     1419 2024-05-18 19:12:51.459144 oooenv-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3791 1970-01-01 00:00:00.000000 oooenv-0.2.4/PKG-INFO
```

### Comparing `oooenv-0.2.3/LICENSE` & `oooenv-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/README.md` & `oooenv-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/oooenv/cli/main.py` & `oooenv-0.2.4/oooenv/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,30 +206,31 @@
         action="store_true",
         dest="show_version",
         default=False,
     )
     parser.add_argument(
         "-e",
         "--editable",
-        help="Install a project in editable mode from the local project path. Similar to pip install -e <package>. Defaults to . (the current package itself), but the root folder of any package source can be given (relative or absolute).",
-        action="store",
-        dest="editable_package_path",
-        default=".",
+        help="Install a project in editable mode from the local project path. Similar to pip install -e .",
+        action="store_true",
+        dest="editable",
+        default=False,
     )
 
 
 def _args_action_global(a_parser: argparse.ArgumentParser, args: argparse.Namespace) -> str | None:
     # sourcery skip: assign-if-exp, reintroduce-else
     if args.show_version:
         # return importlib.metadata.version(__package__ or __name__)
         return importlib.metadata.version("oooenv")
-    if args.editable_package_path:
-        if result := install.pip_e(args.editable_package_path):
+    if args.editable:
+        if result := install.pip_e():
             return result
-        return "Install Failed for unknown reason."
+        else:
+            return "Install Failed for unknown reason."
     return None
 
 
 # endregion process arg command for global
 
 # endregion parser
```

### Comparing `oooenv-0.2.3/oooenv/cmds/install.py` & `oooenv-0.2.4/oooenv/cmds/install.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from __future__ import annotations
 from pathlib import Path
+import os
 from ..utils import local_paths
 
 
-def pip_e(package_path: str = ".") -> str:
+def pip_e() -> str:
     """
     Install root path in virtual environment site-packages directory.
 
     Basically the same thing as ``pip -e .`` but without the need for pip.
 
-    Args:
-        package_path (str, optional): Path to package. Defaults to ``"."``.
-
     Returns:
         str: Message indicating success or failure. Empty string on failure.
     """
     try:
         root_path = Path(local_paths.get_virtual_env_path()).parent
-        if package_path and package_path != ".":
-            root_path = root_path / package_path
-
-        if not root_path.exists():
-            return f"No such package path as: {str(root_path)}"
         site_packages_dir = local_paths.get_site_packages_dir()
         if site_packages_dir is None:
             return ""
         file_name = site_packages_dir / f"{root_path.name.replace('.', '_').replace(' ', '_')}.pth"
         with open(file_name, "w") as f:
             f.write(str(root_path))
         return f"Created file: {file_name}"
```

### Comparing `oooenv-0.2.3/oooenv/cmds/manage_env_cfg.py` & `oooenv-0.2.4/oooenv/cmds/manage_env_cfg.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/oooenv/cmds/uno_lnk.py` & `oooenv-0.2.4/oooenv/cmds/uno_lnk.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/oooenv/cmds/updater.py` & `oooenv-0.2.4/oooenv/cmds/updater.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/oooenv/utils/local_paths.py` & `oooenv-0.2.4/oooenv/utils/local_paths.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/oooenv/utils/sys_info.py` & `oooenv-0.2.4/oooenv/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/oooenv/utils/uno_paths.py` & `oooenv-0.2.4/oooenv/utils/uno_paths.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.3/pyproject.toml` & `oooenv-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooenv"
-version = "0.2.3"
+version = "0.2.4"
 description = "Configures a project python environment for LibreOffice UNO."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 keywords = ["libreoffice", "macro", "uno", "ooouno", "venv"]
 homepage = "https://github.com/Amourspirit/python_oooenv"
 documentation = "https://github.com/Amourspirit/python_oooenv"
 repository = "https://github.com/Amourspirit/python_oooenv"
 license = "MIT"
```

### Comparing `oooenv-0.2.3/PKG-INFO` & `oooenv-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooenv
-Version: 0.2.3
+Version: 0.2.4
 Summary: Configures a project python environment for LibreOffice UNO.
 Home-page: https://github.com/Amourspirit/python_oooenv
 License: MIT
 Keywords: libreoffice,macro,uno,ooouno,venv
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
```


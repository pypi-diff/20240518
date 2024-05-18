# Comparing `tmp/omuplugin_obssync-0.3.2.tar.gz` & `tmp/omuplugin_obssync-0.4.2.tar.gz`

## Comparing `omuplugin_obssync-0.3.2.tar` & `omuplugin_obssync-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/__main__.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/src/omuplugin_obssync/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/src/omuplugin_obssync/__main__.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/src/omuplugin_obssync/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/src/omuplugin_obssync/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/README.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 omuplugin_obssync-0.4.2/PKG-INFO
```

### Comparing `omuplugin_obssync-0.3.2/src/omuplugin_obssync/plugin.py` & `omuplugin_obssync-0.4.2/src/omuplugin_obssync/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import Any, TypedDict
 
 import psutil
 from omu.identifier import Identifier
 from omuserver.server import Server
 
-IDENTIFIER = Identifier("cc.omuchat", "plugin-obssync")
+IDENTIFIER = Identifier("com.omuapps", "plugin-obssync")
 
 
 class obs:
     launch_command: list[str] | None = None
     cwd: Path | None = None
```

### Comparing `omuplugin_obssync-0.3.2/pyproject.toml` & `omuplugin_obssync-0.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_obssync"
-version = "0.3.2"
+version = "0.4.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9", "psutil>=5.9.8"]
+dependencies = ["loguru>=0.7.2", "omu_chat>=0.1.9", "psutil>=5.9.8"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_obssync:plugin"
 
 [build-system]
```


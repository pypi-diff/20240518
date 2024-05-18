# Comparing `tmp/coherent_build-0.6.0.tar.gz` & `tmp/coherent_build-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.6.0.tar", last modified: Thu May  9 19:59:35 2024, max compression
+gzip compressed data, was "coherent_build-0.7.0.tar", last modified: Sat May 18 18:26:52 2024, max compression
```

## Comparing `coherent_build-0.6.0.tar` & `coherent_build-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-09 19:59:33.401990 coherent_build-0.6.0/
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.6.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     5660 2024-05-09 19:51:56.014871 coherent_build-0.6.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.6.0/__init__.py.orig
--rw-r--r--   0 jaraco     (501) staff       (20)      492 2024-05-09 19:24:41.199168 coherent_build-0.6.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     4238 2024-05-09 19:58:21.109403 coherent_build-0.6.0/discovery.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-09 19:59:33.402047 coherent_build-0.6.0/pyproject.toml
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.6.0/system.toml
--rw-r--r--   0        0        0      611 2024-05-09 19:59:35.832361 coherent_build-0.6.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-18 18:21:00.880212 coherent_build-0.7.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.7.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)      268 2024-05-18 18:04:29.832212 coherent_build-0.7.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.7.0/__init__.py.orig
+-rw-r--r--   0 jaraco     (501) staff       (20)      492 2024-05-09 19:24:41.199168 coherent_build-0.7.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     5482 2024-05-18 18:04:29.832430 coherent_build-0.7.0/backend.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     4363 2024-05-18 18:23:06.275278 coherent_build-0.7.0/discovery.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-18 18:20:50.401743 coherent_build-0.7.0/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.7.0/system.toml
+-rw-r--r--   0        0        0      611 2024-05-18 18:26:52.048515 coherent_build-0.7.0/PKG-INFO
```

### Comparing `coherent_build-0.6.0/__init__.py` & `coherent_build-0.7.0/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-__requires__ = [
-    'wheel',
-    'pip-run',
-    'setuptools_scm',
-    'build',
-    'git-fame',
-    'jaraco.context',
-    'requests',
-    'packaging',
-    'jaraco.functools',
-]
-
 import functools
 import importlib.metadata
 import io
 import os
 import pathlib
 import posixpath
 import re
@@ -77,26 +65,14 @@
         super().__init__(path=path, name=zip_name)
 
 
 def _normalize(name):
     return packaging.utils.canonicalize_name(name).replace('-', '_')
 
 
-def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
-    metadata = Metadata.from_sdist() or Metadata.discover()
-    root = metadata['Name'].replace('.', '/')
-    filename = pathlib.Path(wheel_directory) / f'{metadata.id}-py3-none-any.whl'
-    with WheelFile(filename, 'w') as zf:
-        for info in wheel_walk(Wheel(root)):
-            zf.write(info.path, arcname=info.name)
-        for md_name, contents in make_wheel_metadata(metadata):
-            zf.writestr(md_name, contents)
-    return str(filename)
-
-
 def make_wheel_metadata(metadata):
     dist_info = f'{metadata.id}.dist-info'
     yield f'{dist_info}/METADATA', metadata.render()
     wheel_md = Metadata({
         'Wheel-Version': '1.0',
         'Generator': 'coherent.build',
         'Root-Is-Purelib': 'true',
@@ -192,14 +168,26 @@
     info = tarfile.TarInfo(f'{metadata.id}/PKG-INFO')
     file = io.BytesIO(metadata.render().encode('utf-8'))
     info.size = len(file.getbuffer())
     info.mtime = time.time()
     return info, file
 
 
+def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
+    metadata = Metadata.from_sdist() or Metadata.discover()
+    root = metadata['Name'].replace('.', '/')
+    filename = pathlib.Path(wheel_directory) / f'{metadata.id}-py3-none-any.whl'
+    with WheelFile(filename, 'w') as zf:
+        for info in wheel_walk(Wheel(root)):
+            zf.write(info.path, arcname=info.name)
+        for md_name, contents in make_wheel_metadata(metadata):
+            zf.writestr(md_name, contents)
+    return str(filename)
+
+
 def build_sdist(sdist_directory, config_settings=None):
     metadata = Metadata.discover()
     filename = pathlib.Path(sdist_directory) / f'{metadata.id}.tar.gz'
     with tarfile.open(filename, 'w:gz') as tf:
         tf.add(pathlib.Path(), filter=SDist(metadata.id))
         tf.addfile(*make_sdist_metadata(metadata))
     return str(filename)
```

### Comparing `coherent_build-0.6.0/__init__.py.orig` & `coherent_build-0.7.0/__init__.py.orig`

 * *Files identical despite different names*

### Comparing `coherent_build-0.6.0/discovery.py` & `coherent_build-0.7.0/discovery.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """
     url = subprocess.check_output(
         ['git', 'remote', 'get-url', 'origin'],
         text=True,
         encoding='utf-8',
     )
     _, _, tail = url.strip().rpartition('/')
-    return tail
+    return tail.removesuffix('.git')
 
 
 def name_from_path():
     """
     >>> name_from_vcs()
     'coherent.build'
     """
@@ -98,15 +98,18 @@
     '>= 3...'
     """
     owner = 'python'
     repo = 'cpython'
     url = f'https://api.github.com/repos/{owner}/{repo}/branches'
     branches = requests.get(url).json()
     # cheat and grab the first branch, which is the oldest supported Python version
-    return f'>= {branches[0]["name"]}'
+    try:
+        return f'>= {branches[0]["name"]}'
+    except KeyError as err:
+        raise RuntimeError(f"Unexpected {branches=}") from err
 
 
 def read_deps():
     """
     Read deps from ``__init__.py``.
     """
     return scripts.DepsReader.search(['__init__.py'])
```

### Comparing `coherent_build-0.6.0/PKG-INFO` & `coherent_build-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coherent.build
-Version: 0.6.0
+Version: 0.7.0
 Author-Email: "Jason R. Coombs" <jaraco@jaraco.com>
 Summary: A zero-config Python project build backend
 Requires-Python: >= 3.8
 Requires-Dist: wheel
 Requires-Dist: pip-run
 Requires-Dist: setuptools_scm
 Requires-Dist: build
```


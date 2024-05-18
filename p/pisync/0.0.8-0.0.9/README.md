# Comparing `tmp/pisync-0.0.8.tar.gz` & `tmp/pisync-0.0.9.tar.gz`

## Comparing `pisync-0.0.8.tar` & `pisync-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pisync-0.0.8/Makefile
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 pisync-0.0.8/.github/workflows/main.yaml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pisync-0.0.8/examples/run_backups.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/__about__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/config/__init__.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/config/base_config.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/config/local_config.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/config/remote_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 pisync-0.0.8/src/pisync/util/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pisync-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pisync-0.0.8/tests/test_backup.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 pisync-0.0.8/tests/test_local_config.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pisync-0.0.8/tests/test_remote_config.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pisync-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.8/LICENSE
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pisync-0.0.8/README.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 pisync-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 pisync-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pisync-0.0.9/Makefile
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 pisync-0.0.9/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pisync-0.0.9/examples/run_backups.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/__about__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/config/__init__.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/config/base_config.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/config/local_config.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/config/remote_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 pisync-0.0.9/src/pisync/util/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pisync-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 pisync-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 pisync-0.0.9/tests/test_backup.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 pisync-0.0.9/tests/test_local_config.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pisync-0.0.9/tests/test_remote_config.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pisync-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pisync-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pisync-0.0.9/README.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 pisync-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 pisync-0.0.9/PKG-INFO
```

### Comparing `pisync-0.0.8/Makefile` & `pisync-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/.github/workflows/main.yaml` & `pisync-0.0.9/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/examples/run_backups.py` & `pisync-0.0.9/examples/run_backups.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/src/pisync/config/base_config.py` & `pisync-0.0.9/src/pisync/config/base_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/src/pisync/config/local_config.py` & `pisync-0.0.9/src/pisync/config/local_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         else:
             self.log_file = log_file
         self.link_dir = str(Path(self.destination_dir) / "latest")
         self._optionless_rsync_arguments = [
             "--delete",  # delete extraneous files from dest dirs
             "--archive",  # archive mode is -rlptgoD (no -A,-X,-U,-N,-H)
             "--verbose",  # increase verbosity
+            "--info=stats3",
         ]
 
     def is_symlink(self, path: str) -> bool:
         return Path(path).is_symlink()
 
     def file_exists(self, path: str) -> bool:
         return Path(path).exists()
```

### Comparing `pisync-0.0.8/src/pisync/config/remote_config.py` & `pisync-0.0.9/src/pisync/config/remote_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             "--delete",  # delete extraneous files from dest dirs
             "--archive",  # archive mode is -rlptgoD (no -A,-X,-U,-N,-H)
             # NOTE: these options are linux specific and do not work on the
             # macOS version of rsync.
             # "--acls",       # preserve ACLs (implies --perms)
             # "--xattrs",     # preserve extended attributes
             "--verbose",  # increase verbosity
+            "--info=stats3",
         ]
 
     def _ensure_dir_exists_locally(self, path: str):
         _path = Path(path)
         if not _path.exists():
             msg = f"{_path} does not exist"
             raise InvalidPathError(msg)
```

### Comparing `pisync-0.0.8/src/pisync/util/__init__.py` & `pisync-0.0.9/src/pisync/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/tests/conftest.py` & `pisync-0.0.9/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 def optionless_arguments():
     return [
         "--delete",
         "--archive",
         # "--acls",
         # "--xattrs",
         "--verbose",
+        "--info=stats3",
     ]
 
 
 @pytest.fixture(scope="function")
 def scratch_file_system(tmp_path):
     file1 = tmp_path / "file1"
     file2 = tmp_path / "file2"
```

### Comparing `pisync-0.0.8/tests/test_backup.py` & `pisync-0.0.9/tests/test_backup.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/tests/test_local_config.py` & `pisync-0.0.9/tests/test_local_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/tests/test_remote_config.py` & `pisync-0.0.9/tests/test_remote_config.py`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/LICENSE` & `pisync-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/README.md` & `pisync-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/pyproject.toml` & `pisync-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pisync-0.0.8/PKG-INFO` & `pisync-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisync
-Version: 0.0.8
+Version: 0.0.9
 Summary: Minimal incremental backup script using rsync 
 Project-URL: Documentation, https://github.com/erietz/pisync#readme
 Project-URL: Issues, https://github.com/erietz/pisync/issues
 Project-URL: Source, https://github.com/erietz/pisync
 Author-email: erietz <ewrietz@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```


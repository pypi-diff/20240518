# Comparing `tmp/bin_package_manager-2.2.7.tar.gz` & `tmp/bin_package_manager-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bin_package_manager-2.2.7.tar", max compression
+gzip compressed data, was "bin_package_manager-2.2.8.tar", max compression
```

## Comparing `bin_package_manager-2.2.7.tar` & `bin_package_manager-2.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      219 2024-04-11 09:05:50.998865 bin_package_manager-2.2.7/bpm/__init__.py
--rw-r--r--   0        0        0       65 2024-02-15 09:27:57.497385 bin_package_manager-2.2.7/bpm/__main__.py
--rw-r--r--   0        0        0     4279 2024-04-14 23:31:08.910941 bin_package_manager-2.2.7/bpm/cli.py
--rw-r--r--   0        0        0     7215 2024-04-16 03:12:08.318003 bin_package_manager-2.2.7/bpm/command.py
--rw-r--r--   0        0        0    19223 2024-05-07 10:16:01.248459 bin_package_manager-2.2.7/bpm/install/__init__.py
--rw-r--r--   0        0        0     4103 2024-02-19 09:51:08.195821 bin_package_manager-2.2.7/bpm/lib/windowspathadder.py
--rw-r--r--   0        0        0     9268 2024-05-03 07:57:34.768541 bin_package_manager-2.2.7/bpm/search/__init__.py
--rw-r--r--   0        0        0     6901 2024-05-07 10:14:40.683232 bin_package_manager-2.2.7/bpm/search/arch_select.py
--rw-r--r--   0        0        0     4586 2024-04-16 03:12:06.131815 bin_package_manager-2.2.7/bpm/storage.py
--rw-r--r--   0        0        0     2941 2024-04-16 11:05:28.888260 bin_package_manager-2.2.7/bpm/utils/__init__.py
--rw-r--r--   0        0        0      548 2024-04-12 12:37:08.951081 bin_package_manager-2.2.7/bpm/utils/constants.py
--rw-r--r--   0        0        0     1025 2024-02-20 12:24:21.046111 bin_package_manager-2.2.7/bpm/utils/exceptions.py
--rw-r--r--   0        0        0     1126 2024-04-21 03:06:57.655022 bin_package_manager-2.2.7/bpm/utils/input.py
--rw-r--r--   0        0        0     1087 2024-02-04 04:59:52.630709 bin_package_manager-2.2.7/LICENSE
--rw-r--r--   0        0        0     1038 2024-05-07 10:21:06.638758 bin_package_manager-2.2.7/pyproject.toml
--rw-r--r--   0        0        0     4074 2024-04-14 23:31:08.909941 bin_package_manager-2.2.7/README.md
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 bin_package_manager-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-03 15:14:27.236806 bin_package_manager-2.2.8/LICENSE
+-rw-r--r--   0        0        0     4162 2024-05-18 06:35:52.484297 bin_package_manager-2.2.8/README.md
+-rw-r--r--   0        0        0      211 2024-04-12 12:39:24.674496 bin_package_manager-2.2.8/bpm/__init__.py
+-rw-r--r--   0        0        0       61 2024-02-14 06:21:44.497403 bin_package_manager-2.2.8/bpm/__main__.py
+-rw-r--r--   0        0        0     4138 2024-04-14 10:57:29.327187 bin_package_manager-2.2.8/bpm/cli.py
+-rw-r--r--   0        0        0     7005 2024-04-14 11:16:00.299639 bin_package_manager-2.2.8/bpm/command.py
+-rw-r--r--   0        0        0    18907 2024-05-18 07:13:18.364473 bin_package_manager-2.2.8/bpm/install/__init__.py
+-rw-r--r--   0        0        0     4103 2024-02-19 11:56:44.850635 bin_package_manager-2.2.8/bpm/lib/windowspathadder.py
+-rw-r--r--   0        0        0     9388 2024-05-18 07:07:16.211350 bin_package_manager-2.2.8/bpm/search/__init__.py
+-rw-r--r--   0        0        0     7272 2024-05-18 06:58:34.213212 bin_package_manager-2.2.8/bpm/search/arch_select.py
+-rw-r--r--   0        0        0     4449 2024-04-12 12:39:24.674496 bin_package_manager-2.2.8/bpm/storage.py
+-rw-r--r--   0        0        0     2806 2024-05-18 06:35:52.487630 bin_package_manager-2.2.8/bpm/utils/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-12 12:39:24.674496 bin_package_manager-2.2.8/bpm/utils/constants.py
+-rw-r--r--   0        0        0      988 2024-02-21 10:21:37.512797 bin_package_manager-2.2.8/bpm/utils/exceptions.py
+-rw-r--r--   0        0        0     1079 2024-05-18 06:35:52.487630 bin_package_manager-2.2.8/bpm/utils/input.py
+-rw-r--r--   0        0        0      952 2024-05-18 07:14:57.456022 bin_package_manager-2.2.8/pyproject.toml
+-rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 bin_package_manager-2.2.8/PKG-INFO
```

### Comparing `bin_package_manager-2.2.7/bpm/command.py` & `bin_package_manager-2.2.8/bpm/command.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-import logging as log
-from copy import copy
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from urllib.parse import urlparse
-
-from .install import auto_install, download_and_extract, extract, remove
-from .search import RepoHandler
-from .storage import repo_group
-from .utils import check_root, error_exit, set_dry_run, trace
-from .utils.constants import BIN_PATH, WINDOWS
-from .utils.exceptions import RepoNotFoundError
-
-
-def parse_name_or_url(name_or_url: str) -> tuple[str, bool]:
-    """
-    Parse the name or url of a package.
-    `Returns`: a tuple with two elements: first is the true name, second is the flag of whether it is a url.
-    """
-    test_parse = urlparse(name_or_url)
-    if test_parse.netloc == "github.com":
-        return RepoHandler.get_info_by_url(name_or_url)[1], True
-    return name_or_url, False
-
-
-def download_and_install(args, repo: RepoHandler, rename=True):
-    try:
-        with TemporaryDirectory() as tmp_dir:
-            tmp_dir = Path(tmp_dir)
-            if args.local:
-                with Path(args.local).open("rb") as f:
-                    main_path = extract(f, tmp_dir)
-            else:
-                main_path = download_and_extract(repo.asset, tmp_dir)
-            auto_install(repo, main_path, rename=rename)
-    except Exception as e:
-        raise e
-
-
-def cli_install(args):
-    if args.interactive and args.quiet:
-        log.error("Cannot use both --interactive and --quiet.")
-        exit(1)
-    if args.quiet:
-        log.getLogger().setLevel(log.WARNING)
-    if args.dry_run:
-        set_dry_run()
-    else:
-        check_root()
-    if args.local and len(args.packages) > 1:
-        log.error(
-            "Cannot install multiple packages from local. Please install them separately."
-        )
-        exit(1)
-    for package in args.packages:
-        real_name, is_url = parse_name_or_url(package)
-        if not args.dry_run and repo_group.find_repo(real_name)[1]:
-            log.info(f"{real_name} is already installed.")
-            continue
-
-        # search
-        try:
-            if is_url:
-                repo = (
-                    RepoHandler(
-                        real_name,
-                        prefer_gnu=args.prefer_gnu,
-                        one_bin=args.one_bin,
-                        asset_filter=args.filter,
-                    )
-                    .set_by_url(package)
-                    .with_bin_name(args.bin_name)
-                )
-            else:
-                repo = RepoHandler(
-                    package,
-                    prefer_gnu=args.prefer_gnu,
-                    one_bin=args.one_bin,
-                    asset_filter=args.filter,
-                ).with_bin_name(args.bin_name)
-                if not args.local:
-                    repo.ask(quiet=args.quiet, sort=args.sort)
-            if not args.local:
-                repo.get_asset(interactive=args.interactive)
-        except Exception as e:
-            log.error(f"Failed on searching `{package}`: {e}")
-            trace()
-            exit(1)
-
-        # install
-        try:
-            download_and_install(args, repo)
-            print(f"Successfully installed `{repo.name}`.")
-            if WINDOWS:
-                bins = copy(repo.file_list)
-                bins = filter(lambda x: x.endswith(".lnk"), bins)
-                bins = map(lambda x: Path(x).stem, bins)
-                bins = map(lambda x: f"`{x}`", bins)
-                print(
-                    f"You can press `Win+r`, enter {', '.join(bins)} to start software, or execute in cmd."
-                )
-            if not args.dry_run:
-                repo_group.insert_repo(repo)
-        except Exception as e:
-            log.error(f"Failed to install `{repo.name}`: {e}")
-            trace()
-            log.error("Restoring...")
-            # rollback.
-            remove(repo.file_list)
-            error_exit("Files restored. Exiting...")
-
-
-def cli_remove(args):
-    check_root()
-    failed = []
-    for package in args.packages:
-        repo = repo_group.find_repo(package)[1]
-        if not repo:
-            log.info(f"Package `{package}` is not installed.")
-            failed.append(package)
-            continue
-        try:
-            log.info(
-                f"""Removing `{package}`{" in soft mode" if args.soft else ""}..."""
-            )
-            args.soft or remove(repo.file_list)
-            repo_group.remove_repo(package)
-        except Exception as e:
-            failed.append(package)
-            log.error(f"Failed to remove `{package}`: {e}")
-            trace()
-            continue
-        log.info(f"`{package}` removed successfully.")
-    log.info(
-        f"Removing complete. Total: {len(args.packages)}, Success: {len(args.packages)-len(failed)}"
-    )
-    if failed:
-        log.info(f"Failed list: {failed}")
-
-
-def cli_update(args):
-    check_root()
-    failed = []
-
-    def update(repo: RepoHandler):
-        try:
-            log.info(f"Updating `{repo.name}`...")
-            result = repo.update_asset()
-            if result:
-                log.info(
-                    f"`{repo.name}` has an update: {result[0]} -> {result[1]}. Updating..."
-                )
-                download_and_install(args, repo, rename=False)
-                log.info(f"`{repo.name}` updated successfully.")
-            else:
-                log.info(f"`{repo.name}` is the newest.")
-        except Exception as e:
-            failed.append(repo.name)
-            log.error(f"Failed to update {repo.name}: {e}")
-            trace()
-
-    if not args.packages:  # update all
-        num = len(repo_group.repos)
-        for repo in repo_group.repos:
-            update(repo)
-    else:  # update some
-        num = len(args.packages)
-        for name in args.packages:
-            _, repo = repo_group.find_repo(name)
-            if repo:
-                update(repo)
-                repo_group.save()
-            else:
-                failed.append(name)
-                log.error(f"Package `{name}` not found.")
-
-    log.info(f"Update complete. Total: {num}, Success: {num-len(failed)}")
-    if failed:
-        log.info(f"Failed: {failed}")
-
-
-def cli_info(args):
-    try:
-        if not args.package:
-            repo_group.info_repos()
-        else:
-            repo_group.info_one_repo(str(args.package))
-    except RepoNotFoundError as e:
-        log.error(e)
-        exit(1)
-
-
-def cli_alias(args):
-    assert WINDOWS, "Alias command is only supported on Windows."
-    assert (
-        args.old_name != args.new_name
-    ), "Alias name cannot be the same as the original."
-
-    file = list(BIN_PATH.glob(args.old_name + "*"))
-    if not file:
-        log.error(f"Script `{args.old_name}` not found.")
-        exit(1)
-    if len(file) > 1:
-        name = file[0].with_suffix("")
-        assert name == file[1].with_suffix(
-            ""
-        ), "Both lnk should point to the same file."
-
-    repo_group.alias_lnk(args.old_name, args.new_name)
-    log.info(f"Alias `{args.old_name}` to `{args.new_name}`.")
+import logging as log
+from copy import copy
+from pathlib import Path
+from tempfile import TemporaryDirectory
+from urllib.parse import urlparse
+
+from .install import auto_install, download_and_extract, extract, remove
+from .search import RepoHandler
+from .storage import repo_group
+from .utils import check_root, error_exit, set_dry_run, trace
+from .utils.constants import BIN_PATH, WINDOWS
+from .utils.exceptions import RepoNotFoundError
+
+
+def parse_name_or_url(name_or_url: str) -> tuple[str, bool]:
+    """
+    Parse the name or url of a package.
+    `Returns`: a tuple with two elements: first is the true name, second is the flag of whether it is a url.
+    """
+    test_parse = urlparse(name_or_url)
+    if test_parse.netloc == "github.com":
+        return RepoHandler.get_info_by_url(name_or_url)[1], True
+    return name_or_url, False
+
+
+def download_and_install(args, repo: RepoHandler, rename=True):
+    try:
+        with TemporaryDirectory() as tmp_dir:
+            tmp_dir = Path(tmp_dir)
+            if args.local:
+                with Path(args.local).open("rb") as f:
+                    main_path = extract(f, tmp_dir)
+            else:
+                main_path = download_and_extract(repo.asset, tmp_dir)
+            auto_install(repo, main_path, rename=rename)
+    except Exception as e:
+        raise e
+
+
+def cli_install(args):
+    if args.interactive and args.quiet:
+        log.error("Cannot use both --interactive and --quiet.")
+        exit(1)
+    if args.quiet:
+        log.getLogger().setLevel(log.WARNING)
+    if args.dry_run:
+        set_dry_run()
+    else:
+        check_root()
+    if args.local and len(args.packages) > 1:
+        log.error(
+            "Cannot install multiple packages from local. Please install them separately."
+        )
+        exit(1)
+    for package in args.packages:
+        real_name, is_url = parse_name_or_url(package)
+        if not args.dry_run and repo_group.find_repo(real_name)[1]:
+            log.info(f"{real_name} is already installed.")
+            continue
+
+        # search
+        try:
+            if is_url:
+                repo = (
+                    RepoHandler(
+                        real_name,
+                        prefer_gnu=args.prefer_gnu,
+                        one_bin=args.one_bin,
+                        asset_filter=args.filter,
+                    )
+                    .set_by_url(package)
+                    .with_bin_name(args.bin_name)
+                )
+            else:
+                repo = RepoHandler(
+                    package,
+                    prefer_gnu=args.prefer_gnu,
+                    one_bin=args.one_bin,
+                    asset_filter=args.filter,
+                ).with_bin_name(args.bin_name)
+                if not args.local:
+                    repo.ask(quiet=args.quiet, sort=args.sort)
+            if not args.local:
+                repo.get_asset(interactive=args.interactive)
+        except Exception as e:
+            log.error(f"Failed on searching `{package}`: {e}")
+            trace()
+            exit(1)
+
+        # install
+        try:
+            download_and_install(args, repo)
+            print(f"Successfully installed `{repo.name}`.")
+            if WINDOWS:
+                bins = copy(repo.file_list)
+                bins = filter(lambda x: x.endswith(".lnk"), bins)
+                bins = map(lambda x: Path(x).stem, bins)
+                bins = map(lambda x: f"`{x}`", bins)
+                print(
+                    f"You can press `Win+r`, enter {', '.join(bins)} to start software, or execute in cmd."
+                )
+            if not args.dry_run:
+                repo_group.insert_repo(repo)
+        except Exception as e:
+            log.error(f"Failed to install `{repo.name}`: {e}")
+            trace()
+            log.error("Restoring...")
+            # rollback.
+            remove(repo.file_list)
+            error_exit("Files restored. Exiting...")
+
+
+def cli_remove(args):
+    check_root()
+    failed = []
+    for package in args.packages:
+        repo = repo_group.find_repo(package)[1]
+        if not repo:
+            log.info(f"Package `{package}` is not installed.")
+            failed.append(package)
+            continue
+        try:
+            log.info(
+                f"""Removing `{package}`{" in soft mode" if args.soft else ""}..."""
+            )
+            args.soft or remove(repo.file_list)
+            repo_group.remove_repo(package)
+        except Exception as e:
+            failed.append(package)
+            log.error(f"Failed to remove `{package}`: {e}")
+            trace()
+            continue
+        log.info(f"`{package}` removed successfully.")
+    log.info(
+        f"Removing complete. Total: {len(args.packages)}, Success: {len(args.packages)-len(failed)}"
+    )
+    if failed:
+        log.info(f"Failed list: {failed}")
+
+
+def cli_update(args):
+    check_root()
+    failed = []
+
+    def update(repo: RepoHandler):
+        try:
+            log.info(f"Updating `{repo.name}`...")
+            result = repo.update_asset()
+            if result:
+                log.info(
+                    f"`{repo.name}` has an update: {result[0]} -> {result[1]}. Updating..."
+                )
+                download_and_install(args, repo, rename=False)
+                log.info(f"`{repo.name}` updated successfully.")
+            else:
+                log.info(f"`{repo.name}` is the newest.")
+        except Exception as e:
+            failed.append(repo.name)
+            log.error(f"Failed to update {repo.name}: {e}")
+            trace()
+
+    if not args.packages:  # update all
+        num = len(repo_group.repos)
+        for repo in repo_group.repos:
+            update(repo)
+    else:  # update some
+        num = len(args.packages)
+        for name in args.packages:
+            _, repo = repo_group.find_repo(name)
+            if repo:
+                update(repo)
+                repo_group.save()
+            else:
+                failed.append(name)
+                log.error(f"Package `{name}` not found.")
+
+    log.info(f"Update complete. Total: {num}, Success: {num-len(failed)}")
+    if failed:
+        log.info(f"Failed: {failed}")
+
+
+def cli_info(args):
+    try:
+        if not args.package:
+            repo_group.info_repos()
+        else:
+            repo_group.info_one_repo(str(args.package))
+    except RepoNotFoundError as e:
+        log.error(e)
+        exit(1)
+
+
+def cli_alias(args):
+    assert WINDOWS, "Alias command is only supported on Windows."
+    assert (
+        args.old_name != args.new_name
+    ), "Alias name cannot be the same as the original."
+
+    file = list(BIN_PATH.glob(args.old_name + "*"))
+    if not file:
+        log.error(f"Script `{args.old_name}` not found.")
+        exit(1)
+    if len(file) > 1:
+        name = file[0].with_suffix("")
+        assert name == file[1].with_suffix(
+            ""
+        ), "Both lnk should point to the same file."
+
+    repo_group.alias_lnk(args.old_name, args.new_name)
+    log.info(f"Alias `{args.old_name}` to `{args.new_name}`.")
```

### Comparing `bin_package_manager-2.2.7/bpm/lib/windowspathadder.py` & `bin_package_manager-2.2.8/bpm/lib/windowspathadder.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.7/bpm/storage.py` & `bin_package_manager-2.2.8/bpm/storage.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import bisect
-import logging as log
-import pickle
-from contextlib import suppress
-from pathlib import Path
-from pprint import pprint
-from tempfile import TemporaryDirectory
-from typing import Optional, Union
-
-from .search import RepoHandler
-from .utils.constants import DATABASE_PATH, INFO_BASE_STRING, WINDOWS
-from .utils.exceptions import RepoNotFoundError
-
-
-class RepoGroup:
-    def __init__(self, db_path=DATABASE_PATH):
-        self.repos: list[RepoHandler] = []
-        self.db_path = db_path
-        # read config once in the init of RepoGroup.
-        self.read()
-
-    def read(self):
-        with suppress(FileNotFoundError):
-            self.repos = pickle.loads(self.db_path.read_bytes())
-        return self
-
-    def save(self):
-        self.db_path.parent.mkdir(parents=True, exist_ok=True)
-        self.db_path.write_bytes(pickle.dumps(self.repos))
-
-    def info_repos(self):
-        print(INFO_BASE_STRING.format("Name", "Url", "Version"))
-        for repo in self.repos:
-            print(repo)
-
-    def find_repo(
-        self, repo: Union[str, RepoHandler]
-    ) -> tuple[int, Optional[RepoHandler]]:
-        """
-        Find a repo.
-        return the index and the object of repo.
-        """
-        if isinstance(repo, str):
-            repo = RepoHandler(repo)
-        index = bisect.bisect_left(self.repos, repo)
-        if index != len(self.repos) and self.repos[index] == repo:
-            return (index, self.repos[index])
-        return (-1, None)
-
-    def info_one_repo(self, repo: Union[str, RepoHandler]) -> RepoHandler:
-        """
-        Print ALL messages about one repo.
-        If not found, raise exception `RepoNotFoundError`.
-        """
-        _, result = self.find_repo(repo)
-        if result:
-            pprint(vars(result))
-            return result
-        else:
-            raise RepoNotFoundError(getattr(repo, "name", repo))
-
-    def insert_repo(self, repo: RepoHandler):
-        """
-        Insert repo to RepoGroup, and save.
-        """
-        index = bisect.bisect_left(self.repos, repo)
-        self.repos.insert(index, repo)
-        self.save()
-
-    def remove_repo(self, repo: Union[str, RepoHandler]) -> RepoHandler:
-        """
-        Remove repo and save.
-        """
-        index, result = self.find_repo(repo)
-        if result:
-            self.repos.pop(index)
-            self.save()
-        else:
-            raise RepoNotFoundError(getattr(repo, "name", repo))
-
-    def alias_lnk(self, old_name: str, new_name: str):
-        """
-        Find `old_name` in all repo_group's `file_list`, and change the lnk and cmd name to `new_name`.
-
-        Note that the `old_name` and `new_name` should not include suffix.
-        """
-        assert WINDOWS, "alias is not supported on non-Windows systems."
-
-        # only change two files: lnk, cmd
-        count = 0
-        for repo in self.repos:
-            for i, s in enumerate(repo.installed_files):
-                s = Path(s)
-                assert s.exists(), "file in installed_list not found: " + s
-                if s.is_dir():
-                    continue
-                if s.stem == old_name and s.suffix in (".lnk", ".cmd", ""):
-                    new_path = s.with_stem(new_name)
-                    s.replace(new_path)
-                    repo.installed_files[i] = str(new_path)
-                    count += 1
-                    self.save()
-                if count >= 3:
-                    return
-        log.warning(
-            "You can update bpm and reinstall softwares to get cmd and sh support."
-        )
-
-
-import unittest  # noqa: E402
-
-
-class Test(unittest.TestCase):
-    def test_repogroup_operations(self):
-        with TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir) / "repos.db"
-            test_group = RepoGroup(db_path=tmpdir)
-            # insert, save
-            test_group.insert_repo(RepoHandler("test_repo"))
-            test_group.insert_repo(RepoHandler("abc"))
-            test_group.insert_repo(RepoHandler("z"))
-            test_group.repos.clear()
-            # read
-            test_group.read()
-            self.assertListEqual(
-                ["abc", "test_repo", "z"], [r.name for r in test_group.repos]
-            )
-            # remove
-            test_group.remove_repo("test_repo")
-            self.assertListEqual(["abc", "z"], [r.name for r in test_group.repos])
-
-
-if __name__ == "__main__":
-    unittest.main()
-    exit(0)
-else:
-    repo_group = RepoGroup()
+import bisect
+import logging as log
+import pickle
+from contextlib import suppress
+from pathlib import Path
+from pprint import pprint
+from tempfile import TemporaryDirectory
+from typing import Optional, Union
+
+from .search import RepoHandler
+from .utils.constants import DATABASE_PATH, INFO_BASE_STRING, WINDOWS
+from .utils.exceptions import RepoNotFoundError
+
+
+class RepoGroup:
+    def __init__(self, db_path=DATABASE_PATH):
+        self.repos: list[RepoHandler] = []
+        self.db_path = db_path
+        # read config once in the init of RepoGroup.
+        self.read()
+
+    def read(self):
+        with suppress(FileNotFoundError):
+            self.repos = pickle.loads(self.db_path.read_bytes())
+        return self
+
+    def save(self):
+        self.db_path.parent.mkdir(parents=True, exist_ok=True)
+        self.db_path.write_bytes(pickle.dumps(self.repos))
+
+    def info_repos(self):
+        print(INFO_BASE_STRING.format("Name", "Url", "Version"))
+        for repo in self.repos:
+            print(repo)
+
+    def find_repo(
+        self, repo: Union[str, RepoHandler]
+    ) -> tuple[int, Optional[RepoHandler]]:
+        """
+        Find a repo.
+        return the index and the object of repo.
+        """
+        if isinstance(repo, str):
+            repo = RepoHandler(repo)
+        index = bisect.bisect_left(self.repos, repo)
+        if index != len(self.repos) and self.repos[index] == repo:
+            return (index, self.repos[index])
+        return (-1, None)
+
+    def info_one_repo(self, repo: Union[str, RepoHandler]) -> RepoHandler:
+        """
+        Print ALL messages about one repo.
+        If not found, raise exception `RepoNotFoundError`.
+        """
+        _, result = self.find_repo(repo)
+        if result:
+            pprint(vars(result))
+            return result
+        else:
+            raise RepoNotFoundError(getattr(repo, "name", repo))
+
+    def insert_repo(self, repo: RepoHandler):
+        """
+        Insert repo to RepoGroup, and save.
+        """
+        index = bisect.bisect_left(self.repos, repo)
+        self.repos.insert(index, repo)
+        self.save()
+
+    def remove_repo(self, repo: Union[str, RepoHandler]) -> RepoHandler:
+        """
+        Remove repo and save.
+        """
+        index, result = self.find_repo(repo)
+        if result:
+            self.repos.pop(index)
+            self.save()
+        else:
+            raise RepoNotFoundError(getattr(repo, "name", repo))
+
+    def alias_lnk(self, old_name: str, new_name: str):
+        """
+        Find `old_name` in all repo_group's `file_list`, and change the lnk and cmd name to `new_name`.
+
+        Note that the `old_name` and `new_name` should not include suffix.
+        """
+        assert WINDOWS, "alias is not supported on non-Windows systems."
+
+        # only change two files: lnk, cmd
+        count = 0
+        for repo in self.repos:
+            for i, s in enumerate(repo.installed_files):
+                s = Path(s)
+                assert s.exists(), "file in installed_list not found: " + s
+                if s.is_dir():
+                    continue
+                if s.stem == old_name and s.suffix in (".lnk", ".cmd", ""):
+                    new_path = s.with_stem(new_name)
+                    s.replace(new_path)
+                    repo.installed_files[i] = str(new_path)
+                    count += 1
+                    self.save()
+                if count >= 3:
+                    return
+        log.warning(
+            "You can update bpm and reinstall softwares to get cmd and sh support."
+        )
+
+
+import unittest  # noqa: E402
+
+
+class Test(unittest.TestCase):
+    def test_repogroup_operations(self):
+        with TemporaryDirectory() as tmpdir:
+            tmpdir = Path(tmpdir) / "repos.db"
+            test_group = RepoGroup(db_path=tmpdir)
+            # insert, save
+            test_group.insert_repo(RepoHandler("test_repo"))
+            test_group.insert_repo(RepoHandler("abc"))
+            test_group.insert_repo(RepoHandler("z"))
+            test_group.repos.clear()
+            # read
+            test_group.read()
+            self.assertListEqual(
+                ["abc", "test_repo", "z"], [r.name for r in test_group.repos]
+            )
+            # remove
+            test_group.remove_repo("test_repo")
+            self.assertListEqual(["abc", "z"], [r.name for r in test_group.repos])
+
+
+if __name__ == "__main__":
+    unittest.main()
+    exit(0)
+else:
+    repo_group = RepoGroup()
```

### Comparing `bin_package_manager-2.2.7/bpm/utils/constants.py` & `bin_package_manager-2.2.8/bpm/utils/constants.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import pathlib
-import platform
-
-WINDOWS = False
-LINUX = False
-
-if platform.system() == "Linux":
-    CONF_PATH = pathlib.Path("/etc/bpm")
-    LINUX = True
-elif platform.system() == "Windows":
-    CONF_PATH = pathlib.Path.home() / "bpm"
-    WINDOWS = True
-else:
-    raise NotImplementedError("Unsupported platform")
-
-DATABASE_PATH = CONF_PATH / "bpm.db"
-INFO_BASE_STRING = "{:20}{:50}{:20}"
-OPTION_REPO_NUM = 7  # the number of repos to select in asking
-
-# windows only
-APP_PATH = CONF_PATH / "app"
-BIN_PATH = CONF_PATH / "bin"
+import pathlib
+import platform
+
+WINDOWS = False
+LINUX = False
+
+if platform.system() == "Linux":
+    CONF_PATH = pathlib.Path("/etc/bpm")
+    LINUX = True
+elif platform.system() == "Windows":
+    CONF_PATH = pathlib.Path.home() / "bpm"
+    WINDOWS = True
+else:
+    raise NotImplementedError("Unsupported platform")
+
+DATABASE_PATH = CONF_PATH / "bpm.db"
+INFO_BASE_STRING = "{:20}{:50}{:20}"
+OPTION_REPO_NUM = 7  # the number of repos to select in asking
+
+# windows only
+APP_PATH = CONF_PATH / "app"
+BIN_PATH = CONF_PATH / "bin"
```

### Comparing `bin_package_manager-2.2.7/pyproject.toml` & `bin_package_manager-2.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[tool.poetry]
-name = "bin-package-manager"
-version = "2.2.7"
-description = "Bin package manager, a package manager based on Github release"
-authors = ["lxl66566 <lxl66566@gmail.com>"]
-license = "MIT"
-readme = ["README.md"]
-keywords = ["binary", "packaging", "release"]
-repository = "https://github.com/lxl66566/bpm"
-homepage = "https://github.com/lxl66566/bpm"
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-]
-packages = [{ include = "bpm" }]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-py7zr = { version = "^0.20.8", markers = "sys_platform == 'win32'" }
-requests = "^2.31.0"
-tqdm = "^4.66.2"
-pylnk3 = { version = "^0.4.2", markers = "sys_platform == 'win32'" }
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.scripts]
-bpm = 'bpm.cli:main'
-
-[[tool.poetry.source]]
-name = "tsinghua-pypi"
-url = "https://pypi.tuna.tsinghua.edu.cn/simple"
-priority = "default"
+[tool.poetry]
+name = "bin-package-manager"
+version = "2.2.8"
+description = "Bin package manager, a package manager based on Github release"
+authors = ["lxl66566 <lxl66566@gmail.com>"]
+license = "MIT"
+readme = ["README.md"]
+keywords = ["binary", "packaging", "release"]
+repository = "https://github.com/lxl66566/bpm"
+homepage = "https://github.com/lxl66566/bpm"
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+packages = [{ include = "bpm" }]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+py7zr = "^0.20.8"
+requests = "^2.31.0"
+tqdm = "^4.66.2"
+pylnk3 = { version = "^0.4.2", markers = "sys_platform == 'win32'" }
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+bpm = 'bpm.cli:main'
+
+[[tool.poetry.source]]
+name = "tsinghua-pypi"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
+priority = "primary"
```

### Comparing `bin_package_manager-2.2.7/README.md` & `bin_package_manager-2.2.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,132 @@
-# bin package manager
-
-English | [简体中文](./docs/README.zh-CN.md)
-
-Bin package manager (BPM) is a Github release-based package manager that allows users to install and manage binaries from any Github release.
-
-BPM is currently supported on Linux and Windows, python >= 3.9.
-
-> [!CAUTION]
-> Risk Warning: BPM on Linux may damage your computer. By using BPM to install software, you accept this risk and trust third-party Github release packagers.
-
-## Why use it?
-
-In non-rolling release Linux distributions, the version of softwares in official source are often too low to use some new features.
-
-Rolling distributions, such as Archlinux, are also unable to install software from the AUR as root.
-
-A common way to manage packages on Windows is scoop, but it requires the packager to maintain a "manifest" list.
-
-## Installation
-
-BPM needs to be installed to root user.
-
-### pip
-
-#### Linux
-
-```sh
-sudo pip install bin-package-manager --break-system-packages
-sudo bpm
-```
-
-Note the risk of potentially breaking system packages.
-
-#### Windows
-
-```sh
-pip install bin-package-manager
-bpm
-```
-
-### pipx
-
-You can use pipx to install BPM.
-
-```sh
-sudo pipx install bin-package-manager
-```
-
-pipx will only install for the current user, so `sudo` is required. Alternatively, you can track on [this issue](https://github.com/pypa/pipx/issues/754) and use other methods mentioned there.
-
-### Source code
-
-If you don't want to use pipx, you can also download and use the source code.
-
-BPM requires [these libs](./requirements.txt), please install them manually.
-
-```sh
-git clone https://github.com/lxl66566/bpm.git
-cd bpm
-python3 -m bpm
-# or use poetry to install dependencies and run: `poetry install && poetry run python -m bpm`
-```
-
-## Usage
-
-- Install: `bpm i <package>`
-- Run `bpm -h` and `bpm i -h` for more help.
-
-```
-❯ bpm i -h
-usage: bpm install [-h] [-b [BIN_NAME]] [-l [Archive]] [-q] [--one-bin] [--prefer-gnu] [-n] [-i] [--filter [FILTER ...]] [--sort [SORT]] packages [packages ...]
-
-positional arguments:
-  packages              Package name or github url to install
-
-options:
-  -h, --help            show this help message and exit
-  -b [BIN_NAME], --bin-name [BIN_NAME]
-                        specify the binary executable filename, otherwise use package name by default.
-  -l [Archive], --local [Archive]
-                        install from local archive.
-  -q, --quiet           not ask, install the best match repo.
-  --one-bin             install given binary only. Use package name as binary name by default.
-  --prefer-gnu          bpm prefers musl target by default, you can change this default option.
-  -n, --dry-run         print the install position, but not install actually.
-  -i, --interactive     select asset interactively.
-  --filter [FILTER ...]
-                        filter assets
-  --sort [SORT]         sort param in github api, use `best-match` by default. The value could be `stars`, `forks`, `help-wanted-
-                        issues`, `updated`.
-```
-
-## How it works
-
-### Linux
-
-BPM automatically determines the file structure in the asset and installs it to the appropriate location on the system. The current installation is like:
-
-1. install binary
-2. merge the `lib`, `include`, `share`, `man`, `bin` directories into the system
-3. install completions
-4. install services (if exists systemd)
-
-BPM automatically adds the `.old` suffix to existing files to avoid overwrite. The `.old` files will be restored in uninstalling.
-
-### Windows
-
-BPM downloads asset into `%userprofile%/bpm/app/<name>` and creates shortcuts and cmd runner for the executables to `%userprofile%/bpm/bin`, which is added to `%path%`.
-
-## Develop
-
-```sh
-git clone https://github.com/lxl66566/bpm.git
-cd bpm
-poetry install
-poetry run python -m unittest bpm/**/*.py  # run tests
-```
-
-## TODO
-
-- [ ] no pre release
-- [x] try install
-- [x] windows support
-- [x] offline install
-- [x] install from github link
-- [x] update from local
+# bin package manager
+
+English | [简体中文](./docs/README.zh-CN.md)
+
+Bin package manager (BPM) is a Github release-based package manager that allows users to install and manage binaries from any Github release.
+
+BPM is currently supported on Linux and Windows, python >= 3.9.
+
+> [!CAUTION]
+> Risk Warning: Be aware of the potential risk of BPM Linux damaging your computer. By using BPM to install software, you accept this risk and trust third-party Github release packagers.
+
+> [TIP]
+> BPM guarantees parity, i.e., `bpm install` followed immediately by `bpm uninstall` will not change the system in any way.
+
+## Why use it?
+
+In non-rolling release Linux distributions, the version of softwares in official source are often too low to use some new features.
+
+Rolling distributions, such as Archlinux, are also unable to install software from the AUR as root.
+
+A common way to manage packages on Windows is scoop, but it requires the packager to maintain a "manifest" list.
+
+## Installation
+
+BPM needs to be installed to root user.
+
+### pip
+
+#### Linux
+
+```sh
+sudo pip install bin-package-manager --break-system-packages
+sudo bpm
+```
+
+Note the risk of potentially breaking system packages.
+
+#### Windows
+
+```sh
+pip install bin-package-manager
+bpm
+```
+
+### pipx
+
+You can use pipx to install BPM.
+
+```sh
+sudo pipx install bin-package-manager
+```
+
+pipx will only install for the current user, so `sudo` is required. Alternatively, you can track on [this issue](https://github.com/pypa/pipx/issues/754) and use other methods mentioned there.
+
+### Source code
+
+If you don't want to use pipx, you can also download and use the source code.
+
+BPM requires [these libs](./requirements.txt), please install them manually.
+
+```sh
+git clone https://github.com/lxl66566/bpm.git
+cd bpm
+python3 -m bpm
+# or use poetry to install dependencies and run: `poetry install && poetry run python -m bpm`
+```
+
+## Usage
+
+- Install: `bpm i <package>`
+- Run `bpm -h` and `bpm i -h` for more help.
+
+```
+❯ bpm i -h
+usage: bpm install [-h] [-b [BIN_NAME]] [-l [Archive]] [-q] [--one-bin] [--prefer-gnu] [-n] [-i] [--filter [FILTER ...]] [--sort [SORT]] packages [packages ...]
+
+positional arguments:
+  packages              Package name or github url to install
+
+options:
+  -h, --help            show this help message and exit
+  -b [BIN_NAME], --bin-name [BIN_NAME]
+                        specify the binary executable filename, otherwise use package name by default.
+  -l [Archive], --local [Archive]
+                        install from local archive.
+  -q, --quiet           not ask, install the best match repo.
+  --one-bin             install given binary only. Use package name as binary name by default.
+  --prefer-gnu          bpm prefers musl target by default, you can change this default option.
+  -n, --dry-run         print the install position, but not install actually.
+  -i, --interactive     select asset interactively.
+  --filter [FILTER ...]
+                        filter assets
+  --sort [SORT]         sort param in github api, use `best-match` by default. The value could be `stars`, `forks`, `help-wanted-
+                        issues`, `updated`.
+```
+
+## How it works
+
+### Linux
+
+BPM automatically determines the file structure in the asset and installs it to the appropriate location on the system. The current installation is like:
+
+1. install binary
+2. merge the `lib`, `include`, `share`, `man`, `bin` directories into the system
+3. install completions
+4. install services (if exists systemd)
+
+BPM automatically adds the `.old` suffix to existing files to avoid overwrite. The `.old` files will be restored in uninstalling.
+
+### Windows
+
+BPM downloads asset into `%userprofile%/bpm/app/<name>` and creates shortcuts and cmd runner for the executables to `%userprofile%/bpm/bin`, which is added to `%path%`.
+
+After v2.2.7, single `.exe` will be also installed.
+
+## Develop
+
+```sh
+git clone https://github.com/lxl66566/bpm.git
+cd bpm
+poetry install
+poetry run python -m unittest bpm/**/*.py  # run tests
+```
+
+## TODO
+
+- [ ] no pre release
+- [x] try install
+- [x] windows support
+- [x] offline install
+- [x] install from github link
+- [x] update from local
```

### Comparing `bin_package_manager-2.2.7/PKG-INFO` & `bin_package_manager-2.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: bin-package-manager
-Version: 2.2.7
+Version: 2.2.8
 Summary: Bin package manager, a package manager based on Github release
 Home-page: https://github.com/lxl66566/bpm
 License: MIT
 Keywords: binary,packaging,release
 Author: lxl66566
 Author-email: lxl66566@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: py7zr (>=0.20.8,<0.21.0) ; sys_platform == "win32"
+Requires-Dist: py7zr (>=0.20.8,<0.21.0)
 Requires-Dist: pylnk3 (>=0.4.2,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/lxl66566/bpm
 Description-Content-Type: text/markdown
 
 # bin package manager
@@ -27,15 +27,18 @@
 English | [简体中文](./docs/README.zh-CN.md)
 
 Bin package manager (BPM) is a Github release-based package manager that allows users to install and manage binaries from any Github release.
 
 BPM is currently supported on Linux and Windows, python >= 3.9.
 
 > [!CAUTION]
-> Risk Warning: BPM on Linux may damage your computer. By using BPM to install software, you accept this risk and trust third-party Github release packagers.
+> Risk Warning: Be aware of the potential risk of BPM Linux damaging your computer. By using BPM to install software, you accept this risk and trust third-party Github release packagers.
+
+> [TIP]
+> BPM guarantees parity, i.e., `bpm install` followed immediately by `bpm uninstall` will not change the system in any way.
 
 ## Why use it?
 
 In non-rolling release Linux distributions, the version of softwares in official source are often too low to use some new features.
 
 Rolling distributions, such as Archlinux, are also unable to install software from the AUR as root.
 
@@ -128,14 +131,16 @@
 
 BPM automatically adds the `.old` suffix to existing files to avoid overwrite. The `.old` files will be restored in uninstalling.
 
 ### Windows
 
 BPM downloads asset into `%userprofile%/bpm/app/<name>` and creates shortcuts and cmd runner for the executables to `%userprofile%/bpm/bin`, which is added to `%path%`.
 
+After v2.2.7, single `.exe` will be also installed.
+
 ## Develop
 
 ```sh
 git clone https://github.com/lxl66566/bpm.git
 cd bpm
 poetry install
 poetry run python -m unittest bpm/**/*.py  # run tests
```


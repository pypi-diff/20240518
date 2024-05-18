# Comparing `tmp/todotree-2.4.2.tar.gz` & `tmp/todotree-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todotree-2.4.2.tar", max compression
+gzip compressed data, was "todotree-2.5.0.tar", max compression
```

## Comparing `todotree-2.4.2.tar` & `todotree-2.5.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1211 2024-04-21 08:04:17.743468 todotree-2.4.2/LICENSE
--rw-r--r--   0        0        0     2289 2024-04-21 08:04:17.743468 todotree-2.4.2/README.md
--rw-r--r--   0        0        0     2618 2024-04-21 08:04:34.322252 todotree-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      537 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/AbstractCommand.py
--rw-r--r--   0        0        0      930 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Add.py
--rw-r--r--   0        0        0      626 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/AddX.py
--rw-r--r--   0        0        0     1564 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Addons.py
--rw-r--r--   0        0        0     1063 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Append.py
--rw-r--r--   0        0        0      640 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Cd.py
--rw-r--r--   0        0        0      403 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Context.py
--rw-r--r--   0        0        0     2032 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Do.py
--rw-r--r--   0        0        0      562 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Due.py
--rw-r--r--   0        0        0      319 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Edit.py
--rw-r--r--   0        0        0      512 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Filter.py
--rw-r--r--   0        0        0    11436 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Init.py
--rw-r--r--   0        0        0      419 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/List.py
--rw-r--r--   0        0        0      482 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/ListDone.py
--rw-r--r--   0        0        0      391 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/PrintRaw.py
--rw-r--r--   0        0        0      828 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Priority.py
--rw-r--r--   0        0        0      429 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Project.py
--rw-r--r--   0        0        0      822 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Recur.py
--rw-r--r--   0        0        0     1284 2024-04-21 08:04:17.749468 todotree-2.4.2/todotree/Commands/Revive.py
--rw-r--r--   0        0        0     1484 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Schedule.py
--rw-r--r--   0        0        0     1092 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Stale_add.py
--rw-r--r--   0        0        0      495 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Stale_list.py
--rw-r--r--   0        0        0      979 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Stale_revive.py
--rw-r--r--   0        0        0      473 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Commands/Version.py
--rw-r--r--   0        0        0      614 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/AbstractSubConfig.py
--rw-r--r--   0        0        0     7900 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/Config.py
--rw-r--r--   0        0        0     4102 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/ConsolePrefixes.py
--rw-r--r--   0        0        0     3772 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/ConsolePrefixesInit.py
--rw-r--r--   0        0        0     6179 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/GitHandler.py
--rw-r--r--   0        0        0     4099 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/Paths.py
--rw-r--r--   0        0        0     1567 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Config/TreePrint.py
--rw-r--r--   0        0        0      853 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/ConfigFileNotFoundError.py
--rw-r--r--   0        0        0      492 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/DoneFileNotFoundError.py
--rw-r--r--   0        0        0      461 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/GitError.py
--rw-r--r--   0        0        0      181 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/NoSuchTaskError.py
--rw-r--r--   0        0        0      182 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/ProjectFolderError.py
--rw-r--r--   0        0        0      173 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/RecurParseError.py
--rw-r--r--   0        0        0      498 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/StaleFileNotFoundError.py
--rw-r--r--   0        0        0      166 2024-04-21 08:04:17.750468 todotree-2.4.2/todotree/Errors/TaskParseError.py
--rw-r--r--   0        0        0      497 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Errors/TodoFileNotFoundError.py
--rw-r--r--   0        0        0      267 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Errors/TodotreeError.py
--rw-r--r--   0        0        0       91 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Errors/__init__.py
--rwxr-xr-x   0        0        0    13203 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Main.py
--rw-r--r--   0        0        0     3094 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/MainUtils.py
--rw-r--r--   0        0        0     3982 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/AbstractManager.py
--rw-r--r--   0        0        0     1593 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/DoneManager.py
--rw-r--r--   0        0        0     7001 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/RecurManager.py
--rw-r--r--   0        0        0      744 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/StaleManager.py
--rw-r--r--   0        0        0     5755 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Managers/TaskManager.py
--rw-r--r--   0        0        0     3806 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/ConsoleTask.py
--rw-r--r--   0        0        0     1634 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/DoneTask.py
--rw-r--r--   0        0        0     2399 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/RecurTask.py
--rw-r--r--   0        0        0    12630 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Task/Task.py
--rw-r--r--   0        0        0        0 2024-04-21 08:04:17.779467 todotree-2.4.2/todotree/Task/__init__.py
--rw-r--r--   0        0        0     4250 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/Tree.py
--rw-r--r--   0        0        0      129 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/__init__.py
--rw-r--r--   0        0        0      684 2024-04-21 08:04:34.736246 todotree-2.4.2/todotree/completions/todotree-completion.bash
--rw-r--r--   0        0        0      613 2024-04-21 08:04:34.852245 todotree-2.4.2/todotree/completions/todotree-completion.fish
--rw-r--r--   0        0        0     1182 2024-04-21 08:04:34.617248 todotree-2.4.2/todotree/completions/todotree-completion.zsh
--rw-r--r--   0        0        0     2776 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/examples/config.yaml
--rw-r--r--   0        0        0      188 2024-04-21 08:04:17.751468 todotree-2.4.2/todotree/examples/done.txt
--rw-r--r--   0        0        0      791 2024-04-21 08:04:17.752468 todotree-2.4.2/todotree/examples/recur.txt
--rw-r--r--   0        0        0      197 2024-04-21 08:04:17.752468 todotree-2.4.2/todotree/examples/stale.txt
--rw-r--r--   0        0        0     1372 2024-04-21 08:04:17.752468 todotree-2.4.2/todotree/examples/todo.txt
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 todotree-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-18 09:52:43.478278 todotree-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2289 2024-05-18 09:52:43.478278 todotree-2.5.0/README.md
+-rw-r--r--   0        0        0     2618 2024-05-18 09:53:01.158213 todotree-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      819 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/AbstractCommand.py
+-rw-r--r--   0        0        0      842 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Add.py
+-rw-r--r--   0        0        0      826 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/AddX.py
+-rw-r--r--   0        0        0     1646 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Addons.py
+-rw-r--r--   0        0        0     1028 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Append.py
+-rw-r--r--   0        0        0      710 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Cd.py
+-rw-r--r--   0        0        0      466 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Context.py
+-rw-r--r--   0        0        0     1993 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Do.py
+-rw-r--r--   0        0        0      559 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Due.py
+-rw-r--r--   0        0        0      389 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Edit.py
+-rw-r--r--   0        0        0      564 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Filter.py
+-rw-r--r--   0        0        0    11436 2024-05-18 09:52:43.486278 todotree-2.5.0/todotree/Commands/Init.py
+-rw-r--r--   0        0        0      507 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/List.py
+-rw-r--r--   0        0        0      520 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/ListDone.py
+-rw-r--r--   0        0        0      461 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/PrintRaw.py
+-rw-r--r--   0        0        0      861 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Priority.py
+-rw-r--r--   0        0        0      466 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Project.py
+-rw-r--r--   0        0        0      879 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Recur.py
+-rw-r--r--   0        0        0     1398 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Revive.py
+-rw-r--r--   0        0        0     1548 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Schedule.py
+-rw-r--r--   0        0        0     1179 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Stale_add.py
+-rw-r--r--   0        0        0      536 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Stale_list.py
+-rw-r--r--   0        0        0     1155 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Stale_revive.py
+-rw-r--r--   0        0        0      537 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Commands/Version.py
+-rw-r--r--   0        0        0      614 2024-05-18 09:52:43.487278 todotree-2.5.0/todotree/Config/AbstractSubConfig.py
+-rw-r--r--   0        0        0     7884 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Config/Config.py
+-rw-r--r--   0        0        0     4102 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Config/ConsolePrefixes.py
+-rw-r--r--   0        0        0     3740 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Config/ConsolePrefixesInit.py
+-rw-r--r--   0        0        0     6179 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Config/GitHandler.py
+-rw-r--r--   0        0        0     4053 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Config/Paths.py
+-rw-r--r--   0        0        0     1567 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Config/TreePrint.py
+-rw-r--r--   0        0        0      853 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Errors/ConfigFileNotFoundError.py
+-rw-r--r--   0        0        0      492 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Errors/DoneFileNotFoundError.py
+-rw-r--r--   0        0        0      461 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Errors/GitError.py
+-rw-r--r--   0        0        0      181 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Errors/NoSuchTaskError.py
+-rw-r--r--   0        0        0      182 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Errors/ProjectFolderError.py
+-rw-r--r--   0        0        0      173 2024-05-18 09:52:43.488278 todotree-2.5.0/todotree/Errors/RecurParseError.py
+-rw-r--r--   0        0        0      498 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Errors/StaleFileNotFoundError.py
+-rw-r--r--   0        0        0      166 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Errors/TaskParseError.py
+-rw-r--r--   0        0        0      497 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Errors/TodoFileNotFoundError.py
+-rw-r--r--   0        0        0      267 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Errors/TodotreeError.py
+-rw-r--r--   0        0        0       91 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Errors/__init__.py
+-rwxr-xr-x   0        0        0    13170 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Main.py
+-rw-r--r--   0        0        0     3094 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/MainUtils.py
+-rw-r--r--   0        0        0     3982 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Managers/AbstractManager.py
+-rw-r--r--   0        0        0     1593 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Managers/DoneManager.py
+-rw-r--r--   0        0        0     6970 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Managers/RecurManager.py
+-rw-r--r--   0        0        0      744 2024-05-18 09:52:43.489277 todotree-2.5.0/todotree/Managers/StaleManager.py
+-rw-r--r--   0        0        0     5773 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/Managers/TaskManager.py
+-rw-r--r--   0        0        0     3781 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/Task/ConsoleTask.py
+-rw-r--r--   0        0        0     1634 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/Task/DoneTask.py
+-rw-r--r--   0        0        0     2399 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/Task/RecurTask.py
+-rw-r--r--   0        0        0    12586 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/Task/Task.py
+-rw-r--r--   0        0        0        0 2024-05-18 09:52:43.532277 todotree-2.5.0/todotree/Task/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/Tree.py
+-rw-r--r--   0        0        0      324 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-18 09:53:01.602212 todotree-2.5.0/todotree/completions/todotree-completion.bash
+-rw-r--r--   0        0        0      613 2024-05-18 09:53:01.723211 todotree-2.5.0/todotree/completions/todotree-completion.fish
+-rw-r--r--   0        0        0     1182 2024-05-18 09:53:01.472212 todotree-2.5.0/todotree/completions/todotree-completion.zsh
+-rw-r--r--   0        0        0     2776 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/examples/config.yaml
+-rw-r--r--   0        0        0      188 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/examples/done.txt
+-rw-r--r--   0        0        0      791 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/examples/recur.txt
+-rw-r--r--   0        0        0      197 2024-05-18 09:52:43.490278 todotree-2.5.0/todotree/examples/stale.txt
+-rw-r--r--   0        0        0     1372 2024-05-18 09:52:43.491278 todotree-2.5.0/todotree/examples/todo.txt
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 todotree-2.5.0/PKG-INFO
```

### Comparing `todotree-2.4.2/LICENSE` & `todotree-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/README.md` & `todotree-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/pyproject.toml` & `todotree-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todotree"
-version = "2.4.2"
+version = "2.5.0"
 description = "todo.txt manager which adds tree printing"
 authors = ["chim1aap <fkjansen@protonmail.com>"]
 repository = "https://gitlab.com/chim1aap/todotree"
 documentation = "https://chim1aap.gitlab.io/todotree/"
 readme = "README.md"
 license = "Unlicense"
 packages = [
```

### Comparing `todotree-2.4.2/todotree/Commands/Add.py` & `todotree-2.5.0/todotree/Commands/Append.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from typing import Tuple
-
-import click
-
 from todotree.Commands.AbstractCommand import AbstractCommand
+from todotree.Errors.NoSuchTaskError import NoSuchTaskError
 from todotree.Errors.TodoFileNotFoundError import TodoFileNotFoundError
-from todotree.Task.Task import Task
 
 
-class Add(AbstractCommand):
+class Append(AbstractCommand):
+    def __call__(self, task_nr: int, append_string: str):
+        # Disable fancy imports, because they are not needed.
+        self.config.enable_project_folder = False
+        self.taskManager.import_tasks()
+        return self.taskManager.append_to_task(task_number=task_nr, task_string=append_string)
 
-    def run(self, task: Tuple):
-        # Convert tuple to string
-        task: str = " ".join(map(str, task))
+    def run(self, task_nr: int, append_string: tuple[str]):
+        # Append task.
         try:
-            # Disable fancy imports, because they are not needed.
-            self.config.enable_project_folder = False
-            # Import tasks.
-            self.taskManager.import_tasks()
-            # Add task
-            new_tasks = self.taskManager.add_tasks_to_file([Task(0, task)])
-            self.config.console.info("Task added:")
-            for task in new_tasks:
-                self.config.console.info(str(task))
-            self.config.git.commit_and_push("add")
+            new_task = self(task_nr, " ".join(append_string))
         except TodoFileNotFoundError as e:
             e.echo_and_exit(self.config)
+        except NoSuchTaskError as e:
+            self.config.console.error(e.message)
+            exit(1)
+        self.config.console.info("The new task is: ")
+        self.config.console.info(new_task)
+        self.config.git.commit_and_push("append")
```

### Comparing `todotree-2.4.2/todotree/Commands/AddX.py` & `todotree-2.5.0/todotree/Commands/AddX.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from typing import Tuple
-
 import click
 
 from todotree.Commands.AbstractCommand import AbstractCommand
 from todotree.Errors.DoneFileNotFoundError import DoneFileNotFoundError
 from todotree.Task.DoneTask import DoneTask
 from todotree.Task.Task import Task
 
 
 class AddX(AbstractCommand):
 
-    def run(self, task: Tuple):
+    def run(self, task: tuple):
         done = DoneTask.task_to_done(Task(0, " ".join(map(str, task))))
         if not self.config.paths.done_file.exists():
             DoneFileNotFoundError("").echo_and_exit(self.config)
         with self.config.paths.done_file.open("a") as f:
             f.write(done.to_file())
         click.echo(done)
+
+    def __call__(self, *args, **kwargs):
+        done = DoneTask.task_to_done(Task(0, " ".join(map(str, args))))
+        with self.config.paths.done_file.open("a") as f:
+            f.write(done.to_file())
+        return done
```

### Comparing `todotree-2.4.2/todotree/Commands/Addons.py` & `todotree-2.5.0/todotree/Commands/Addons.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,7 +39,10 @@
             self.config.console.error(f"The error is {e}")
             raise e
 
         click.echo(result.stdout, nl=False)
         if result.returncode != 0:
             click.echo(result.stderr)
         self.config.git.commit_and_push(f"addons {invocation}")
+
+    def __call__(self, *args, **kwargs):
+        raise NotImplemented # Too lazy.
```

### Comparing `todotree-2.4.2/todotree/Commands/Append.py` & `todotree-2.5.0/todotree/Commands/Revive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-from typing import Tuple
-
 import click
 
 from todotree.Commands.AbstractCommand import AbstractCommand
+from todotree.Errors.DoneFileNotFoundError import DoneFileNotFoundError
 from todotree.Errors.NoSuchTaskError import NoSuchTaskError
 from todotree.Errors.TodoFileNotFoundError import TodoFileNotFoundError
+from todotree.Managers.DoneManager import DoneManager
+from todotree.Task.Task import Task
 
 
-class Append(AbstractCommand):
-    def run(self, task_nr: int, append_string: Tuple[str]):
-        # Disable fancy imports, because they are not needed.
-        self.config.enable_project_folder = False
-        # Import tasks.
+class Revive(AbstractCommand):
+    def run(self, done_number: int):
         try:
-            self.taskManager.import_tasks()
-        except TodoFileNotFoundError as e:
+            new_tasks = self(done_number)
+        except DoneFileNotFoundError as e:
             e.echo_and_exit(self.config)
-        # Convert tuple to string.
-        append_string = " ".join(append_string)
-        # Append task.
-        try:
-            new_task = self.taskManager.append_to_task(task_nr, append_string.strip())
+            exit(1)  # IDE hinting.
         except NoSuchTaskError as e:
             self.config.console.error(e.message)
-            exit(1)
-        self.config.console.info("The new task is: ")
-        self.config.console.info(new_task)
-        self.config.git.commit_and_push("append")
+            exit(1)  # IDE hinting.
+        except TodoFileNotFoundError as e:
+            e.echo_and_exit(self.config)
+            exit(1)  # IDE hinting.
+        self.config.console.info("The newly revived tasks:")
+        for task in new_tasks:
+            self.config.console.info(str(task))
+        self.config.git.commit_and_push("revive")
+
+    def __call__(self, done_number: int) -> list[Task]:
+        done_manager = DoneManager(self.config)
+        done_manager.import_tasks()
+        revived_task = done_manager.remove_task_from_file(done_number)
+        self.taskManager.import_tasks()
+        return self.taskManager.add_tasks_to_file([Task(revived_task.i, revived_task.task_string)])
```

### Comparing `todotree-2.4.2/todotree/Commands/Cd.py` & `todotree-2.5.0/todotree/Commands/Cd.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,7 +16,10 @@
             click.echo(str(config_path))
             exit()
         # Then the relative path is resolved to be absolute.
         base_path: Path = Path.home()
         full_path: Path = base_path / config_path
         click.echo(str(full_path))
         exit()
+
+    def __call__(self, *args, **kwargs):
+        raise NotImplemented
```

### Comparing `todotree-2.4.2/todotree/Commands/Do.py` & `todotree-2.5.0/todotree/Commands/Do.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,46 @@
-from typing import Tuple, List
-
-import click
-from dateutil.utils import today
-
 from todotree.Commands.AbstractCommand import AbstractCommand
 from todotree.Errors.DoneFileNotFoundError import DoneFileNotFoundError
 from todotree.Errors.NoSuchTaskError import NoSuchTaskError
 from todotree.Errors.TodoFileNotFoundError import TodoFileNotFoundError
 from todotree.Managers.DoneManager import DoneManager
 from todotree.Task.DoneTask import DoneTask
 
 
 class Do(AbstractCommand):
 
-    def run(self, task_numbers: List[Tuple]):
+    def __call__(self, task_numbers: list[int]) -> list[DoneTask]:
+        # Marking something as Done cannot be done with fancy imports
+        # So we disable them.
+        self.config.enable_project_folder = False
+        self.taskManager.import_tasks()
+        completed_tasks = self.taskManager.remove_tasks_from_file(task_numbers)
+        done_manager = DoneManager(self.config)
+        done_manager.import_tasks()
+        done_tasks = [DoneTask.task_to_done(task) for task in completed_tasks]
+        done_manager.add_tasks_to_file(done_tasks)
+        return done_tasks
+
+    def run(self, task_numbers: list[tuple]):
         # Convert to ints. Task numbers is a list of tuples. Each tuple contains one digit of the number.
-        new_numbers: List[int] = []
+        new_numbers: list[int] = []
         for task_tuple in task_numbers:
             new_number: str = ""
             for task_digit in task_tuple:
                 new_number += task_digit
             new_numbers.append(int(new_number))
-        # Write back to old value.
-        task_numbers = new_numbers
-        # Marking something as Done cannot be done with fancy imports
-        # So we disable them.
-        self.config.enable_project_folder = False
         try:
-            self.taskManager.import_tasks()
-            completed_tasks = self.taskManager.remove_tasks_from_file(task_numbers)
+            done_tasks = self(new_numbers)
         except TodoFileNotFoundError as e:
             e.echo_and_exit(self.config)
             exit(1)  # IDE hinting.
         except NoSuchTaskError as e:
             self.config.console.error(e.message)
-            exit(1)
-        try:
-            done_manager = DoneManager(self.config)
-            done_manager.import_tasks()
-            done_tasks = [DoneTask.task_to_done(task) for task in completed_tasks]
-            done_manager.add_tasks_to_file(done_tasks)
-
+            exit(1) # IDE hinting.
         except DoneFileNotFoundError as e:
             e.echo_and_exit(self.config)
-            exit(1)  # For IDE hinting.
+            exit(1)  # IDE hinting.
         # Print the results
         self.config.console.info("Tasks marked as done:")
         for task in done_tasks:
             self.config.console.info(str(task))
         self.config.git.commit_and_push("do")
```

### Comparing `todotree-2.4.2/todotree/Commands/Due.py` & `todotree-2.5.0/todotree/Commands/Due.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import click
 
 from todotree.Commands.AbstractCommand import AbstractCommand
 from todotree.Errors.TodoFileNotFoundError import TodoFileNotFoundError
 
 
 class Due(AbstractCommand):
-    def run(self):
+    def __call__(self):
         # Disable fancy imports, because they do not have due dates.
         self.config.enable_project_folder = False
-        # Import tasks.
+        self.taskManager.import_tasks()
+        return self.taskManager.print_tree("due")
+
+    def run(self):
         try:
-            self.taskManager.import_tasks()
+            click.echo(self())
         except TodoFileNotFoundError as e:
             e.echo_and_exit(self.config)
-        # Print due tree.
-        click.echo(self.taskManager.print_tree("due"))
```

### Comparing `todotree-2.4.2/todotree/Commands/Init.py` & `todotree-2.5.0/todotree/Commands/Init.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Commands/Priority.py` & `todotree-2.5.0/todotree/Commands/Stale_revive.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from todotree.Commands.AbstractCommand import AbstractCommand
-from todotree.Errors.TodoFileNotFoundError import TodoFileNotFoundError
+from todotree.Errors.NoSuchTaskError import NoSuchTaskError
+from todotree.Errors.StaleFileNotFoundError import StaleFileNotFoundError
+from todotree.Managers.StaleManager import StaleManager
 from todotree.Task.Task import Task
 
 
-class Priority(AbstractCommand):
-    def run(self, task_number: int, new_priority: str):
-        # Disable fancy imports.
-        self.config.enable_project_folder = False
-        # Run task.
+class StaleRevive(AbstractCommand):
+
+    def run(self, task_number: int):
         try:
-            self.taskManager.import_tasks()
-        except TodoFileNotFoundError as e:
+            result = self(task_number)
+        except StaleFileNotFoundError as e:
             e.echo_and_exit(self.config)
-        new_task = self.taskManager.add_or_update_task(task_number, Task.add_or_update_priority,
-                                                       new_priority.upper())
-        self.config.console.info("The new task is: ")
-        self.config.console.info(new_task)
-        self.config.git.commit_and_push("priority")
+            exit(1) # IDE hinting.
+        except NoSuchTaskError as e:
+            self.config.console.error(e.message)
+            exit(1)
+
+        self.config.console.info("Revived the following task:")
+        for task in result:
+            self.config.console.info(task)
+        self.config.git.commit_and_push("Stale Revive")
+
+    def __call__(self, task_number: int) -> list[Task]:
+        stale_manager = StaleManager(self.config)
+        stale_manager.import_tasks()
+        revived_task = stale_manager.remove_task_from_file(task_number)
+        self.taskManager.import_tasks()
+        return self.taskManager.add_tasks_to_file([revived_task])
```

### Comparing `todotree-2.4.2/todotree/Commands/Recur.py` & `todotree-2.5.0/todotree/Commands/Recur.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 
     def run(self):
         if not self.config.paths.recur_file.exists():
             self.config.console.error("recur.txt not found, nothing to add.")
             self.config.console.error("It should be at the following location:")
             self.config.console.error(self.config.paths.recur_file)
             exit(1)
-        rm = RecurManager(self.config)
         try:
-            rm.import_tasks()
+            self()
         except RecurParseError as e:
             self.config.console.error(str(e))
             exit(1)
+        self.config.git.commit_and_push("recur")
+
+    def __call__(self, *args, **kwargs):
+        rm = RecurManager(self.config)
+        rm.import_tasks()
         rm.add_to_todo()
         rm.set_last_time_run()
-        self.config.git.commit_and_push("recur")
```

### Comparing `todotree-2.4.2/todotree/Commands/Schedule.py` & `todotree-2.5.0/todotree/Commands/Schedule.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,7 +29,10 @@
             self.taskManager.import_tasks()
             self.config.console.info(f"Task {task_number} hidden until {date}")
             updated_task = self.taskManager.add_or_update_task(task_number, Task.add_or_update_t_date, date)
             self.config.console.info(str(updated_task))
         except TodoFileNotFoundError as e:
             e.echo_and_exit(self.config)
         self.config.git.commit_and_push("schedule")
+
+    def __call__(self, *args, **kwargs):
+        NotImplemented
```

### Comparing `todotree-2.4.2/todotree/Commands/Stale_add.py` & `todotree-2.5.0/todotree/Commands/Stale_add.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from todotree.Commands.AbstractCommand import AbstractCommand
 from todotree.Errors.NoSuchTaskError import NoSuchTaskError
 from todotree.Errors.StaleFileNotFoundError import StaleFileNotFoundError
 from todotree.Managers.StaleManager import StaleManager
+from todotree.Task.Task import Task
 
 
 class StaleAdd(AbstractCommand):
 
-    def run(self, task_number):
-        stale_manager = StaleManager(self.config)
+    def run(self, task_number: int):
         try:
-            stale_manager.import_tasks()
+            task_to_add = self(task_number)
         except StaleFileNotFoundError as e:
             e.echo_and_exit(self.config)
+            exit(1)  # IDE hinting.
         except NoSuchTaskError as e:
             self.config.console.error(e.message)
             exit(1)
-        self.taskManager.import_tasks()
-        try:
-            task_to_add = self.taskManager.remove_task_from_file(task_number)
-        except NoSuchTaskError as e:
-            self.config.console.error(e.message)
-            exit(1)
-        stale_manager.add_tasks_to_file([task_to_add])
         self.config.console.info("Added the following tasks to the stale list.")
-        self.config.console.info(str(task_to_add))
+        for task in task_to_add:
+            self.config.console.info(str(task))
         self.config.git.commit_and_push("Stale Add")
+
+    def __call__(self, task_number: int) -> list[Task]:
+        stale_manager = StaleManager(self.config)
+        stale_manager.import_tasks()
+        self.taskManager.import_tasks()
+        task_to_add = self.taskManager.remove_task_from_file(task_number)
+        return stale_manager.add_tasks_to_file([task_to_add])
```

### Comparing `todotree-2.4.2/todotree/Config/AbstractSubConfig.py` & `todotree-2.5.0/todotree/Config/AbstractSubConfig.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Config/Config.py` & `todotree-2.5.0/todotree/Config/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Callable
+from typing import Callable
 
 from pathlib import Path
 
 import xdg_base_dirs
 
 from todotree.Config.Paths import Paths
 from todotree.Config.ConsolePrefixes import ConsolePrefixes
@@ -20,15 +20,15 @@
 
     For a user guide, please refer to the content in `examples/config.yaml` instead.
     Not all values are mapped 1-to-1.
     """
 
     def __init__(self):
         #  Main variables.
-        self.config_file: Optional[Path] = None
+        self.config_file: Path | None = None
         """Path to the config file."""
 
         # Features - Enables or disables certain features.
         self.enable_project_folder: bool = True
         """A value indicating whether to enable the project folder functionality."""
 
         #  Localization. #
@@ -49,15 +49,15 @@
         # Git functionality.
         self.git = GitHandler("disabled", 1, self.paths.todo_folder, self.console)
 
         # Debug
         self.__yaml_object = None
         """Raw config object, for debugging."""
 
-    def read(self, path: Optional[Path] = None):
+    def read(self, path: Path | None = None):
         """
         Loads the configuration from the given file at `path`.
 
         If empty, reads from default locations.
         """
         if path is not None:
             # print(f"Path is not None: {path}") # FUTURE: Verbose logging
```

### Comparing `todotree-2.4.2/todotree/Config/ConsolePrefixes.py` & `todotree-2.5.0/todotree/Config/ConsolePrefixes.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Config/ConsolePrefixesInit.py` & `todotree-2.5.0/todotree/Config/ConsolePrefixesInit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 import click
 
 from todotree.Config.ConsolePrefixes import ConsolePrefixes
 
 
 class ConsolePrefixesInit(ConsolePrefixes):
     """
@@ -33,15 +31,15 @@
             warning_prefix=c.warning_prefix,
             error_prefix=c.error_prefix,
             info_color=c.info_color,
             warn_color=c.warn_color,
             error_color=c.error_color
         )
 
-    def prompt_menu(self, question: str, answers: list, custom_answer: Optional[str] = None) -> str | int:
+    def prompt_menu(self, question: str, answers: list, custom_answer: str | None = None) -> str | int:
         """
         Ask the end user for input using a menu.
         @param question: The question to ask the user.
         @param answers: The predefined answers that the user can select.
         @param custom_answer: The custom option Text. Do not append with a dot.
             If the user chooses the Custom answer option. The user will be prompted to fill in the custom answer.
         @return: The answer that the user chose.
```

### Comparing `todotree-2.4.2/todotree/Config/GitHandler.py` & `todotree-2.5.0/todotree/Config/GitHandler.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Config/Paths.py` & `todotree-2.5.0/todotree/Config/Paths.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from pathlib import Path
-from typing import Optional
 
 import xdg_base_dirs
 from todotree.Config.AbstractSubConfig import AbstractSubConfig
 
 
 class Paths(AbstractSubConfig):
     """
     Configuration of the paths.
     Paths are calculated dynamically when not set.
     """
 
     def __init__(self):
         self.todo_folder: Path = xdg_base_dirs.xdg_data_home() / "todotree"
         """Path to the folder containing the data files."""
-        self.__project_tree_folder: Optional[Path] = None
-        self.__todo_file: Optional[Path] = None
-        self.__done_file: Optional[Path] = None
-        self.__recur_file: Optional[Path] = None
-        self.__addons_folder: Optional[Path] = None
-        self.__stale_file: Optional[Path] = None
+        self.__project_tree_folder: Path | None = None
+        self.__todo_file: Path | None = None
+        self.__done_file: Path | None = None
+        self.__recur_file: Path | None = None
+        self.__addons_folder: Path | None = None
+        self.__stale_file: Path | None = None
 
     def read_from_dict(self, new_values: dict):
         self.todo_folder = Path(new_values.get('folder', self.todo_folder)).expanduser()
 
         if (todo_file := new_values.get('todo_file')) is not None:
             self.todo_file = Path(todo_file).expanduser()
```

### Comparing `todotree-2.4.2/todotree/Config/TreePrint.py` & `todotree-2.5.0/todotree/Config/TreePrint.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Errors/ConfigFileNotFoundError.py` & `todotree-2.5.0/todotree/Errors/ConfigFileNotFoundError.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Main.py` & `todotree-2.5.0/todotree/Main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # NOTE: this file cannot be in a class. See: https://github.com/pallets/click/issues/601
 # https://click.palletsprojects.com/en/8.1.x/commands/#nested-handling-and-contexts
-
-from typing import List, Tuple
-
 import click
 
 # Commands are imported when the function is run, to increase performance.
 from todotree.Managers.TaskManager import TaskManager
 from todotree.Config.Config import Config
 from todotree.MainUtils import MainUtils
 
@@ -26,40 +23,40 @@
     ctx.obj["config"] = Config()
     MainUtils.parse_common_options(ctx.obj["config"], **kwargs)
 
 
 @root.command("add", short_help="Add a task to the task list")
 @click.argument("task", type=str, nargs=-1)
 @MainUtils.common_options
-def add(ctx: click.Context, task: Tuple, **kwargs):
+def add(ctx: click.Context, task: tuple, **kwargs):
     MainUtils.initialize(ctx.obj["config"], **kwargs)
     from todotree.Commands.Add import Add
 
     Add(ctx.obj["config"], TaskManager(ctx.obj["config"])).run(task)
 
 
 @root.command("addx", short_help="Add a task and immediately mark it as done")
 @click.argument("task", type=str, nargs=-1)
 @MainUtils.common_options
-def add_x(ctx: click.Context, task: Tuple, **kwargs):
+def add_x(ctx: click.Context, task: tuple, **kwargs):
     """
     Adds a completed task to done.txt. The task is not added to todo.txt.
     :param task: The task to add to done.txt.
     """
     MainUtils.initialize(ctx.obj["config"], **kwargs)
     from todotree.Commands.AddX import AddX
 
     AddX(ctx.obj["config"], TaskManager(ctx.obj["config"])).run(task)
 
 
 @root.command("append", short_help="Append `append_string` to `task_nr`")
 @click.argument("task_nr", type=int)
 @click.argument("append_string", type=str, nargs=-1)
 @MainUtils.common_options
-def append(ctx: click.Context, task_nr: int, append_string: Tuple[str], **kwargs):
+def append(ctx: click.Context, task_nr: int, append_string: tuple[str], **kwargs):
     """
     Appends the contents of append_string to the task represented by task_nr.
     A space is inserted between the two tasks, so you do not have to worry that words aretogether.
 
     Example: todotree append 1 "some text"
     """
     MainUtils.initialize(ctx.obj["config"], **kwargs)
@@ -87,15 +84,15 @@
 
     Context(ctx.obj["config"], TaskManager(ctx.obj["config"])).run()
 
 
 @root.command("do", short_help="Mark task as done and move it to the done.txt")
 @click.argument("task_numbers", type=list, nargs=-1)  # type=list[int]
 @MainUtils.common_options
-def do(ctx: click.Context, task_numbers: List[Tuple], **kwargs):
+def do(ctx: click.Context, task_numbers: list[tuple], **kwargs):
     """
     Mark tasks as done, therefor moving them to done.txt with a date stamp of today.
     :param task_numbers: The list of tasks which are completed.
     """
 
     MainUtils.initialize(ctx.obj["config"], **kwargs)
     from todotree.Commands.Do import Do
@@ -266,15 +263,15 @@
     Revive(ctx.obj["config"], TaskManager(ctx.obj["config"])).run(done_number)
 
 
 @root.command("schedule", short_help="Hide task until date.")
 @click.argument("task_number", type=int)
 @click.argument("new_date", type=str, nargs=-1)
 @MainUtils.common_options
-def schedule(ctx: click.Context, task_number: int, new_date: Tuple[str], **kwargs):
+def schedule(ctx: click.Context, task_number: int, new_date: tuple[str], **kwargs):
     """
     hide the task until the date given. If new_date is not in ISO format (yyyy-mm-dd) such as "Next Wednesday",
     then it tries to figure out the date with the `date` program, which is only in linux.
     """
     MainUtils.initialize(ctx.obj["config"], **kwargs)
     from todotree.Commands.Schedule import Schedule
```

### Comparing `todotree-2.4.2/todotree/MainUtils.py` & `todotree-2.5.0/todotree/MainUtils.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Managers/AbstractManager.py` & `todotree-2.5.0/todotree/Managers/AbstractManager.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Managers/DoneManager.py` & `todotree-2.5.0/todotree/Managers/DoneManager.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Managers/RecurManager.py` & `todotree-2.5.0/todotree/Managers/RecurManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import re
 from itertools import chain
-from typing import Optional
 
 from todotree.Config.Config import Config
 from todotree.Errors.RecurParseError import RecurParseError
 from todotree.Task.RecurTask import RecurTask
 from todotree.Managers.TaskManager import TaskManager
 
 
@@ -18,15 +17,15 @@
     recur_timestamp_filename = ".recur.timestamp"
     """Name of the timestamp file."""
 
     def __init__(self, config: Config):
         self.config: Config = config
         self.task_list: list[RecurTask] = []
         self.task_manager: TaskManager = TaskManager(self.config)
-        self.last_date: Optional[datetime.date] = None
+        self.last_date: datetime.date | None = None
 
     def import_tasks(self):
         """Import the tasks from recur.txt."""
         error = False
         with self.config.paths.recur_file.open("r") as f:
             for line_number, recur_task in enumerate(f.readlines()):
                 if not recur_task.strip():
```

### Comparing `todotree-2.4.2/todotree/Managers/StaleManager.py` & `todotree-2.5.0/todotree/Managers/StaleManager.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Managers/TaskManager.py` & `todotree-2.5.0/todotree/Managers/TaskManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,19 +130,21 @@
         :param task_number: The number of the existing task.
         :return: The new merged task.
         """
         self.task_list[task_number - 1] = self.task_list[task_number - 1] + task_string
         self.write_to_file()
         return self.task_list[task_number - 1]
 
-    def __str__(self, filter_string=None):
+    def filter(self, filter_string=None):
         """
         Filters the task list by whether `filter_string` occurred in the task.
         """
+        self.task_list = [item for item in self.task_list if filter_string in item.task_string]
+        return str(self)
+
+    def __str__(self):
         # Prepare the lists.
         self.filter_t_date()
         self.filter_block()
-        if filter_string:
-            self.task_list = [item for item in self.task_list if filter_string in item.task_string]
         self.task_list.sort(key=lambda x: x.priority)
         # Output the list.
         return super().__str__()
```

### Comparing `todotree-2.4.2/todotree/Task/ConsoleTask.py` & `todotree-2.5.0/todotree/Task/ConsoleTask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from todotree.Task.DoneTask import DoneTask
 from todotree.Task.Task import Task
 
 
 class ConsoleTask(Task):
     """
     Task class for printing to the console.
@@ -16,15 +14,15 @@
         return ct
 
     def __init__(self, i: int, task_string: str, total_digits=1):
         super().__init__(i, task_string)
         self.total_digits = total_digits
         """Represents the total number of digits that `i` must have."""
 
-        self.parts: List = []
+        self.parts: list = []
         """The parts of the final string for printing."""
 
 
 
 
     def __str__(self):
         """Base representation."""
```

### Comparing `todotree-2.4.2/todotree/Task/DoneTask.py` & `todotree-2.5.0/todotree/Task/DoneTask.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Task/RecurTask.py` & `todotree-2.5.0/todotree/Task/RecurTask.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/Task/Task.py` & `todotree-2.5.0/todotree/Task/Task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import datetime
 import re
 from datetime import datetime, date, timedelta
 
-from typing import List, Optional
-
 from dateutil.utils import today
 
 from todotree.Errors.TaskParseError import TaskParseError
 
 
 class Task:
     """
@@ -52,21 +50,21 @@
     block_pattern = re.compile(r"(bl:)(\w+)\s?")
     """Regex pattern which defines a block key. format: bl:string"""
 
     blocked_by_pattern = re.compile(r"(by:)(\w+)\s?")
     """Regex pattern which defines a blocked by key. format: by:string"""
 
     @property
-    def t_date(self) -> Optional[date]:
+    def t_date(self) -> date | None:
         """Property which returns the latest t date of the task."""
         return max(self.t_date_all) if len(self.t_date_all) > 0 else None
     # FUTURE: t_date Setter.
 
     @property
-    def due_date(self) -> Optional[date]:
+    def due_date(self) -> date | None:
         """Property which returns the earliest due date."""
         return min(self.due_date_all) if len(self.due_date_all) > 0 else None
     # FUTURE: due_date setter. https://mathspp.com/blog/pydonts/properties
 
     @property
     def due_date_band(self) -> str:
         """
@@ -95,45 +93,45 @@
 
     def __init__(self, i: int, task_string: str):
         """
         Initializes a single task from a string.
         :param i: The task number.
         :param task_string: The string containing the task.
         """
-        self.date_marked_done: Optional[str] = None
+        self.date_marked_done: str | None = None
         """Date that this task was marked as done."""
 
-        self.t_date_all: List[datetime.date] = []
+        self.t_date_all: list[datetime.date] = []
         """All t dates of a task."""
 
-        self.due_date_all: List[datetime.date] = []
+        self.due_date_all: list[datetime.date] = []
         """All due dates of a task"""
 
         self.task_string: str = ""
         """raw un formatted string"""
 
         self.other_string: str = task_string
         """String containing any part which is not captured in another variable."""
 
         self.i: int = i
         """Task Number"""
 
         self.priority_string: str = ""  # FUTURE: Convert to property instead.
         """priority as a String."""
 
-        self.projects: List[str] = []
+        self.projects: list[str] = []
         """List of all projects"""
 
-        self.contexts: List[str] = []
+        self.contexts: list[str] = []
         """List of all contexts"""
 
-        self.blocks: List[str] = []
+        self.blocks: list[str] = []
         """List of all block identifiers."""
 
-        self.blocked: List[str] = []
+        self.blocked: list[str] = []
         """List of all blocked by identifiers"""
 
         # Parse the various properties from the task.
         if task_string:  # task is not empty
             self.task_string = task_string.strip()  # Remove whitespace and the \n.
             self.write_string = task_string
```

### Comparing `todotree-2.4.2/todotree/Tree.py` & `todotree-2.5.0/todotree/Tree.py`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/completions/todotree-completion.bash` & `todotree-2.5.0/todotree/completions/todotree-completion.bash`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/completions/todotree-completion.fish` & `todotree-2.5.0/todotree/completions/todotree-completion.fish`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/completions/todotree-completion.zsh` & `todotree-2.5.0/todotree/completions/todotree-completion.zsh`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/examples/config.yaml` & `todotree-2.5.0/todotree/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/examples/recur.txt` & `todotree-2.5.0/todotree/examples/recur.txt`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/todotree/examples/todo.txt` & `todotree-2.5.0/todotree/examples/todo.txt`

 * *Files identical despite different names*

### Comparing `todotree-2.4.2/PKG-INFO` & `todotree-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todotree
-Version: 2.4.2
+Version: 2.5.0
 Summary: todo.txt manager which adds tree printing
 Home-page: https://gitlab.com/chim1aap/todotree
 License: Unlicense
 Author: chim1aap
 Author-email: fkjansen@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
```


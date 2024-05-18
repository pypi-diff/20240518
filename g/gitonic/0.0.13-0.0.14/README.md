# Comparing `tmp/gitonic-0.0.13.tar.gz` & `tmp/gitonic-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitonic-0.0.13.tar", last modified: Sat Nov 25 12:39:49 2023, max compression
+gzip compressed data, was "gitonic-0.0.14.tar", last modified: Sat May 18 05:09:12 2024, max compression
```

## Comparing `gitonic-0.0.13.tar` & `gitonic-0.0.14.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-11-25 12:39:49.900025 gitonic-0.0.13/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2788 2023-11-16 09:40:21.000000 gitonic-0.0.13/BACKLOG.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2340 2023-11-25 12:35:09.000000 gitonic-0.0.13/CHANGELOG.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    34078 2022-06-08 15:43:45.000000 gitonic-0.0.13/LICENSE.md
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       77 2022-07-30 03:47:27.000000 gitonic-0.0.13/MANIFEST.in
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    49216 2023-11-25 12:39:49.900025 gitonic-0.0.13/PKG-INFO
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     9046 2023-11-25 12:35:19.000000 gitonic-0.0.13/README.md
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-11-25 12:39:49.896025 gitonic-0.0.13/gitonic/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      147 2022-08-01 18:12:09.000000 gitonic-0.0.13/gitonic/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      155 2022-08-02 06:43:08.000000 gitonic-0.0.13/gitonic/__main__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       20 2023-11-25 12:34:50.000000 gitonic-0.0.13/gitonic/const.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    10328 2023-11-11 05:47:16.000000 gitonic-0.0.13/gitonic/file.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     7071 2023-11-16 09:23:21.000000 gitonic-0.0.13/gitonic/gitutil.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    38163 2023-11-25 12:18:12.000000 gitonic-0.0.13/gitonic/gui.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      172 2022-08-02 07:44:36.000000 gitonic-0.0.13/gitonic/icons.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3759 2023-07-05 05:07:07.000000 gitonic-0.0.13/gitonic/main.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     8941 2023-07-26 05:49:00.000000 gitonic-0.0.13/gitonic/pyjsoncfg.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1993 2023-07-10 08:49:03.000000 gitonic-0.0.13/gitonic/singleinstance.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      447 2022-08-11 08:09:58.000000 gitonic-0.0.13/gitonic/sysutil.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2821 2023-11-11 05:47:16.000000 gitonic-0.0.13/gitonic/task.py
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-11-25 12:39:49.900025 gitonic-0.0.13/gitonic/tile/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      462 2022-08-01 18:02:26.000000 gitonic-0.0.13/gitonic/tile/__init__.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    33970 2023-11-11 05:47:35.000000 gitonic-0.0.13/gitonic/tile/core.py
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1941 2023-11-11 05:47:16.000000 gitonic-0.0.13/gitonic/tile/tkcmd.py
-drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2023-11-25 12:39:49.896025 gitonic-0.0.13/gitonic.egg-info/
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    49216 2023-11-25 12:39:49.000000 gitonic-0.0.13/gitonic.egg-info/PKG-INFO
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      568 2023-11-25 12:39:49.000000 gitonic-0.0.13/gitonic.egg-info/SOURCES.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        1 2023-11-25 12:39:49.000000 gitonic-0.0.13/gitonic.egg-info/dependency_links.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       72 2023-11-25 12:39:49.000000 gitonic-0.0.13/gitonic.egg-info/entry_points.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      215 2023-11-25 12:39:49.000000 gitonic-0.0.13/gitonic.egg-info/requires.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        8 2023-11-25 12:39:49.000000 gitonic-0.0.13/gitonic.egg-info/top_level.txt
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      130 2023-07-26 12:09:46.000000 gitonic-0.0.13/pyproject.toml
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      896 2023-11-25 12:39:49.900025 gitonic-0.0.13/setup.cfg
--rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      716 2023-06-24 05:31:43.000000 gitonic-0.0.13/setup.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2024-05-18 05:09:12.950243 gitonic-0.0.14/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3005 2024-01-18 19:58:59.000000 gitonic-0.0.14/BACKLOG.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3025 2024-05-18 05:07:32.000000 gitonic-0.0.14/CHANGELOG.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    34078 2022-06-08 15:43:45.000000 gitonic-0.0.14/LICENSE.md
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       77 2022-07-30 03:47:27.000000 gitonic-0.0.14/MANIFEST.in
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    54456 2024-05-18 05:09:12.950243 gitonic-0.0.14/PKG-INFO
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    13384 2024-05-18 05:08:38.000000 gitonic-0.0.14/README.md
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2024-05-18 05:09:12.946243 gitonic-0.0.14/gitonic/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      147 2022-08-01 18:12:09.000000 gitonic-0.0.14/gitonic/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      155 2022-08-02 06:43:08.000000 gitonic-0.0.14/gitonic/__main__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       20 2024-05-18 05:07:48.000000 gitonic-0.0.14/gitonic/const.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    10328 2023-11-11 05:47:16.000000 gitonic-0.0.14/gitonic/file.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     7071 2023-11-16 09:23:21.000000 gitonic-0.0.14/gitonic/gitutil.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    43055 2024-02-20 06:56:15.000000 gitonic-0.0.14/gitonic/gui.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      172 2022-08-02 07:44:36.000000 gitonic-0.0.14/gitonic/icons.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     3759 2023-07-05 05:07:07.000000 gitonic-0.0.14/gitonic/main.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     8941 2023-07-26 05:49:00.000000 gitonic-0.0.14/gitonic/pyjsoncfg.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1993 2023-07-10 08:49:03.000000 gitonic-0.0.14/gitonic/singleinstance.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      447 2022-08-11 08:09:58.000000 gitonic-0.0.14/gitonic/sysutil.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     2889 2024-01-17 20:47:04.000000 gitonic-0.0.14/gitonic/task.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2024-05-18 05:09:12.950243 gitonic-0.0.14/gitonic/tile/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      492 2024-01-07 07:12:06.000000 gitonic-0.0.14/gitonic/tile/__init__.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    35938 2024-03-24 09:02:45.000000 gitonic-0.0.14/gitonic/tile/core.py
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)     1941 2023-11-11 05:47:16.000000 gitonic-0.0.14/gitonic/tile/tkcmd.py
+drwxrwxr-x   0 benutzer  (1000) benutzer  (1000)        0 2024-05-18 05:09:12.950243 gitonic-0.0.14/gitonic.egg-info/
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)    54456 2024-05-18 05:09:12.000000 gitonic-0.0.14/gitonic.egg-info/PKG-INFO
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      568 2024-05-18 05:09:12.000000 gitonic-0.0.14/gitonic.egg-info/SOURCES.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        1 2024-05-18 05:09:12.000000 gitonic-0.0.14/gitonic.egg-info/dependency_links.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)       72 2024-05-18 05:09:12.000000 gitonic-0.0.14/gitonic.egg-info/entry_points.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      215 2024-05-18 05:09:12.000000 gitonic-0.0.14/gitonic.egg-info/requires.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)        8 2024-05-18 05:09:12.000000 gitonic-0.0.14/gitonic.egg-info/top_level.txt
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      130 2023-07-26 12:09:46.000000 gitonic-0.0.14/pyproject.toml
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      896 2024-05-18 05:09:12.954243 gitonic-0.0.14/setup.cfg
+-rw-rw-r--   0 benutzer  (1000) benutzer  (1000)      716 2023-06-24 05:31:43.000000 gitonic-0.0.14/setup.py
```

### Comparing `gitonic-0.0.13/BACKLOG.md` & `gitonic-0.0.14/BACKLOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 - git error handling
 - switch to log tab after pull
 - logging, use python logger for expert mode output
 - support for .gitignore 
   - adding single files 
   - open .gitignore for editing
 - execute git operations in parallel where possible
+- make expert mode debugging out better (use python logging)
 - 
 
 
 # OPEN ISSUES
 
 refer to [issues](https://github.com/kr-g/gitonic/issues)
 
@@ -82,10 +83,11 @@
  no separate credit store provided.
 - only existing git repo's under the workspace are supported,
  as of now no support to create a new git repo. 
  use `git init`, or `git clone` manually from cmd-line
 - `gitonic` interacts with `git` just like starting in bash / commandline.
 at the present time there is _no_additional_ error checking. 
 this must be done by checking the log tab manually where all cmdline output goes.
-
+- at the present time the context menu only works on the underlying file (row) in the table. 
+ there is no support for multiple files (selection) as of now.
```

### Comparing `gitonic-0.0.13/CHANGELOG.md` & `gitonic-0.0.14/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,29 @@
-
+ 
 # Changelog
 
 
-# next version v0.0.13 - 20231125
+# version v0.0.14 - 20240518
+
+- improved formatter 
+  - support for multiple file extension for single config entry 
+  - support for path expansion for formatter config
+  - added sample for uncrustify (c, c++)
+- on "changes" tab
+  - added context menu to open file system explorer
+  - added support for custom context menu with `~/.gitonic/context.json`
+- calling merge-tool with more then more file selected on change tab will 
+ not block the user-interface anymore since starting independent from main process
+  - **important** add `--newtab` to `meld` configuration in `.gitconfig` 
+   to re-use an already running instance of `meld`
+- context menu handler expands user path (`~`)
+- 
+
+
+# version v0.0.13 - 20231125
 
 - show all untracked files on changes tab (not only the folder)
 - 
 
 
 # version v0.0.12 - 20231111
```

### Comparing `gitonic-0.0.13/LICENSE.md` & `gitonic-0.0.14/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/PKG-INFO` & `gitonic-0.0.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitonic
-Version: 0.0.13
+Version: 0.0.14
 Summary: manage a multi git workspace
 Home-page: https://github.com/kr-g/gitonic
 Author: k. goger
 Author-email: k.r.goger+gitonic@gmail.com
 License: AGPLv3+
 Keywords: python utility shell git git-workspace tkinter
 Platform: UNKNOWN
@@ -25,27 +25,24 @@
 Provides-Extra: PEP08_BLACK
 Provides-Extra: PEP08_FULL
 License-File: LICENSE.md
 
 [![PEP-08](https://img.shields.io/badge/code%20style-PEP08-green.svg)](https://www.python.org/dev/peps/pep-0008/)
 
 
-you are reading VERSION = v0.0.13
+you are reading VERSION = v0.0.14
 
 
 # gitonic 
 
 gitonic simplifies working with multiple git repositories.
 
 
 gitonic comes with an easy to use Tkinter GUI.
 
-there is also a plugin for thonny 
-[`thonny-gitonic`](https://github.com/kr-g/thonny-gitonic) 
-
 
 # background 
 
 where software components/ artefacts are stored in multiple repositories 
 separately gitonic helps to keep track
 
 
@@ -156,15 +153,19 @@
         "cmd": "full-path-to-command",
         "para": [
           "%file"
         ]
       }
     }
 
-here `para` is an array of cmd-line options passed to the formatter command
+where `.file-ext` is a simple file extension such as `.py`, 
+or a comma separated list of extensions `.c,.h,.cpp`.
+wild-cards are not supported.
+
+where `para` is an array of cmd-line options passed to the formatter command
 where `%file` is a placeholder and replaced by the file name
 
 for different file extensions `gitonic` will call the formatter accordingly 
 even if the selected files are of different types (extensions)
 
 
 ## templates for python pep08 formatters
@@ -187,14 +188,28 @@
         "para": [
           "-i",
           "%file"
         ]
       }
     }
 
+to use the same code formatter also for 
+[`cython's`](https://github.com/cython/cython) 
+files with extension `.pyx` change the setting to
+
+    {
+      ".py,.pyx": {
+        "cmd": "autopep8",
+        "para": [
+          "-i",
+          "%file"
+        ]
+      }
+    }
+
 
 ### black
 
 black is also an offical python tool, but resolves not fully to issues reported by pycodestyle.
 there might be some rework required (from case to case). 
 result is quite similar to autopep8 beside the list reported by pycodestyle (after formatting) 
 is a bit longer comparing to autopep8 what does a better job here.
@@ -221,14 +236,171 @@
           "-i",
           "%file"
         ]
       }
     }
 
 
+## templates for c, c++ formatters
+
+all of the following tools are NOT part of `gitonic` standard installation. 
+
+
+### uncrustify
+
+[`uncrustify`](https://github.com/uncrustify/uncrustify) 
+is a code formatter for c, c++ (and other languages).
+
+here in this config sample it is configured for extensions `.c`, `.h`, and `.cpp`.
+
+IMPORTANT: `uncrustify` requires an additional config file, a sample can be found here
+[`uncrustify.cfg`](https://github.com/uncrustify/uncrustify/blob/master/forUncrustifySources.cfg)
+
+here in the sample the `uncrustify` config file is placed in path `~/.gitonic/uncrustify.cfg`.
+make sure that it is there.
+
+the following needs to be placed inside `~/.gitonic/formatter.json`
+
+
+    ".c,.h,.cpp": {
+        "cmd": "uncrustify",
+        "para": [
+              "-c",
+              "~/.gitonic/uncrustify.cfg",
+              "--replace",
+              "%file",
+              "--no-backup",
+              "--if-changed"
+        ]
+    }
+
+
+# custom context menu handler 
+
+when clicking on the `changes` tab right a context memu opens offering 
+to open the system file manager tool (file explorer) 
+at the base git repo path or at the changed file path.
+
+in addition it is possible to add own custom context menu entries here.
+configuration is done with `~/.gitonic/context.json` file.
+
+the general structure is:
+
+    {
+      "a-context-name-ctx": {
+        "expr": "*",
+        "menu": [
+          [
+            "some text $GIT",
+            [
+              "cmd-path",
+              "whatever_param=$GIT"
+            ]
+          ],
+          [
+            "some other text $PATH",
+            [
+              "cmd-path2",
+              "whatever_param=$PATH"
+            ]
+          ]
+        ]
+      },
+      ...
+    }
+
+
+here the variables `$GIT`, `$PATH`, or `$FILE` are replaced 
+by the corrosponding path before execution.
+
+the `expr` key contains a single file pattern, or a list of 
+file patterns - when to enable the context menu. 
+the file pattern is following Unix filename pattern matching.
+
+the `menu` array contains the text to display in the menu, 
+and the command params as embedded array.
+
+the context name as such can have any value 
+(as long it is unique in the structure).
+
+
+below a sample `~/.gitonic/context.json` file 
+for running on linux with xfce.
+
+    {
+      "term-ctx": {
+        "expr": "*",
+        "menu": [
+          [
+            "Open Terminal at $GIT",
+            [
+              "xfce4-terminal",
+              "--working-directory=$GIT"
+            ]
+          ],
+          [
+            "Open Terminal at $PATH",
+            [
+              "xfce4-terminal",
+              "--working-directory=$PATH"
+            ]
+          ],
+          [
+            "Edit .gitignore at $GIT",
+            [
+              "xed",
+              "$GIT/.gitignore"
+            ]
+          ]
+        ]
+      },
+      "spyder-ctx": {
+        "expr": "*.py",
+        "menu": [
+          [
+            "spyder python $FILE",
+            [
+              "~/spyder/.venv/bin/spyder",
+              "$FILE"
+            ]
+          ]
+        ]
+      },
+      "geany-ctx": {
+        "expr": [
+          "*.c",
+          "*.cpp",
+          "*.h"
+        ],
+        "menu": [
+          [
+            "geany c $FILE",
+            [
+              "geany",
+              "$FILE"
+            ]
+          ]
+        ]
+      }
+    }
+
+
+remark:
+the sample config file provides support for opening
+- terminal, in this case `xfce4-terminal`, can be replaced by e.g. `xterm` - depending on your distribution
+- `.gitignore` file for selected repo with [`xed`](https://en.wikipedia.org/wiki/Xed)
+- [`spyder-ide.org`](https://spyder-ide.org/), for files matching `*.py`
+- [`geany`](https://www.geany.org/), for files matching `*.c`, `*.cpp`, `*.h`
+
+
+**limitation:**
+
+at the present time the context menu only works on the underlying file (row) in the table.
+there is **no** support for multiple files (selection) as of now.
+
 
 
 # platform
 
 tested on python3, and linux
 
 
@@ -315,15 +487,15 @@
 when during startup an error is thrown, refer to 
 [installation on raspberry, fedorra](https://github.com/kr-g/gitonic/issues/6)
 
 
 # git configuration
 
 add a `.git-credentials` file as described here 
-[`git-credentials`](https://git-scm.com/docs/git-credential-store#_storage_format)
+[`git-credentials`](https://git-scm.com/docs/git-credential-store)
 
 
 add a `.gitconfig` file as described here
 [`git-config`](https://git-scm.com/docs/git-config)
 and configure for diff and merge tools. 
 NOTE: you need to install the diff-tool e.g. 
 [`meld merge`](https://meldmerge.org/) manually, 
@@ -338,22 +510,22 @@
         helper = store
 
     [diff]
         tool = meld
     [difftool]
         prompt = false
     [difftool "meld"]
-        cmd = meld "$LOCAL" "$REMOTE"
+        cmd = meld --newtab "$LOCAL" "$REMOTE"
 
     [merge]
         tool = meld
     [mergetool "meld"]
         # Choose one of these 2 lines (not both!) 
         # cmd = meld "$LOCAL" "$MERGED" "$REMOTE" --output "$MERGED"
-        cmd = meld "$LOCAL" "$BASE" "$REMOTE" --output "$MERGED"
+        cmd = meld --newtab "$LOCAL" "$BASE" "$REMOTE" --output "$MERGED"
 
 
 # additional notes 
 
 the following tools are part of the standard git distribution 
 
 - [`gitk`](https://git-scm.com/docs/gitk)
@@ -367,17 +539,18 @@
 # internals
 
 following files are used:
 
 |file|description|
 |---|---|
 |~/.gitonic/commit.json|the last commit messages show in the combo box|
-|~/.gitonic/tracked.json|tracked git repositories|
 |~/.gitonic/config.json|configuration settings|
+|~/.gitonic/context.json|configuration for context menu on changes tab|
 |~/.gitonic/formatter.json|configuration for external formatter tools|
+|~/.gitonic/tracked.json|tracked git repositories|
 |~/.gitonic/socket|internal use|
 
 
 HINT:
 crash after configuration change can be resolved by changing the setting manually 
 in `config.json`, or delete the config file to fall back to the defaults
 
@@ -385,19 +558,36 @@
 # license
 
 gitonic is released under the following
 [`LICENSE`](https://github.com/kr-g/gitonic/blob/main/LICENSE.md)
 
 
 
-
+ 
 # Changelog
 
 
-# next version v0.0.13 - 20231125
+# version v0.0.14 - 20240518
+
+- improved formatter 
+  - support for multiple file extension for single config entry 
+  - support for path expansion for formatter config
+  - added sample for uncrustify (c, c++)
+- on "changes" tab
+  - added context menu to open file system explorer
+  - added support for custom context menu with `~/.gitonic/context.json`
+- calling merge-tool with more then more file selected on change tab will 
+ not block the user-interface anymore since starting independent from main process
+  - **important** add `--newtab` to `meld` configuration in `.gitconfig` 
+   to re-use an already running instance of `meld`
+- context menu handler expands user path (`~`)
+- 
+
+
+# version v0.0.13 - 20231125
 
 - show all untracked files on changes tab (not only the folder)
 - 
 
 
 # version v0.0.12 - 20231111
 
@@ -570,14 +760,15 @@
 - git error handling
 - switch to log tab after pull
 - logging, use python logger for expert mode output
 - support for .gitignore 
   - adding single files 
   - open .gitignore for editing
 - execute git operations in parallel where possible
+- make expert mode debugging out better (use python logging)
 - 
 
 
 # OPEN ISSUES
 
 refer to [issues](https://github.com/kr-g/gitonic/issues)
 
@@ -593,15 +784,16 @@
  no separate credit store provided.
 - only existing git repo's under the workspace are supported,
  as of now no support to create a new git repo. 
  use `git init`, or `git clone` manually from cmd-line
 - `gitonic` interacts with `git` just like starting in bash / commandline.
 at the present time there is _no_additional_ error checking. 
 this must be done by checking the log tab manually where all cmdline output goes.
-
+- at the present time the context menu only works on the underlying file (row) in the table. 
+ there is no support for multiple files (selection) as of now.
  
 
 
 ---
 
 Copyright (c) 2022 k. goger - https://github.com/kr-g
```

### Comparing `gitonic-0.0.13/gitonic/file.py` & `gitonic-0.0.14/gitonic/file.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/gitonic/gitutil.py` & `gitonic-0.0.14/gitonic/gitutil.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/gitonic/gui.py` & `gitonic-0.0.14/gitonic/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .const import VERSION
 
 import os
 import time
 import json
 import webbrowser
+import fnmatch
 
 from .pyjsoncfg import Config
 
 import tkinter
 from tkinter import Tk
 
 from .icons import get_icon
@@ -348,17 +349,21 @@
                                         ("git", None),
                                         ("branch", None),
                                         ("file", None),
                                         ("unstaged", None),
                                         ("staged", None),
                                         ("type", None),
                                     ],
-                                    header_width=(150, 100, 250, 100, 100, 100),
+                                    header_width=(
+                                        150, 100, 250, 100, 100, 100),
                                     height=13,
-                                    on_double_click=lambda x: on_add_or_undo(x),
+                                    on_double_click=lambda x: on_add_or_undo(
+                                        x),
+                                    on_right_click=lambda cntrl, ctx: on_changed_context(
+                                        cntrl, ctx),
                                 ),
                                 TileCols(
                                     source=[
                                         TileLabelButton(
                                             caption="changes",
                                             commandtext="refresh",
                                             icon=get_icon(ICO_REFRESH),
@@ -408,15 +413,16 @@
                                             command=lambda: on_diff(),
                                             hotkey="<Alt-Key-w>",
                                         ),
                                         TileLabelButton(
                                             idn="black",
                                             caption="",
                                             commandtext="autoformat source",
-                                            icon=get_icon(ICO_FILE_FORMATSOURCE),
+                                            icon=get_icon(
+                                                ICO_FILE_FORMATSOURCE),
                                             command=lambda: on_formatter(),
                                             hotkey="<Alt-Key-f>",
                                         ),
                                         TileLabelButton(
                                             idn="difftool",
                                             caption="",
                                             commandtext="difftool",
@@ -436,15 +442,16 @@
                                 TileLabel(caption=""),
                                 TileCols(
                                     source=[
                                         TileEntryCombo(
                                             caption="message:",
                                             idn="commit_short",
                                             width=50,
-                                            on_select=lambda x, v: on_sel_commit(x),
+                                            on_select=lambda x, v: on_sel_commit(
+                                                x),
                                         ),
                                         TileLabelButton(
                                             caption="",
                                             commandtext="clear",
                                             icon=get_icon(ICO_CLR),
                                             command=lambda: on_clr_commit(),
                                             hotkey="<Alt-Key-c>",
@@ -469,15 +476,16 @@
                                             icon=get_icon("upload"),
                                             command=lambda: on_push_tracked(),
                                             hotkey="<Alt-Key-s>",
                                         ),
                                         TileLabelButton(
                                             caption="",
                                             commandtext="commit + push",
-                                            icon=get_icon("wand-magic-sparkles"),
+                                            icon=get_icon(
+                                                "wand-magic-sparkles"),
                                             command=lambda: on_commit_push_tracked(),
                                             hotkey="<Alt-Key-e>",
                                         ),
                                         TileCheckbutton(
                                             caption="push tags",
                                             idn="push_tags",
                                             on_click=lambda x: write_config(),
@@ -608,62 +616,139 @@
 
 def on_unsel_all_gits():
     dgb_pr("on_sel_all_gits")
     gt("gits").clr_selection()
     set_tracked_gits()
 
 
+def _run_diff_tool(path, file, callb=None):
+    # todo rework with gitutil -> git_difftool
+    dgb_pr("_run_diff_tool", path, file)
+
+    from .gitutil import GIT
+
+    cwd = os.getcwd()
+
+    try:
+        os.chdir(path)
+        if os.getcwd() != path:
+            raise Exception("path not exist", path)
+        args = [GIT, "difftool", file]
+        rc = os.spawnvpe(os.P_NOWAIT, args[0], args, os.environ)
+    except Exception as ex:
+        dgb_pr(ex)
+
+    os.chdir(cwd)
+
+    return ["difftool", file]
+
+
 def on_cmd_diff(info, diff_, ignore_switch=False):
     dgb_pr(info)
     sel = gt("changes").get_selection_values()
+    run_first = True
     for rec in sel:
         if rec["type"] == "file":
             pg = FileStat(gws.base_repo_dir.name).join([rec["git"]]).name
             git = gws.find(pg)[0]
             logs = []
             rc = diff_(git.path, rec["file"], callb=logs.append)
+
+#             if run_first and len(sel) > 1:
+#                 run_first = False
+#                 # todo rework -> freezing screen
+#                 # todo add input field on settings tab
+#                 time.sleep(0.5)
+
             dgb_pr(f"--- {git}")
             [dgb_pr(x) for x in rc]
             do_log_time(info, ignore_switch=ignore_switch)
             do_logs(rc)
             do_logs_opt(logs)
 
 
 def on_diff():
     on_cmd_diff("on_diff", git_diff)
 
 
 def on_difftool():
-    on_cmd_diff("on_difftool", git_difftool, True)
+    # todo rework with gitutil -> git_difftool
+    on_cmd_diff("on_difftool", _run_diff_tool, True)
 
 
 def strip_non_ascii(s):
     import string
 
     rc = ""
     for c in s:
         if c in string.printable:
             rc += c
     return rc
 
 
+def ext_iter(k):
+    if "," not in k:
+        dgb_pr("found formatter ex", k)
+        yield k
+        return
+
+    for ex in k.split(","):
+        dgb_pr("found formatter ex", ex)
+        yield ex.strip()
+
+
+def elements_iter(adict, keypath=[]):
+    """deep elements iterator"""
+    def _iter(x): return x.items()
+    if type(adict) == list:
+        _iter = enumerate
+
+    for k, v in _iter(adict):
+        keypath = [*keypath, k]
+
+        if type(v) in [list, dict]:
+            yield from elements_iter(v, keypath)
+            continue
+
+        def setr(nv):
+            adict[k] = nv
+
+        yield keypath, v, setr
+
+
+def expand_all_vars(v):
+
+    for keypath, val, setr in elements_iter(v):
+        org_val = str(val)
+        val = os.path.expanduser(val)
+        # val = os.path.expandvars(val)
+        setr(val)
+
+        # todo logging
+        if org_val != val:
+            dgb_pr("expanded", val)
+
+    return v
+
+
 def read_formatter_settings():
     frmt_cfg = FileStat(fconfigdir.name).join(["formatter.json"])
     if frmt_cfg.exists() is False:
-        print("no formatter config file")
+        dgb_pr("no formatter config file")
         return None
-    print("found formatter config file")
+    dgb_pr("found formatter config file")
     with open(frmt_cfg.name) as f:
         c = f.read()
         cfg = json.loads(c)
     normdict = {}
-    for k, v in cfg.items():
-        lower_k = k.lower()
-        # todo check for double entries
-        normdict[k.lower()] = v
+    for ki, v in cfg.items():
+        for k in ext_iter(ki):
+            lower_k = k.lower()
+            # todo check for double entries
+            normdict[k.lower()] = expand_all_vars(v)
     return normdict
 
 
 def on_formatter():
     dgb_pr("on_formatter")
     sel = gt("changes").get_selection_values()
 
@@ -867,14 +952,113 @@
     file = vals[0]
     if file["unstaged"] != "":
         on_add()
     else:
         on_add_undo()
 
 
+def on_changed_context(cntrl, ctx):
+    # dgb_pr
+    print("on_changed_context", ctx)
+    global changes
+    row_no = ctx.row[1]
+    col_no = ctx.column[1]
+
+    print(changes)
+    gnam_base = changes[row_no]['git']
+    fnam_base = changes[row_no]['file']
+
+    gnam = FileStat(gws.base_repo_dir.name).join([gnam_base])
+    gnam_dir = gnam.name
+
+    fnam = FileStat(gws.base_repo_dir.name).join([gnam_base, fnam_base])
+    fnam_dir = fnam.dirname()
+    fnam_dirnam = fnam.dirname()[len(gnam.name)+1:]
+
+    dgb_pr(gnam_base, gnam)
+    dgb_pr(fnam_base, fnam)
+
+    git = gws.find(gnam)
+
+    ctxmenu = ContextMenu(cntrl._treeview, ctx)
+
+    def open_explorer(fnam):
+        def _call(x):
+            open_file_explorer(fnam)
+        return _call
+
+    ctxmenu.add_command(
+        f"open project folder {gnam_base}", open_explorer(gnam_dir))
+    if gnam_base != fnam_dirnam:
+        ctxmenu.add_command(
+            f"open file folder {fnam_dirnam}", open_explorer(fnam_dir))
+
+    load_and_set_context_settings(ctxmenu, gnam_dir, fnam_dir, fnam.name)
+    ctxmenu.show()
+
+
+def replace_all_vars(d, env):
+
+    for keypath, val, setr in elements_iter(d):
+        org_val = str(val)
+        for k, v in env.items():
+            if type(val) == str:
+                val = val.replace(k, v)
+                val = os.path.expanduser(val)
+                setr(val)
+
+    return d
+
+
+def load_and_set_context_settings(ctxmenu, gnam_dir, fnam_dir, fnam):
+    ctx_cfg = FileStat(fconfigdir.name).join(["context.json"])
+    if ctx_cfg.exists() is False:
+        dgb_pr("no context config file")
+        return None
+
+    try:
+        with open(ctx_cfg.name) as f:
+            c = f.read()
+            cfg = json.loads(c)
+    except:
+        dgb_pr("json parsing error")
+        return
+
+    env = {"$GIT": gnam_dir, "$PATH": fnam_dir, "$FILE": fnam}
+
+    cfg = replace_all_vars(cfg, env)
+    dgb_pr(cfg)
+
+    for _, ctxset in cfg.items():
+
+        patnli = ctxset["expr"]
+        if patnli:
+            patnli = patnli if type(patnli) == list else [patnli]
+            found = False
+            for patn in patnli:
+                found = fnmatch.fnmatch(fnam, patn)
+                if found:
+                    break
+            if found is False:
+                continue
+
+        ctxmenu.add_separator()
+        for mi in ctxset["menu"]:
+            def _run(args):
+                def _runner(x):
+                    if args is None or len(args) == 0:
+                        return
+                    dgb_pr(*args)
+                    rc = os.spawnvpe(os.P_NOWAIT, args[0], args, os.environ)
+                    dgb_pr("call result", rc)
+                return _runner
+            ctxmenu.add_command(
+                mi[0], _run(mi[1]))
+
+
 fcommit = FileStat(fconfigdir.name).join(["commit.json"])
 commit_history = []
 
 
 def read_commit():
     global commit_history
     try:
```

### Comparing `gitonic-0.0.13/gitonic/main.py` & `gitonic-0.0.14/gitonic/main.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/gitonic/pyjsoncfg.py` & `gitonic-0.0.14/gitonic/pyjsoncfg.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/gitonic/singleinstance.py` & `gitonic-0.0.14/gitonic/singleinstance.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/gitonic/task.py` & `gitonic-0.0.14/gitonic/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             proc.wait()
 
             if proc.returncode == 0:
                 return
             return proc.returncode
 
         else:
+            print("no proc", file=sys.stderr)
             rc = 1
 
     except Exception as ex:
         rc = ex
 
     return rc
 
@@ -115,15 +116,16 @@
         pass
 
     def _loopcb(self, p):
         if self._stop_req:
             return self._stop_req
 
     def run(self):
-        rc = run_proc(self._cmd, callb=self._callb, loopcallb=self._loopcb, shell=True)
+        rc = run_proc(self._cmd, callb=self._callb,
+                      loopcallb=self._loopcb, shell=True)
         return rc
 
 
 class CmdTask(Cmd, Task):
     def start(self):
         if self._callb is None:
             self.set_callb(self._append_rc)
```

### Comparing `gitonic-0.0.13/gitonic/tile/core.py` & `gitonic-0.0.14/gitonic/tile/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
     (c)2021 K. Goger - https://github.com/kr-g
     legal: https://github.com/kr-g/gitonic/blob/main/LICENSE.md
 """
 
 
+from tkinter import Tk, ttk, filedialog, scrolledtext
+from tktooltip import ToolTip
+from tkinter import *
 import os
 
 # loggin support
 
 import logging
 
 enableLogging = logging.DEBUG
@@ -41,18 +44,14 @@
 
 def print_e(*args):
     _log(logging.CRITICAL, args)
 
 
 #
 
-from tkinter import *
-from tktooltip import ToolTip
-
-from tkinter import Tk, ttk, filedialog, scrolledtext
 
 CAPTION = "caption"
 
 VALUE = "value"
 VALUES = "values"
 MAP_VALUE = "map_value"
 SOURCE = "source"
@@ -186,15 +185,15 @@
     def _init_frame(self):
         if self.frame != None:
             raise Exception("frame alive")
         p = self.parent_frame()
 
         # opts = { "borderwidth":2,  "relief":"ridge" }  ##todo debug
 
-        self.frame = ttk.Frame(p)  ## **opts
+        self.frame = ttk.Frame(p)  # **opts
 
     def _end_frame(self):
         # todo rename this ...
         self.destroy()
 
     def layout(self):
         self._end_frame()
@@ -647,15 +646,16 @@
         if sel_idx != None:
             self.set_index(sel_idx)
 
         return vars
 
     def _create_entry(self):
         width = self.pref_int("width", 20)
-        self._combo = ttk.Combobox(self.frame, textvariable=self._var, width=width)
+        self._combo = ttk.Combobox(
+            self.frame, textvariable=self._var, width=width)
         self._combo.bind("<<ComboboxSelected>>", self._handler)
 
         self._bind_focus(self._combo)
 
         return self._combo
 
     def _handler(self, event):
@@ -704,19 +704,19 @@
         self._auto_scrollb = int(self.pref("max_show", 5))
         vals = self.pref(VALUES, [])
         self._values = list(vals if vals else [])
 
         self._width = int(self.pref("width", 20))
 
         self._sel_mode = int(self.pref("select_many", False))
-        ##todo self._height = int(self.pref("height", 5))
+        # todo self._height = int(self.pref("height", 5))
 
     def destroy(self):
         super().destroy()
-        ## init tile (move?)
+        # init tile (move?)
         self._lastsel = None
 
     def scrollbar(self, enable=True):
         self._scrollable = enable
         return self
 
     def set_values(self, values):
@@ -932,15 +932,16 @@
         self._spinb.bind("<<Decrement>>", self._change_handler)
         return self._spinb
 
     def _change_handler(self, event):
         self.pref(ON_CHANGE, self.on_change)()
 
     def on_change(self):
-        print_t(self.__class__.__name__, ON_CHANGE, self.get_index(), self.get_val())
+        print_t(self.__class__.__name__, ON_CHANGE,
+                self.get_index(), self.get_val())
 
     def get_index(self):
         return self._map_values.index(self.get_val())
 
     def get_val(self):
         return self._spinb.get()
 
@@ -1164,15 +1165,46 @@
 
     def focus_first_active_tab(self):
         print_t("cur sel tab", self._tab_sel)
         el = self._elem[self._tab_sel]
         el.focus()
 
 
+class ContextMenu(object):
+
+    def __init__(self, root, ctx):
+        self.root = root
+        self.ctx = ctx
+        self._menu = Menu(root, tearoff=0)
+        self._menu.bind("<Leave>", lambda x: self.hide())
+
+    def hide(self):
+        self._menu.destroy()
+        self._menu = None
+
+    def add_separator(self):
+        self._menu.add_separator()
+
+    def add_command(self, caption, cmdfunc, args=None):
+        def _call(args):
+            self.hide()
+            if cmdfunc:
+                cmdfunc(args)
+        self._menu.add_command(label=caption, command=lambda: _call(args))
+
+    def show(self):
+        self._menu.post(self.ctx.x_root, self.ctx.y_root)
+
+
 class TileTreeView(Tile):
+
+    class Context(object):
+        def __repr__(self):
+            return str(self.__dict__)
+
     def create_element(self):
         header = self.pref("header", [])
         header_width = self.pref("header_width", [])
         height = self.pref("height", None)
 
         self.header_name = []
         self.header_title = []
@@ -1189,14 +1221,15 @@
             self._cont,
             columns=self.header_name,
             show="headings",
             height=height,
         )
         self._treeview.bind("<<TreeviewSelect>>", self._select_handler)
         self._treeview.bind("<Double-1>", self._on_double_handler)
+        self._treeview.bind("<3>", self._tree_context_menu)
 
         self._yscroll = ttk.Scrollbar(
             self._cont, orient="vertical", command=self._treeview.yview
         )
         self._treeview.configure(yscrollcommand=self._yscroll.set)
 
         self._treeview.pack(side="left")
@@ -1236,14 +1269,55 @@
         )
 
         sel = self._treeview.focus()
         sel = self._treeview.item(sel)
 
         nullable = self.pref("nullable", True)
 
+    def _tree_context_menu(self, ev):
+        ctx = self._context_from_event(ev)
+        # selected = self._treeview.selection()
+        # print("right-click", ctx, ctx.iid in selected)
+        self.pref(ON_RIGHT_CLICK, self.on_right_click)(self, ctx)
+
+    def on_right_click(self, cntrl, ctx):
+        pass
+
+    def _context_from_event(self, ev):
+
+        ctx = self.Context()
+
+        xp = ctx.x = ev.x
+        yp = ctx.y = ev.y
+        ctx.button = ev.num
+
+        ctx.x_root = ev.x_root
+        ctx.y_root = ev.y_root
+
+        widg = self._treeview
+
+        ctx.region = widg.identify("region", xp, yp)
+        # CHECK region for heading or tree
+
+        ctx.iid = widg.identify("item", xp, yp)
+
+        ctx.row = ctx.iid, widg.index(ctx.iid)
+        ctx.column = widg.identify("column", xp, yp)
+
+        if ctx.column.startswith("#"):
+            no = int(ctx.column[1:])-1
+            nam = widg["columns"][no-1] if no > 0 else ctx.column
+            ctx.column = (ctx.column, no, nam)
+        else:
+            print("error in column", ctx)
+
+        ctx.isopen = widg.item(ctx.iid, "open")
+
+        return ctx
+
     def clear(self):
         self._treeview.delete(*self._treeview.get_children())
 
     def set_values(self, values, mapval=True):
         print("set_values", values)
         self._values = values
         self._iid = []
```

### Comparing `gitonic-0.0.13/gitonic/tile/tkcmd.py` & `gitonic-0.0.14/gitonic/tile/tkcmd.py`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/gitonic.egg-info/PKG-INFO` & `gitonic-0.0.14/gitonic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitonic
-Version: 0.0.13
+Version: 0.0.14
 Summary: manage a multi git workspace
 Home-page: https://github.com/kr-g/gitonic
 Author: k. goger
 Author-email: k.r.goger+gitonic@gmail.com
 License: AGPLv3+
 Keywords: python utility shell git git-workspace tkinter
 Platform: UNKNOWN
@@ -25,27 +25,24 @@
 Provides-Extra: PEP08_BLACK
 Provides-Extra: PEP08_FULL
 License-File: LICENSE.md
 
 [![PEP-08](https://img.shields.io/badge/code%20style-PEP08-green.svg)](https://www.python.org/dev/peps/pep-0008/)
 
 
-you are reading VERSION = v0.0.13
+you are reading VERSION = v0.0.14
 
 
 # gitonic 
 
 gitonic simplifies working with multiple git repositories.
 
 
 gitonic comes with an easy to use Tkinter GUI.
 
-there is also a plugin for thonny 
-[`thonny-gitonic`](https://github.com/kr-g/thonny-gitonic) 
-
 
 # background 
 
 where software components/ artefacts are stored in multiple repositories 
 separately gitonic helps to keep track
 
 
@@ -156,15 +153,19 @@
         "cmd": "full-path-to-command",
         "para": [
           "%file"
         ]
       }
     }
 
-here `para` is an array of cmd-line options passed to the formatter command
+where `.file-ext` is a simple file extension such as `.py`, 
+or a comma separated list of extensions `.c,.h,.cpp`.
+wild-cards are not supported.
+
+where `para` is an array of cmd-line options passed to the formatter command
 where `%file` is a placeholder and replaced by the file name
 
 for different file extensions `gitonic` will call the formatter accordingly 
 even if the selected files are of different types (extensions)
 
 
 ## templates for python pep08 formatters
@@ -187,14 +188,28 @@
         "para": [
           "-i",
           "%file"
         ]
       }
     }
 
+to use the same code formatter also for 
+[`cython's`](https://github.com/cython/cython) 
+files with extension `.pyx` change the setting to
+
+    {
+      ".py,.pyx": {
+        "cmd": "autopep8",
+        "para": [
+          "-i",
+          "%file"
+        ]
+      }
+    }
+
 
 ### black
 
 black is also an offical python tool, but resolves not fully to issues reported by pycodestyle.
 there might be some rework required (from case to case). 
 result is quite similar to autopep8 beside the list reported by pycodestyle (after formatting) 
 is a bit longer comparing to autopep8 what does a better job here.
@@ -221,14 +236,171 @@
           "-i",
           "%file"
         ]
       }
     }
 
 
+## templates for c, c++ formatters
+
+all of the following tools are NOT part of `gitonic` standard installation. 
+
+
+### uncrustify
+
+[`uncrustify`](https://github.com/uncrustify/uncrustify) 
+is a code formatter for c, c++ (and other languages).
+
+here in this config sample it is configured for extensions `.c`, `.h`, and `.cpp`.
+
+IMPORTANT: `uncrustify` requires an additional config file, a sample can be found here
+[`uncrustify.cfg`](https://github.com/uncrustify/uncrustify/blob/master/forUncrustifySources.cfg)
+
+here in the sample the `uncrustify` config file is placed in path `~/.gitonic/uncrustify.cfg`.
+make sure that it is there.
+
+the following needs to be placed inside `~/.gitonic/formatter.json`
+
+
+    ".c,.h,.cpp": {
+        "cmd": "uncrustify",
+        "para": [
+              "-c",
+              "~/.gitonic/uncrustify.cfg",
+              "--replace",
+              "%file",
+              "--no-backup",
+              "--if-changed"
+        ]
+    }
+
+
+# custom context menu handler 
+
+when clicking on the `changes` tab right a context memu opens offering 
+to open the system file manager tool (file explorer) 
+at the base git repo path or at the changed file path.
+
+in addition it is possible to add own custom context menu entries here.
+configuration is done with `~/.gitonic/context.json` file.
+
+the general structure is:
+
+    {
+      "a-context-name-ctx": {
+        "expr": "*",
+        "menu": [
+          [
+            "some text $GIT",
+            [
+              "cmd-path",
+              "whatever_param=$GIT"
+            ]
+          ],
+          [
+            "some other text $PATH",
+            [
+              "cmd-path2",
+              "whatever_param=$PATH"
+            ]
+          ]
+        ]
+      },
+      ...
+    }
+
+
+here the variables `$GIT`, `$PATH`, or `$FILE` are replaced 
+by the corrosponding path before execution.
+
+the `expr` key contains a single file pattern, or a list of 
+file patterns - when to enable the context menu. 
+the file pattern is following Unix filename pattern matching.
+
+the `menu` array contains the text to display in the menu, 
+and the command params as embedded array.
+
+the context name as such can have any value 
+(as long it is unique in the structure).
+
+
+below a sample `~/.gitonic/context.json` file 
+for running on linux with xfce.
+
+    {
+      "term-ctx": {
+        "expr": "*",
+        "menu": [
+          [
+            "Open Terminal at $GIT",
+            [
+              "xfce4-terminal",
+              "--working-directory=$GIT"
+            ]
+          ],
+          [
+            "Open Terminal at $PATH",
+            [
+              "xfce4-terminal",
+              "--working-directory=$PATH"
+            ]
+          ],
+          [
+            "Edit .gitignore at $GIT",
+            [
+              "xed",
+              "$GIT/.gitignore"
+            ]
+          ]
+        ]
+      },
+      "spyder-ctx": {
+        "expr": "*.py",
+        "menu": [
+          [
+            "spyder python $FILE",
+            [
+              "~/spyder/.venv/bin/spyder",
+              "$FILE"
+            ]
+          ]
+        ]
+      },
+      "geany-ctx": {
+        "expr": [
+          "*.c",
+          "*.cpp",
+          "*.h"
+        ],
+        "menu": [
+          [
+            "geany c $FILE",
+            [
+              "geany",
+              "$FILE"
+            ]
+          ]
+        ]
+      }
+    }
+
+
+remark:
+the sample config file provides support for opening
+- terminal, in this case `xfce4-terminal`, can be replaced by e.g. `xterm` - depending on your distribution
+- `.gitignore` file for selected repo with [`xed`](https://en.wikipedia.org/wiki/Xed)
+- [`spyder-ide.org`](https://spyder-ide.org/), for files matching `*.py`
+- [`geany`](https://www.geany.org/), for files matching `*.c`, `*.cpp`, `*.h`
+
+
+**limitation:**
+
+at the present time the context menu only works on the underlying file (row) in the table.
+there is **no** support for multiple files (selection) as of now.
+
 
 
 # platform
 
 tested on python3, and linux
 
 
@@ -315,15 +487,15 @@
 when during startup an error is thrown, refer to 
 [installation on raspberry, fedorra](https://github.com/kr-g/gitonic/issues/6)
 
 
 # git configuration
 
 add a `.git-credentials` file as described here 
-[`git-credentials`](https://git-scm.com/docs/git-credential-store#_storage_format)
+[`git-credentials`](https://git-scm.com/docs/git-credential-store)
 
 
 add a `.gitconfig` file as described here
 [`git-config`](https://git-scm.com/docs/git-config)
 and configure for diff and merge tools. 
 NOTE: you need to install the diff-tool e.g. 
 [`meld merge`](https://meldmerge.org/) manually, 
@@ -338,22 +510,22 @@
         helper = store
 
     [diff]
         tool = meld
     [difftool]
         prompt = false
     [difftool "meld"]
-        cmd = meld "$LOCAL" "$REMOTE"
+        cmd = meld --newtab "$LOCAL" "$REMOTE"
 
     [merge]
         tool = meld
     [mergetool "meld"]
         # Choose one of these 2 lines (not both!) 
         # cmd = meld "$LOCAL" "$MERGED" "$REMOTE" --output "$MERGED"
-        cmd = meld "$LOCAL" "$BASE" "$REMOTE" --output "$MERGED"
+        cmd = meld --newtab "$LOCAL" "$BASE" "$REMOTE" --output "$MERGED"
 
 
 # additional notes 
 
 the following tools are part of the standard git distribution 
 
 - [`gitk`](https://git-scm.com/docs/gitk)
@@ -367,17 +539,18 @@
 # internals
 
 following files are used:
 
 |file|description|
 |---|---|
 |~/.gitonic/commit.json|the last commit messages show in the combo box|
-|~/.gitonic/tracked.json|tracked git repositories|
 |~/.gitonic/config.json|configuration settings|
+|~/.gitonic/context.json|configuration for context menu on changes tab|
 |~/.gitonic/formatter.json|configuration for external formatter tools|
+|~/.gitonic/tracked.json|tracked git repositories|
 |~/.gitonic/socket|internal use|
 
 
 HINT:
 crash after configuration change can be resolved by changing the setting manually 
 in `config.json`, or delete the config file to fall back to the defaults
 
@@ -385,19 +558,36 @@
 # license
 
 gitonic is released under the following
 [`LICENSE`](https://github.com/kr-g/gitonic/blob/main/LICENSE.md)
 
 
 
-
+ 
 # Changelog
 
 
-# next version v0.0.13 - 20231125
+# version v0.0.14 - 20240518
+
+- improved formatter 
+  - support for multiple file extension for single config entry 
+  - support for path expansion for formatter config
+  - added sample for uncrustify (c, c++)
+- on "changes" tab
+  - added context menu to open file system explorer
+  - added support for custom context menu with `~/.gitonic/context.json`
+- calling merge-tool with more then more file selected on change tab will 
+ not block the user-interface anymore since starting independent from main process
+  - **important** add `--newtab` to `meld` configuration in `.gitconfig` 
+   to re-use an already running instance of `meld`
+- context menu handler expands user path (`~`)
+- 
+
+
+# version v0.0.13 - 20231125
 
 - show all untracked files on changes tab (not only the folder)
 - 
 
 
 # version v0.0.12 - 20231111
 
@@ -570,14 +760,15 @@
 - git error handling
 - switch to log tab after pull
 - logging, use python logger for expert mode output
 - support for .gitignore 
   - adding single files 
   - open .gitignore for editing
 - execute git operations in parallel where possible
+- make expert mode debugging out better (use python logging)
 - 
 
 
 # OPEN ISSUES
 
 refer to [issues](https://github.com/kr-g/gitonic/issues)
 
@@ -593,15 +784,16 @@
  no separate credit store provided.
 - only existing git repo's under the workspace are supported,
  as of now no support to create a new git repo. 
  use `git init`, or `git clone` manually from cmd-line
 - `gitonic` interacts with `git` just like starting in bash / commandline.
 at the present time there is _no_additional_ error checking. 
 this must be done by checking the log tab manually where all cmdline output goes.
-
+- at the present time the context menu only works on the underlying file (row) in the table. 
+ there is no support for multiple files (selection) as of now.
  
 
 
 ---
 
 Copyright (c) 2022 k. goger - https://github.com/kr-g
```

### Comparing `gitonic-0.0.13/gitonic.egg-info/SOURCES.txt` & `gitonic-0.0.14/gitonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/setup.cfg` & `gitonic-0.0.14/setup.cfg`

 * *Files identical despite different names*

### Comparing `gitonic-0.0.13/setup.py` & `gitonic-0.0.14/setup.py`

 * *Files identical despite different names*


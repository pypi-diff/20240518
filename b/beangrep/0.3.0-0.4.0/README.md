# Comparing `tmp/beangrep-0.3.0.tar.gz` & `tmp/beangrep-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beangrep-0.3.0.tar", last modified: Wed May 15 16:25:44 2024, max compression
+gzip compressed data, was "beangrep-0.4.0.tar", last modified: Sat May 18 07:19:02 2024, max compression
```

## Comparing `beangrep-0.3.0.tar` & `beangrep-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/.github/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/.github/workflows/
--rw-r--r--   0 zack      (1000) zack      (1000)     1377 2024-05-13 07:53:11.000000 beangrep-0.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 zack      (1000) zack      (1000)       81 2024-05-14 12:58:05.000000 beangrep-0.3.0/.gitignore
--rw-r--r--   0 zack      (1000) zack      (1000)      651 2024-05-14 13:14:24.000000 beangrep-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 zack      (1000) zack      (1000)    18092 2024-05-12 10:30:41.000000 beangrep-0.3.0/LICENSE-GPL-2.0-or-later
--rw-r--r--   0 zack      (1000) zack      (1000)     8732 2024-05-15 16:25:44.358443 beangrep-0.3.0/PKG-INFO
--rw-r--r--   0 zack      (1000) zack      (1000)     7659 2024-05-15 16:22:59.000000 beangrep-0.3.0/README.md
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/bin/
--rwxr-xr-x   0 zack      (1000) zack      (1000)      308 2024-05-12 10:30:41.000000 beangrep-0.3.0/bin/bean-grep
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/dev/
--rwxr-xr-x   0 zack      (1000) zack      (1000)      562 2024-05-15 16:22:56.000000 beangrep-0.3.0/dev/update_readme.sh
--rw-r--r--   0 zack      (1000) zack      (1000)     1177 2024-05-14 13:31:36.000000 beangrep-0.3.0/pyproject.toml
--rw-r--r--   0 zack      (1000) zack      (1000)       38 2024-05-15 16:25:44.358443 beangrep-0.3.0/setup.cfg
--rw-r--r--   0 zack      (1000) zack      (1000)      259 2024-05-12 10:30:41.000000 beangrep-0.3.0/setup.py
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/src/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/src/beangrep/
--rw-r--r--   0 zack      (1000) zack      (1000)      263 2024-05-12 10:30:41.000000 beangrep-0.3.0/src/beangrep/__init__.py
--rw-r--r--   0 zack      (1000) zack      (1000)      284 2024-05-12 10:30:41.000000 beangrep-0.3.0/src/beangrep/__main__.py
--rw-r--r--   0 zack      (1000) zack      (1000)    32938 2024-05-15 16:14:19.000000 beangrep-0.3.0/src/beangrep/beangrep.py
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/src/beangrep.egg-info/
--rw-r--r--   0 zack      (1000) zack      (1000)     8732 2024-05-15 16:25:44.000000 beangrep-0.3.0/src/beangrep.egg-info/PKG-INFO
--rw-r--r--   0 zack      (1000) zack      (1000)      510 2024-05-15 16:25:44.000000 beangrep-0.3.0/src/beangrep.egg-info/SOURCES.txt
--rw-r--r--   0 zack      (1000) zack      (1000)        1 2024-05-15 16:25:44.000000 beangrep-0.3.0/src/beangrep.egg-info/dependency_links.txt
--rw-r--r--   0 zack      (1000) zack      (1000)       43 2024-05-15 16:25:44.000000 beangrep-0.3.0/src/beangrep.egg-info/entry_points.txt
--rw-r--r--   0 zack      (1000) zack      (1000)      102 2024-05-15 16:25:44.000000 beangrep-0.3.0/src/beangrep.egg-info/requires.txt
--rw-r--r--   0 zack      (1000) zack      (1000)        9 2024-05-15 16:25:44.000000 beangrep-0.3.0/src/beangrep.egg-info/top_level.txt
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/tests/
-drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-15 16:25:44.358443 beangrep-0.3.0/tests/data/
--rw-r--r--   0 zack      (1000) zack      (1000)   347380 2024-05-14 09:41:00.000000 beangrep-0.3.0/tests/data/example.beancount
--rw-r--r--   0 zack      (1000) zack      (1000)    17754 2024-05-15 16:03:31.000000 beangrep-0.3.0/tests/test_beangrep.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.558627 beangrep-0.4.0/
+-rw-r--r--   0 zack      (1000) zack      (1000)       56 2024-05-17 15:18:49.000000 beangrep-0.4.0/.coveragerc
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/.github/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/.github/workflows/
+-rw-r--r--   0 zack      (1000) zack      (1000)     1377 2024-05-13 07:53:11.000000 beangrep-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zack      (1000) zack      (1000)      111 2024-05-17 16:21:49.000000 beangrep-0.4.0/.gitignore
+-rw-r--r--   0 zack      (1000) zack      (1000)      651 2024-05-14 13:14:24.000000 beangrep-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 zack      (1000) zack      (1000)    18092 2024-05-12 10:30:41.000000 beangrep-0.4.0/LICENSE-GPL-2.0-or-later
+-rw-r--r--   0 zack      (1000) zack      (1000)      977 2024-05-18 07:16:41.000000 beangrep-0.4.0/Makefile
+-rw-r--r--   0 zack      (1000) zack      (1000)     8860 2024-05-18 07:19:02.558627 beangrep-0.4.0/PKG-INFO
+-rw-r--r--   0 zack      (1000) zack      (1000)     7787 2024-05-18 07:17:44.000000 beangrep-0.4.0/README.md
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/bin/
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      308 2024-05-12 10:30:41.000000 beangrep-0.4.0/bin/bean-grep
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/data/
+-rw-r--r--   0 zack      (1000) zack      (1000)      397 2024-05-17 16:21:49.000000 beangrep-0.4.0/data/man-extras.h2m
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/dev/
+-rwxr-xr-x   0 zack      (1000) zack      (1000)       63 2024-05-17 15:23:37.000000 beangrep-0.4.0/dev/coverage
+-rwxr-xr-x   0 zack      (1000) zack      (1000)      562 2024-05-17 15:23:37.000000 beangrep-0.4.0/dev/update-readme
+-rw-r--r--   0 zack      (1000) zack      (1000)     1243 2024-05-17 16:21:49.000000 beangrep-0.4.0/pyproject.toml
+-rw-r--r--   0 zack      (1000) zack      (1000)       38 2024-05-18 07:19:02.558627 beangrep-0.4.0/setup.cfg
+-rw-r--r--   0 zack      (1000) zack      (1000)      259 2024-05-12 10:30:41.000000 beangrep-0.4.0/setup.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/src/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/src/beangrep/
+-rw-r--r--   0 zack      (1000) zack      (1000)      263 2024-05-12 10:30:41.000000 beangrep-0.4.0/src/beangrep/__init__.py
+-rw-r--r--   0 zack      (1000) zack      (1000)      284 2024-05-12 10:30:41.000000 beangrep-0.4.0/src/beangrep/__main__.py
+-rw-r--r--   0 zack      (1000) zack      (1000)    33230 2024-05-18 07:03:01.000000 beangrep-0.4.0/src/beangrep/beangrep.py
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/src/beangrep/data/
+-rw-r--r--   0 zack      (1000) zack      (1000)        0 2024-05-17 16:21:49.000000 beangrep-0.4.0/src/beangrep/data/.gitkeep
+-rw-r--r--   0 zack      (1000) zack      (1000)     4894 2024-05-18 07:19:01.000000 beangrep-0.4.0/src/beangrep/data/bean-grep.1
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.558627 beangrep-0.4.0/src/beangrep.egg-info/
+-rw-r--r--   0 zack      (1000) zack      (1000)     8860 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/PKG-INFO
+-rw-r--r--   0 zack      (1000) zack      (1000)      681 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/SOURCES.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)        1 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/dependency_links.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)       43 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/entry_points.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)      102 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/requires.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)        9 2024-05-18 07:19:02.000000 beangrep-0.4.0/src/beangrep.egg-info/top_level.txt
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/tests/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/tests/data/
+drwxr-xr-x   0 zack      (1000) zack      (1000)        0 2024-05-18 07:19:02.554628 beangrep-0.4.0/tests/data/documents/
+-rw-r--r--   0 zack      (1000) zack      (1000)       40 2024-05-18 07:03:01.000000 beangrep-0.4.0/tests/data/documents/statements.txt
+-rw-r--r--   0 zack      (1000) zack      (1000)   347380 2024-05-14 09:41:00.000000 beangrep-0.4.0/tests/data/example.beancount
+-rw-r--r--   0 zack      (1000) zack      (1000)      977 2024-05-18 07:03:01.000000 beangrep-0.4.0/tests/data/small.beancount
+-rw-r--r--   0 zack      (1000) zack      (1000)    18680 2024-05-18 07:03:01.000000 beangrep-0.4.0/tests/test_beangrep.py
```

### Comparing `beangrep-0.3.0/.github/workflows/python-package.yml` & `beangrep-0.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `beangrep-0.3.0/.pre-commit-config.yaml` & `beangrep-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beangrep-0.3.0/LICENSE-GPL-2.0-or-later` & `beangrep-0.4.0/LICENSE-GPL-2.0-or-later`

 * *Files identical despite different names*

### Comparing `beangrep-0.3.0/PKG-INFO` & `beangrep-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangrep
-Version: 0.3.0
+Version: 0.4.0
 Summary: Grep-like filter for the Beancount plain text accounting system
 Author-email: Stefano Zacchiroli <zack@upsilon.cc>
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/zacchiro/beangrep
 Project-URL: Issues, https://github.com/zacchiro/beangrep/issues
 Keywords: accounting,beancount,grep,ledger,plaintext,plaintext-accounting
 Classifier: Programming Language :: Python :: 3
@@ -75,22 +75,23 @@
 
 Usage
 -----
 
 The CLI says it all when invoked as `bean-grep --help`:
 
 ```
-Usage: bean-grep [OPTIONS] [PATTERN] FILENAME
+Usage: bean-grep [OPTIONS] [PATTERN] FILENAME...
 
-  Search for entries matching given criteria in a Beancount ledger. Pretty
+  Search for entries matching given criteria in Beancount journals. Pretty
   print matching entries to standard output.
 
   Search criteria can be specified with the options below and/or providing an
   explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
   date (if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"),
+  account (start with an account type, e.g., "Assets", "Income", etc.),
   metadata pair ("key:value"), or string to be matched anywhere (see
   -s/--somewhere below), in this order. If PATTERN is not given, search
   criteria are defined by explicit options.
 
   Multiple options and/or PATTERN are logically joined (AND-ed) together. In
   case of overlap, explicit options override PATTERN.
 
@@ -151,28 +152,29 @@
                                   types. [default: transaction]
   -i, --ignore-case / --no-ignore-case
                                   Ignore case distinctions in string matches.
                                   [default: no-ignore-case]
   --posting-tags-meta TEXT        Metadata key used to attach tags to
                                   transaction postings.  [default: tags]
   -q, --quiet / --no-quiet        Quiet, do not write anything to standard
-                                  output. Exit succesfully immediately if any
+                                  output. Exit successfully immediately if any
                                   match is found.  [default: no-quiet]
   --skip-internals / --no-skip-internals
                                   When matching, ignore internal information
                                   not visible in the ledger. This includes the
                                   automatic metadata: ['filename', 'lineno']
                                   [default: skip-internals]
-  -v, --verbose                   Increase logging verbosity. Default level is
-                                  WARNING. Passing this option once (e.g., -v)
-                                  will increase it to INFO, twice or more
-                                  (e.g., -vv) to DEBUG.
+  --verbose                       Increase logging verbosity. Default
+                                  verbosity is at WARNING level; passing this
+                                  option once will increase it to INFO, twice
+                                  or more to DEBUG.
+  -V, --version                   Show the version and exit.
   --help                          Show this message and exit.
 
-  Exit status is 0 (sucess) if a match is found, 1 if no match is found, 2 if
+  Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
   an error occurred.
 ```
 
 
 Author
 ------
```

### Comparing `beangrep-0.3.0/README.md` & `beangrep-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,23 @@
 
 Usage
 -----
 
 The CLI says it all when invoked as `bean-grep --help`:
 
 ```
-Usage: bean-grep [OPTIONS] [PATTERN] FILENAME
+Usage: bean-grep [OPTIONS] [PATTERN] FILENAME...
 
-  Search for entries matching given criteria in a Beancount ledger. Pretty
+  Search for entries matching given criteria in Beancount journals. Pretty
   print matching entries to standard output.
 
   Search criteria can be specified with the options below and/or providing an
   explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
   date (if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"),
+  account (start with an account type, e.g., "Assets", "Income", etc.),
   metadata pair ("key:value"), or string to be matched anywhere (see
   -s/--somewhere below), in this order. If PATTERN is not given, search
   criteria are defined by explicit options.
 
   Multiple options and/or PATTERN are logically joined (AND-ed) together. In
   case of overlap, explicit options override PATTERN.
 
@@ -125,28 +126,29 @@
                                   types. [default: transaction]
   -i, --ignore-case / --no-ignore-case
                                   Ignore case distinctions in string matches.
                                   [default: no-ignore-case]
   --posting-tags-meta TEXT        Metadata key used to attach tags to
                                   transaction postings.  [default: tags]
   -q, --quiet / --no-quiet        Quiet, do not write anything to standard
-                                  output. Exit succesfully immediately if any
+                                  output. Exit successfully immediately if any
                                   match is found.  [default: no-quiet]
   --skip-internals / --no-skip-internals
                                   When matching, ignore internal information
                                   not visible in the ledger. This includes the
                                   automatic metadata: ['filename', 'lineno']
                                   [default: skip-internals]
-  -v, --verbose                   Increase logging verbosity. Default level is
-                                  WARNING. Passing this option once (e.g., -v)
-                                  will increase it to INFO, twice or more
-                                  (e.g., -vv) to DEBUG.
+  --verbose                       Increase logging verbosity. Default
+                                  verbosity is at WARNING level; passing this
+                                  option once will increase it to INFO, twice
+                                  or more to DEBUG.
+  -V, --version                   Show the version and exit.
   --help                          Show this message and exit.
 
-  Exit status is 0 (sucess) if a match is found, 1 if no match is found, 2 if
+  Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
   an error occurred.
 ```
 
 
 Author
 ------
```

### Comparing `beangrep-0.3.0/dev/update_readme.sh` & `beangrep-0.4.0/dev/update-readme`

 * *Files identical despite different names*

### Comparing `beangrep-0.3.0/pyproject.toml` & `beangrep-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -45,8 +45,11 @@
     "flake8>=5",
     "mypy>=1",
     "pre-commit",
     "pytest>=7.2",
     "pytest-cov>=4",
 ]
 
+[tool.setuptools.package-data]
+"beangrep.data" = ["bean-grep.1"]
+
 [tool.setuptools_scm]
```

### Comparing `beangrep-0.3.0/src/beangrep/beangrep.py` & `beangrep-0.4.0/src/beangrep/beangrep.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,26 +256,29 @@
         """Guess criteria from a single textual pattern, using heuristics.
 
         Heuristics (ordered by priority):
 
         - "YYYY-MM-DD" -> date criteria
         - "#tag" -> tag criteria
         - "^link" -> link criteria
+        - starting with an account type (Assets, Liabilities, etc.) -> account criteria
         - "key:value" -> metadata criteria
         - default -> somewhere criteria
 
         """
         criteria = base if base is not None else cls()
 
         if re.search(r"^\d{4}-\d{2}-\d{2}$", pattern):
             criteria.date = [DatePredicate.parse(f"={pattern}")]
         elif re.search(r"^#[-\w]+$", pattern):
             criteria.tag = cls._re_compile(ignore_case, pattern[1:])
         elif re.search(r"^\^[-\w]+$", pattern):
             criteria.link = cls._re_compile(ignore_case, pattern[1:])
+        elif re.search(r"^(Assets|Liabilities|Equity|Income|Expenses)", pattern):
+            criteria.account = cls._re_compile(ignore_case, pattern)
         elif m := re.search(r"(?P<key>\w+):(?P<val>\w+)$", pattern):
             matches = m.groupdict()
             criteria.metadata = (
                 cls._re_compile(ignore_case, matches["key"]),
                 cls._re_compile(ignore_case, matches["val"]),
             )
         else:
@@ -689,41 +692,42 @@
             logging.debug("Entry %s matches criteria, keeping it", entry)
             yield entry
         else:
             logging.debug("Entry %s does not match criteria, skipping it", entry)
 
 
 @click.command(
-    help="Search for entries matching given criteria in a Beancount ledger. "
+    help="Search for entries matching given criteria in Beancount journals. "
     "Pretty print matching entries to standard output."
     "\n\n"
     "Search criteria can be specified with the options below and/or providing an "
     'explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a date '
-    '(if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"), metadata '
-    'pair ("key:value"), or string to be matched anywhere (see -s/--somewhere below), '
+    '(if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"), account '
+    '(start with an account type, e.g., "Assets", "Income", etc.), metadata pair '
+    '("key:value"), or string to be matched anywhere (see -s/--somewhere below), '
     "in this order. "
     "If PATTERN is not given, search criteria are defined by explicit options. "
     "\n\n"
     "Multiple options and/or PATTERN are logically joined (AND-ed) together. "
     "In case of overlap, explicit options override PATTERN. "
     "\n\n"
     "The granularity of matching (and results) is that of individual entries, e.g., "
     "full transactions, balances, notes, etc. By default only transactions are returned"
     "; use the --type/-T option to override."
     "\n\n"
     'To read from standard input, pass "-" as FILENAME, but beware that it implies '
     "on-disk buffering of stdin.",
-    epilog="Exit status is 0 (sucess) if a match is found, "
+    epilog="Exit status is 0 (success) if a match is found, "
     "1 if no match is found, 2 if an error occurred.",
 )
-@click.argument("pattern", required=False)
 @click.argument(
-    "filename",
-    required=False,
-    metavar="FILENAME",  # override metavar to show this as actually required
+    "args",
+    required=True,
+    nargs=-1,
+    metavar="[PATTERN] FILENAME...",  # override metavar to show what is required
 )
 @click.option(
     "--account",
     "-a",
     "account_re",
     metavar="REGEX",
     help="Only return entries referencing accounts with names matching given regex.",
@@ -830,38 +834,36 @@
 @click.option(
     "--quiet/--no-quiet",
     "-q",
     "quiet",
     default=False,
     show_default=True,
     help="Quiet, do not write anything to standard output. "
-    "Exit succesfully immediately if any match is found.",
+    "Exit successfully immediately if any match is found.",
 )
 @click.option(
     "--skip-internals/--no-skip-internals",
     "skip_internals",
     default=True,
     show_default=True,
     help="When matching, ignore internal information not visible in the ledger. "
     f"This includes the automatic metadata: {sorted(INTERNALS_META)}",
 )
 @click.option(
-    "-v",
     "--verbose",
     count=True,
     help="Increase logging verbosity. "
-    "Default level is WARNING. "
-    "Passing this option once (e.g., -v) will increase it to INFO, "
-    "twice or more (e.g., -vv) to DEBUG.",
+    "Default verbosity is at WARNING level; "
+    "passing this option once will increase it to INFO, twice or more to DEBUG.",
 )
+@click.version_option(None, "--version", "-V")
 @click.pass_context
 def cli(
     ctx,
-    pattern,
-    filename,
+    args,
     account_re,
     amount_preds,
     date_preds,
     link_re,
     metadata_pat,
     narration_re,
     payee_re,
@@ -879,40 +881,22 @@
             log_level = logging.WARNING
         case 1:
             log_level = logging.INFO
         case _:  # >= 2
             log_level = logging.DEBUG
     logging.basicConfig(level=log_level)
 
-    if filename is None and pattern is not None:
-        # Usage is "bean-grep [PATTERN] FILENAME", with both PATTERN and FILENAME
-        # declared as optional for click. Click assigns arguments to variables
-        # sequentially from left to right, so when only one is given, it is interpreted
-        # as PATTERN, rather than FILENAME. We hence swap them here.
-        (pattern, filename) = (filename, pattern)
-
-    if filename is None:  # Manual check, as we want filename to be required=False
-        raise click.UsageError("Missing argument 'FILENAME'.")
-    elif filename == "-":
-        # Beancount does not support streaming reading, so to mimic Unix filter
-        # semantics we read stdin to the end and store it to a temporary file.
-        with NamedTemporaryFile(prefix="beangrep.", suffix=".beancount") as tmpfile:
-            logging.info("Buffering stdin to temporary file %s...", tmpfile.name)
-            shutil.copyfileobj(sys.stdin.buffer, tmpfile.file)
-            tmpfile.flush()
-            logging.info("Loading ledger from %s...", tmpfile.name)
-            ledger = beancount.loader.load_file(tmpfile.name)
-    else:
-        logging.info("Loading ledger from %s...", filename)
-        ledger = beancount.loader.load_file(filename)
-
-    if ledger[1]:  # Beancount encountered loading error(s), fail with diagnostic
+    (pattern, filenames) = (None, [])
+    if len(args) == 1:  # len(args) == 0 should not happen due to required=True
+        filenames = list(args)
+    elif len(args) >= 2:
+        (pattern, filenames) = (args[0], list(args[1:]))
+    if len(list(filter(lambda fname: fname == "-", filenames))) > 1:
         raise click.BadArgumentUsage(
-            f'\nBeancount encountered error(s) when loading "{filename}":\n'
-            + "\n".join(str(err) for err in ledger[1]),
+            'Standard input ("-") cannot be specified multipled times'
         )
 
     try:
         criteria = Criteria()  # start from default criteria
         if pattern is not None:  # override with smart pattern, if given as argument
             criteria = Criteria.guess(pattern, ignore_case, base=criteria)
         criteria = Criteria.build(  # override with explicit options, if any
@@ -928,28 +912,48 @@
             type_pat=type_pat,
             ignore_case=ignore_case,
             base=criteria,
         )
     except ValueError as e:
         raise click.UsageError(e.args[0]) from e
     logging.info("Using search criteria: %s", criteria)
-    logging.debug("Input ledger contains %d entries", len(ledger[0]))
 
     match_found = False
-    for entry in filter_entries(
-        ledger[0],
-        criteria,
-        posting_tags_meta=posting_tags_meta,
-        skip_internals=skip_internals,
-    ):
-        match_found = True
-        if quiet:
-            break
+    for filename in filenames:
+        if filename == "-":
+            # Beancount does not support streaming reading, so to mimic Unix filter
+            # semantics we read stdin to the end and store it to a temporary file.
+            with NamedTemporaryFile(prefix="beangrep.", suffix=".beancount") as tmpfile:
+                logging.info("Buffering stdin to temporary file %s...", tmpfile.name)
+                shutil.copyfileobj(sys.stdin.buffer, tmpfile.file)
+                tmpfile.flush()
+                logging.info("Loading ledger from %s...", tmpfile.name)
+                ledger = beancount.loader.load_file(tmpfile.name)
         else:
-            printer.print_entry(entry)
+            logging.info("Loading ledger from %s...", filename)
+            ledger = beancount.loader.load_file(filename)
+
+        if ledger[1]:  # Beancount encountered loading error(s), fail with diagnostic
+            raise click.BadArgumentUsage(
+                f'\nBeancount encountered error(s) when loading "{filename}":\n'
+                + "\n".join(str(err) for err in ledger[1]),
+            )
+        logging.debug("Input ledger contains %d entries", len(ledger[0]))
+
+        for entry in filter_entries(
+            ledger[0],
+            criteria,
+            posting_tags_meta=posting_tags_meta,
+            skip_internals=skip_internals,
+        ):
+            match_found = True
+            if quiet:
+                break
+            else:
+                printer.print_entry(entry)
 
     exit_status = 0 if match_found else 1
     ctx.exit(exit_status)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `beangrep-0.3.0/src/beangrep.egg-info/PKG-INFO` & `beangrep-0.4.0/src/beangrep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beangrep
-Version: 0.3.0
+Version: 0.4.0
 Summary: Grep-like filter for the Beancount plain text accounting system
 Author-email: Stefano Zacchiroli <zack@upsilon.cc>
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/zacchiro/beangrep
 Project-URL: Issues, https://github.com/zacchiro/beangrep/issues
 Keywords: accounting,beancount,grep,ledger,plaintext,plaintext-accounting
 Classifier: Programming Language :: Python :: 3
@@ -75,22 +75,23 @@
 
 Usage
 -----
 
 The CLI says it all when invoked as `bean-grep --help`:
 
 ```
-Usage: bean-grep [OPTIONS] [PATTERN] FILENAME
+Usage: bean-grep [OPTIONS] [PATTERN] FILENAME...
 
-  Search for entries matching given criteria in a Beancount ledger. Pretty
+  Search for entries matching given criteria in Beancount journals. Pretty
   print matching entries to standard output.
 
   Search criteria can be specified with the options below and/or providing an
   explicit ("smart") PATTERN. If given, PATTERN is interpreted either as a
   date (if it is in the "YYYY-MM-DD" format), tag ("#tag"), link ("^link"),
+  account (start with an account type, e.g., "Assets", "Income", etc.),
   metadata pair ("key:value"), or string to be matched anywhere (see
   -s/--somewhere below), in this order. If PATTERN is not given, search
   criteria are defined by explicit options.
 
   Multiple options and/or PATTERN are logically joined (AND-ed) together. In
   case of overlap, explicit options override PATTERN.
 
@@ -151,28 +152,29 @@
                                   types. [default: transaction]
   -i, --ignore-case / --no-ignore-case
                                   Ignore case distinctions in string matches.
                                   [default: no-ignore-case]
   --posting-tags-meta TEXT        Metadata key used to attach tags to
                                   transaction postings.  [default: tags]
   -q, --quiet / --no-quiet        Quiet, do not write anything to standard
-                                  output. Exit succesfully immediately if any
+                                  output. Exit successfully immediately if any
                                   match is found.  [default: no-quiet]
   --skip-internals / --no-skip-internals
                                   When matching, ignore internal information
                                   not visible in the ledger. This includes the
                                   automatic metadata: ['filename', 'lineno']
                                   [default: skip-internals]
-  -v, --verbose                   Increase logging verbosity. Default level is
-                                  WARNING. Passing this option once (e.g., -v)
-                                  will increase it to INFO, twice or more
-                                  (e.g., -vv) to DEBUG.
+  --verbose                       Increase logging verbosity. Default
+                                  verbosity is at WARNING level; passing this
+                                  option once will increase it to INFO, twice
+                                  or more to DEBUG.
+  -V, --version                   Show the version and exit.
   --help                          Show this message and exit.
 
-  Exit status is 0 (sucess) if a match is found, 1 if no match is found, 2 if
+  Exit status is 0 (success) if a match is found, 1 if no match is found, 2 if
   an error occurred.
 ```
 
 
 Author
 ------
```

### Comparing `beangrep-0.3.0/tests/data/example.beancount` & `beangrep-0.4.0/tests/data/example.beancount`

 * *Files identical despite different names*

### Comparing `beangrep-0.3.0/tests/test_beangrep.py` & `beangrep-0.4.0/tests/test_beangrep.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,54 +22,19 @@
     DatePredicate,
     RelOp,
     cli,
     filter_entries,
     parse_types,
 )
 
-SAMPLE_LEDGER = str(
-    Path(beangrep.__file__).parents[2] / "tests" / "data" / "example.beancount"
-)
+DATA_DIR = Path(beangrep.__file__).parents[2] / "tests" / "data"
+SAMPLE_LEDGER = str(DATA_DIR / "example.beancount")
+SAMPLE_LEDGER_SMALL = str(DATA_DIR / "small.beancount")
 DIRECTIVES_IN_SAMPLE = 2247  # `bean-quey example.beancount` shows this
 
-_META = data.new_metadata("beangrep/test_beangrep.py", 1234)
-_FLAG = "*"
-_DATE = date(2024, 5, 10)
-
-
-# def mk_empty_txn(date=_DATE, flag=_FLAG, meta=_META) -> data.Transaction:
-#     """Test helper to create an empty transaction."""
-#     return data.Transaction(
-#         meta,
-#         date,
-#         flag,
-#         None,
-#         "something happened",
-#         data.EMPTY_SET,
-#         data.EMPTY_SET,
-#         [],
-#     )
-
-
-# def mk_txn(
-#     postings: Iterable[tuple[str, Union[str, Decimal], str]],
-#     date=_DATE,
-#     flag=_FLAG,
-#     meta=_META,
-# ) -> data.Transaction:
-#     """Test helper to create a transaction with postings.
-#
-#     Postings are specified as (account, number, currency) triples.
-#
-#     """
-#     txn = mk_empty_txn(date=date, flag=flag, meta=meta)
-#     for account, number, currency in postings:
-#         data.create_simple_posting(txn, account, number, currency)
-#     return txn
-
 
 def test_relop():
     """Test evaluation of relational operators."""
     assert RelOp.EQ.eval(42, 42)
     assert RelOp.LT.eval(41, 42)
     assert RelOp.GT.eval(43, 42)
     assert RelOp.LEQ.eval(41, 42)
@@ -301,14 +266,17 @@
 
 def test_somewhere_filtering():
     l = load_sample_ledger()  # noqa:E741
     assert (
         grep_len(l, mk_criteria(somewhere=re.compile("^Transfering"))) == 9
     )  # txn narration
     assert grep_len(l, mk_criteria(somewhere=re.compile("^Cafe"))) == 59  # txn payee
+    assert (
+        grep_len(l, mk_criteria(somewhere=re.compile("US:Federal"))) == 94
+    )  # txn account
     assert grep_len(l, mk_criteria(somewhere=re.compile("trip-san"))) == 21  # txn tag
     assert grep_len(l, mk_criteria(somewhere=re.compile("^a-day-in"))) == 6  # txn link
     assert grep_len(l, mk_criteria(somewhere=re.compile("2015-05-01"))) == 6  # txn date
     assert (
         grep_len(l, mk_criteria(somewhere=re.compile("3219.17 USD"))) == 2
     )  # txn amount
     assert (
@@ -358,21 +326,45 @@
 def test_cli_basic():
     """Test basic CLI invocation."""
     runner = CliRunner()
     result = runner.invoke(cli, ["--help"])
     assert result.exit_code == 0
     assert result.output.startswith("Usage:")
 
+    result = runner.invoke(cli, ["-V"])
+    assert result.exit_code == 0
+    assert " version " in result.output
+    result = runner.invoke(cli, ["--version"])
+    assert result.exit_code == 0
+    assert " version " in result.output
+
     result = runner.invoke(cli, ["--foobarbazqux", SAMPLE_LEDGER])  # no such option
     assert result.exit_code == 2
 
     result = runner.invoke(cli, ["--date /2024", SAMPLE_LEDGER])  # invalid predicate
     assert result.exit_code == 2
 
     assert runner.invoke(cli, []).exit_code == 2
+    assert runner.invoke(cli, ["pattern", "-", "-"]).exit_code == 2  # stdin twice
+
+
+def test_cli_multiple_files():
+    runner = CliRunner()
+    result = runner.invoke(cli, ["Opening", SAMPLE_LEDGER, SAMPLE_LEDGER_SMALL])
+    assert result.exit_code == 0
+    assert "Assets:US:BofA:Checking" in result.output  # hit in SAMPLE_LEDGER
+    assert "Assets:Checking" in result.output  # hit in SAMPLE_LEDGER_SMALL
+
+    result = runner.invoke(cli, ["no such text", SAMPLE_LEDGER, SAMPLE_LEDGER_SMALL])
+    assert result.exit_code == 1
+
+    result = runner.invoke(cli, ["Opening Balance", SAMPLE_LEDGER, SAMPLE_LEDGER_SMALL])
+    assert result.exit_code == 0  # hit in SAMPLE_LEDGER
+    result = runner.invoke(cli, ["Opening balance", SAMPLE_LEDGER, SAMPLE_LEDGER_SMALL])
+    assert result.exit_code == 0  # hit in SAMPLE_LEDGER_SMALL
 
 
 def test_cli_exit_code():
     """Test CLI exit code."""
     runner = CliRunner()
     result = runner.invoke(
         cli, ["--account", "Expenses:Food:Restaurant", SAMPLE_LEDGER]
@@ -432,14 +424,23 @@
     assert result.exit_code == 1
 
     result = runner.invoke(cli, ["--type", "balance,query", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "taxes" in result.output
     assert "PreTax401k" in result.output
 
+    result = runner.invoke(
+        cli, ["--type", "pad,document,note,custom", SAMPLE_LEDGER_SMALL]
+    )
+    assert result.exit_code == 0
+    assert "Rounding-Error" in result.output  # pad hit
+    assert "statements.txt" in result.output  # document hit
+    assert "YAY" in result.output  # note hit
+    assert "TRUE" in result.output  # custom hit
+
 
 def test_cli_smart_pattern():
     runner = CliRunner()
     result = runner.invoke(cli, ["2014-03-28", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "Buying groceries" in result.output
 
@@ -447,14 +448,18 @@
     assert result.exit_code == 0
     assert "Eataly Chicago" in result.output
 
     result = runner.invoke(cli, ["^a-day-in", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "Mercadito" in result.output
 
+    result = runner.invoke(cli, ["Expenses:Vacation", SAMPLE_LEDGER])
+    assert result.exit_code == 0
+    assert "vacation days" in result.output
+
     result = runner.invoke(cli, ["--type", "commodity", "export:CASH", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "US Dollar" in result.output
 
     result = runner.invoke(cli, ["Buying groceries", SAMPLE_LEDGER])
     assert result.exit_code == 0
     assert "Onion Market" in result.output
@@ -490,10 +495,13 @@
         ledger_text = f.read()
         assert (
             runner.invoke(cli, ["-p", "Uncle Boons", "-"], input=ledger_text).exit_code
             == 0
         )
 
 
-def test_cli_file_error():
+def test_cli_errors():
     runner = CliRunner()
-    assert runner.invoke(cli, ["does_not_exist_asklahkj15.beancount"]).exit_code == 2
+    assert runner.invoke(cli, ["does_not_exist.beancount"]).exit_code == 2
+    assert (
+        runner.invoke(cli, ["--amount", "%23 USD", SAMPLE_LEDGER]).exit_code == 2
+    )  # invalid amount predicate
```


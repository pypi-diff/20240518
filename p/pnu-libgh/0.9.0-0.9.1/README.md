# Comparing `tmp/pnu_libgh-0.9.0.tar.gz` & `tmp/pnu_libgh-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnu_libgh-0.9.0.tar", last modified: Tue May  7 21:58:16 2024, max compression
+gzip compressed data, was "pnu_libgh-0.9.1.tar", last modified: Sat May 18 17:20:17 2024, max compression
```

## Comparing `pnu_libgh-0.9.0.tar` & `pnu_libgh-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-07 21:58:16.506797 pnu_libgh-0.9.0/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-07 21:58:16.506764 pnu_libgh-0.9.0/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1509 2024-05-07 09:17:07.000000 pnu_libgh-0.9.0/README.md
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-07 21:58:16.503829 pnu_libgh-0.9.0/man/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1935 2024-05-07 21:58:14.000000 pnu_libgh-0.9.0/man/libgh.1.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2199 2024-05-07 21:58:14.000000 pnu_libgh-0.9.0/man/libgh.3.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-31 15:28:19.000000 pnu_libgh-0.9.0/pyproject.toml
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1313 2024-05-07 21:58:16.507509 pnu_libgh-0.9.0/setup.cfg
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-07 21:58:16.502872 pnu_libgh-0.9.0/src/
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-07 21:58:16.505264 pnu_libgh-0.9.0/src/libgh/
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-31 15:28:19.000000 pnu_libgh-0.9.0/src/libgh/__init__.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2296 2024-05-07 08:00:02.000000 pnu_libgh-0.9.0/src/libgh/accounts.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      510 2024-05-06 09:38:42.000000 pnu_libgh-0.9.0/src/libgh/common.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    14507 2024-05-07 09:09:37.000000 pnu_libgh-0.9.0/src/libgh/libpnu2.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7097 2024-05-07 21:27:36.000000 pnu_libgh-0.9.0/src/libgh/main.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     9912 2024-05-07 08:06:49.000000 pnu_libgh-0.9.0/src/libgh/organization_account.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    12984 2024-05-07 08:37:51.000000 pnu_libgh-0.9.0/src/libgh/personal_account.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7827 2024-05-07 08:00:23.000000 pnu_libgh-0.9.0/src/libgh/repositories.py
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-07 21:58:16.506496 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-07 21:58:16.000000 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)      481 2024-05-07 21:58:16.000000 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/SOURCES.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-05-07 21:58:16.000000 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/dependency_links.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       54 2024-05-07 21:58:16.000000 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/entry_points.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       15 2024-05-07 21:58:16.000000 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/requires.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        6 2024-05-07 21:58:16.000000 pnu_libgh-0.9.0/src/pnu_libgh.egg-info/top_level.txt
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.510657 pnu_libgh-0.9.1/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-18 17:20:17.510624 pnu_libgh-0.9.1/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1509 2024-05-18 07:23:12.000000 pnu_libgh-0.9.1/README.md
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.507677 pnu_libgh-0.9.1/man/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1919 2024-05-18 17:20:15.000000 pnu_libgh-0.9.1/man/libgh.1.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     2199 2024-05-18 17:20:15.000000 pnu_libgh-0.9.1/man/libgh.3.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-31 15:28:19.000000 pnu_libgh-0.9.1/pyproject.toml
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1313 2024-05-18 17:20:17.511367 pnu_libgh-0.9.1/setup.cfg
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.506778 pnu_libgh-0.9.1/src/
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.509077 pnu_libgh-0.9.1/src/libgh/
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-31 15:28:19.000000 pnu_libgh-0.9.1/src/libgh/__init__.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2296 2024-05-18 12:44:12.000000 pnu_libgh-0.9.1/src/libgh/accounts.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      510 2024-05-06 09:38:42.000000 pnu_libgh-0.9.1/src/libgh/common.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    14845 2024-05-18 15:25:02.000000 pnu_libgh-0.9.1/src/libgh/libpnu2.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     6855 2024-05-18 17:19:57.000000 pnu_libgh-0.9.1/src/libgh/main.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     9912 2024-05-18 15:35:18.000000 pnu_libgh-0.9.1/src/libgh/organization_account.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    13542 2024-05-18 15:50:32.000000 pnu_libgh-0.9.1/src/libgh/personal_account.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7924 2024-05-18 15:14:50.000000 pnu_libgh-0.9.1/src/libgh/repositories.py
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-05-18 17:20:17.510361 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     2619 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      481 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/SOURCES.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/dependency_links.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       54 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/entry_points.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       15 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/requires.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        6 2024-05-18 17:20:17.000000 pnu_libgh-0.9.1/src/pnu_libgh.egg-info/top_level.txt
```

### Comparing `pnu_libgh-0.9.0/PKG-INFO` & `pnu_libgh-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-libgh
-Version: 0.9.0
+Version: 0.9.1
 Summary: GitHub scraping library and tool
 Home-page: https://github.com/HubTou/libgh/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/libgh/issues
 Keywords: pnu-project
@@ -23,16 +23,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: pnu-libpnu
 
-[![Servier Inspired](https://raw.githubusercontent.com/servierhub/.github/main/badges/inspired.svg)](https://github.com/ServierHub/)
 [![PyPI package](https://repology.org/badge/version-for-repo/pypi/python:pnu-libgh.svg)](https://repology.org/project/python:pnu-libgh/versions)
+[![Servier Inspired](https://raw.githubusercontent.com/servierhub/.github/main/badges/inspired.svg)](https://github.com/ServierHub/)
 
 # libGH(1), libGH(3) - GitHub scraping tool and library
 
 This repository includes a command-line utility:
 * [libgh(1)](https://github.com/HubTou/libgh/blob/main/LIBGH.1.md) - GitHub scraping tool
   (returning data as [text](https://www.frbsd.org/xch/libgh.txt),
   [JSON](https://www.frbsd.org/xch/libgh.json)
```

### Comparing `pnu_libgh-0.9.0/README.md` & `pnu_libgh-0.9.1/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![Servier Inspired](https://raw.githubusercontent.com/servierhub/.github/main/badges/inspired.svg)](https://github.com/ServierHub/)
 [![PyPI package](https://repology.org/badge/version-for-repo/pypi/python:pnu-libgh.svg)](https://repology.org/project/python:pnu-libgh/versions)
+[![Servier Inspired](https://raw.githubusercontent.com/servierhub/.github/main/badges/inspired.svg)](https://github.com/ServierHub/)
 
 # libGH(1), libGH(3) - GitHub scraping tool and library
 
 This repository includes a command-line utility:
 * [libgh(1)](https://github.com/HubTou/libgh/blob/main/LIBGH.1.md) - GitHub scraping tool
   (returning data as [text](https://www.frbsd.org/xch/libgh.txt),
   [JSON](https://www.frbsd.org/xch/libgh.json)
```

### Comparing `pnu_libgh-0.9.0/man/libgh.3.gz` & `pnu_libgh-0.9.1/man/libgh.3.gz`

 * *Files identical despite different names*

### Comparing `pnu_libgh-0.9.0/setup.cfg` & `pnu_libgh-0.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pnu-libgh
 description = GitHub scraping library and tool
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.9.0
+version = 0.9.1
 license = BSD 3-Clause License
 license_files = LICENSe
 author = Hubert Tournier
 author_email = hubert.tournier@gmail.com
 url = https://github.com/HubTou/libgh/
 project_urls = 
 	Bug Tracker = https://github.com/HubTou/libgh/issues
```

### Comparing `pnu_libgh-0.9.0/src/libgh/accounts.py` & `pnu_libgh-0.9.1/src/libgh/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,19 @@
             cache_days=cache_days,
             cache_index=True,
             force_fetch=force_fetch,
             min_delay=REQUESTS_MIN_DELAY,
             max_per_hour=REQUESTS_PER_HOUR
         )
     except (LookupError, PermissionError) as error:
-        logging.error("libGH: %s", error)
+        logging.error("libgh: %s", error)
         return account
     for item in response:
         if item[0].startswith("x-ratelimit"):
-            logging.debug("libGH: HTTP response: %s=%s", item[0], item[1])
+            logging.debug("libgh: HTTP response: %s=%s", item[0], item[1])
 
     soup = BeautifulSoup(data, "html.parser")
 
     organization = soup.find("meta", attrs={"name":"hovercard-subject-tag"})
     if organization is None:
         account = load_user_account(
             account_name,
```

### Comparing `pnu_libgh-0.9.0/src/libgh/libpnu2.py` & `pnu_libgh-0.9.1/src/libgh/libpnu2.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     last_hour = 0
     last_minute = 0
 
     one_day = 24 * 60 * 60 # seconds
     one_hour = 60 * 60 # seconds
     one_minute = 60 # seconds
 
-    # The requests_times is not necessarily ordered by ascending timestamps
+    # The requests_times is not necessarily ordered by ascending timestamps...
     for request_time in requests_times:
         time_diff = current_time - request_time
         if time_diff <= one_day:
             last_day += 1
         if time_diff <= one_hour:
             last_hour += 1
         if time_diff <= one_minute:
@@ -137,21 +137,32 @@
         logging.debug(
             "libpnu/get_url_bdata: Web requests to '%s' last day=%d, hour=%d, min=%d",
             website,
             last_day,
             last_hour,
             last_minute
         )
+        slowing_down = False
         if last_day >= max_per_day > 0:
-            raise PermissionError(f"Max requests per day reached for '{website}'")
+            logging.debug("libpnu/get_url_bdata: Max requests per day reached. Sleeping for 1 day")
+            time.sleep(24 * 60 * 60)
+            slowing_down = True
         if last_hour >= max_per_hour > 0:
-            raise PermissionError(f"Max requests per hour reached for '{website}'")
+            logging.debug(
+                "libpnu/get_url_bdata: Max requests per hour reached. Sleeping for 1 hour"
+            )
+            time.sleep(60 * 60)
+            slowing_down = True
         if last_minute >= max_per_minute > 0:
-            logging.debug("libpnu/get_url_bdata: Slowing down URL fetching. Sleeping for 1 minute")
+            logging.debug(
+                "libpnu/get_url_bdata: Max requests per minute reached. Sleeping for 1 minute"
+            )
             time.sleep(60)
+            slowing_down = True
+        if slowing_down:
             current_time = time.time()
             current_date = datetime.datetime.fromtimestamp(current_time)
 
         if min_delay:
             time_diff = current_time - get_url_bdata.history[website][-1]
             if time_diff < min_delay:
                 time_wait = min_delay - time_diff
@@ -241,14 +252,15 @@
     directory = libpnu.get_caching_directory(cache_dir)
     if not directory:
         # Don't take the risk to remove files
         return
 
     # Load the index file if it exist
     index_name = f"{directory}{os.sep}index.txt"
+    lines = []
     if os.path.isfile(index_name):
         with open(index_name, encoding="utf-8", errors="ignore") as file:
             lines = file.read().splitlines()
 
     # Remove duplicates
     index = {}
     for line in lines:
```

### Comparing `pnu_libgh-0.9.0/src/libgh/main.py` & `pnu_libgh-0.9.1/src/libgh/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,43 +15,41 @@
 
 from .common import CACHE_DIR, CACHE_DAYS
 from .accounts import load_account, load_accounts
 from .repositories import load_repository, load_repositories
 from .libpnu2 import get_url_bdata, get_url_data, prune_cache, collection2xml
 
 # Version string used by the what(1) and ident(1) commands:
-ID = "@(#) $Id: libgh - GitHub scraping tool v0.9.0 (May 7, 2024) by Hubert Tournier $"
+ID = "@(#) $Id: libgh - GitHub scraping tool v0.9.1 (May 18, 2024) by Hubert Tournier $"
 
 # Default parameters. Can be overcome by environment variables, then command line options
 parameters = {
-    "Process repositories": False,
     "Prune cache": False,
     "Force fetching URL": False,
     "Cache days": CACHE_DAYS,
     "Complete partial": [],
     "JSON output": False,
     "XML output": False,
 }
 
 
 ####################################################################################################
 def _display_help():
     """ Display usage and help """
     #pylint: disable=C0301
     print("usage: libgh [--debug] [--help|-?] [--version]", file=sys.stderr)
-    print("       [--from] [--json|-j] [--repo|-r] [--topics] [--xml|-x]", file=sys.stderr)
+    print("       [--from] [--json|-j] [--topics] [--xml|-x]", file=sys.stderr)
     print("       [--days|-d DAYS] [--force|-f] [--prune|-p]", file=sys.stderr)
     print("       [--] account_or_repo [...]", file=sys.stderr)
     print("  ------------------  --------------------------------------------------", file=sys.stderr)
     print("  --days|-d DAYS      Set number of caching days (0=don't use cache)", file=sys.stderr)
     print("  --force|-f          Force fetching URL instead of using cache", file=sys.stderr)
     print("  --from              Load repositories when forked_from is blank", file=sys.stderr)
     print("  --json|-j           Switch to JSON output instead of plain text", file=sys.stderr)
     print("  --prune|-p          Prune cache items olday than DAYS and cache index", file=sys.stderr)
-    print("  --repo|-r           Process repositories instead of accounts", file=sys.stderr)
     print("  --topics            Load repositories when there are missing topics", file=sys.stderr)
     print("  --xml|-x            Switch to XML output instead of plain text", file=sys.stderr)
     print("  --debug             Enable debug mode", file=sys.stderr)
     print("  --help|-?           Print usage and this help message and exit", file=sys.stderr)
     print("  --version           Print version and exit", file=sys.stderr)
     print("  --                  Options processing terminator", file=sys.stderr)
     print(file=sys.stderr)
@@ -63,24 +61,23 @@
     """ Process command line options """
     #pylint: disable=C0103, W0602
     global parameters
     #pylint: enable=C0103, W0602
 
     # option letters followed by : expect an argument
     # same for option strings followed by =
-    character_options = "d:fjprx?"
+    character_options = "d:fjpx?"
     string_options = [
         "days=",
         "debug",
         "force",
         "from",
         "help",
         "json",
         "prune",
-        "repo",
         "topics",
         "version",
         "xml",
     ]
 
     try:
         options, remaining_arguments = getopt.getopt(
@@ -122,19 +119,14 @@
 
         elif option in ("--json", "-j"):
             parameters["JSON output"] = True
             parameters["XML output"] = False
 
         elif option in ("--prune", "-p"):
             parameters["Prune cache"] = True
-            parameters["Process repositories"] = False
-
-        elif option in ("--repo", "-r"):
-            parameters["Process repositories"] = True
-            parameters["Prune cache"] = False
 
         elif option == "--topics":
             parameters["Complete partial"].append("topics")
 
         elif option in ("--xml", "-x"):
             parameters["XML output"] = True
             parameters["JSON output"] = False
@@ -150,51 +142,57 @@
     libpnu.initialize_debugging(program_name)
     libpnu.handle_interrupt_signals(libpnu.interrupt_handler_function)
     arguments = _process_command_line()
 
     if parameters["Prune cache"]:
         prune_cache(CACHE_DIR, parameters["Cache days"])
 
-    elif parameters["Process repositories"]:
-        if not arguments:
-            _display_help()
-        else:
-            repositories = load_repositories(
-                arguments,
-                parameters["Cache days"],
-                force_fetch=parameters["Force fetching URL"],
-            )
-            if parameters["JSON output"]:
-                json.dump(repositories, sys.stdout)
-                print()
-            elif parameters["XML output"]:
-                xml = collection2xml(repositories, name="repositories")
-                for line in xml:
-                    print(line)
-            else:
-                pprint.pprint(repositories, sort_dicts=False)
+    if not arguments:
+        _display_help()
 
     else:
-        if not arguments:
-            _display_help()
-        else:
-            accounts = load_accounts(
-                arguments,
+        accounts = []
+        repositories = []
+        for argument in arguments:
+            if '/' in argument:
+                repositories.append(argument)
+            else:
+                accounts.append(argument)
+
+        data = {}
+        if accounts:
+            data = load_accounts(
+                accounts,
                 parameters["Cache days"],
                 force_fetch=parameters["Force fetching URL"],
                 complete=parameters["Complete partial"],
             )
-            if parameters["JSON output"]:
-                json.dump(accounts, sys.stdout)
-                print()
-            elif parameters["XML output"]:
-                xml = collection2xml(accounts, name="accounts")
-                for line in xml:
-                    print(line)
-            else:
-                pprint.pprint(accounts, sort_dicts=False)
+        if repositories:
+            data2 = load_repositories(
+                repositories,
+                parameters["Cache days"],
+                force_fetch=parameters["Force fetching URL"],
+            )
+
+            # Performing nested dictionary update
+            for account, account_value in data2.items():
+                if account in data:
+                    for repository, repository_value in account_value["repositories"].items():
+                        data[account]["repositories"][repository] = repository_value
+                else:
+                    data[account] = account_value
+
+        if parameters["JSON output"]:
+            json.dump(data, sys.stdout)
+            print()
+        elif parameters["XML output"]:
+            xml = collection2xml(data, name="GitHub")
+            for line in xml:
+                print(line)
+        else:
+            pprint.pprint(data, sort_dicts=False)
 
     sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pnu_libgh-0.9.0/src/libgh/organization_account.py` & `pnu_libgh-0.9.1/src/libgh/organization_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
                 cache_days=cache_days,
                 cache_index=True,
                 force_fetch=force_fetch,
                 min_delay=REQUESTS_MIN_DELAY,
                 max_per_hour=REQUESTS_PER_HOUR
             )
         except (LookupError, PermissionError) as error:
-            logging.error("libGH: %s", error)
+            logging.error("libgh: %s", error)
             return repos
         for item in response:
             if item[0].startswith("x-ratelimit"):
-                logging.debug("libGH: HTTP response: %s=%s", item[0], item[1])
+                logging.debug("libgh: HTTP response: %s=%s", item[0], item[1])
 
         soup = BeautifulSoup(data, "html.parser")
 
         # repositories list
         json_data = soup.find(
             "script",
             attrs={"type":"application/json", "data-target":"react-app.embeddedData"}
@@ -57,18 +57,14 @@
             j = json.loads(data)
 
         for repository in j["payload"]["repositories"]:
             name = repository["name"]
             repos[name] = {}
             uncomplete = False
 
-            # archived?
-            if repos_type == "archived":
-                repos[name]["archived"] = True
-
             # forked from
             if repository["isFork"]:
                 repos[name]["forked_from"] = "" # The original location is not provided
                 if "forked_from" in complete:
                     uncomplete = True
 
             # topics
@@ -107,14 +103,18 @@
                 # license
                 if repository["license"] is not None:
                     repos[name]["license"] = repository["license"]
 
             # last updated
             repos[name]["last_updated"] = repository["lastUpdated"]["timestamp"]
 
+            # archived?
+            if repos_type == "archived":
+                repos[name]["archived"] = True
+
         # is there a next page?
         next_page = soup.select_one('[aria-label="Next Page"]')
         if next_page is not None:
             try:
                 next_page.get("href")
             except AttributeError:
                 break
@@ -275,13 +275,13 @@
         most_used_topics.items(),
         key=lambda item: item[1],
         reverse=True
     ))
 
     if len(account["repositories"]) != account["repositories_count"]:
         logging.warning(
-            "libGH: Loaded %d/%d repositories",
+            "libgh: Loaded %d/%d repositories",
             len(account["repositories"]),
             account["repositories_count"]
         )
 
     return account
```

### Comparing `pnu_libgh-0.9.0/src/libgh/personal_account.py` & `pnu_libgh-0.9.1/src/libgh/personal_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 import re
 
 from bs4 import BeautifulSoup
 
 from .common import GITHUB_URL, CACHE_DIR, REQUESTS_MIN_DELAY, REQUESTS_PER_HOUR
 from .libpnu2 import get_url_data
+from .repositories import load_repository
 
 ####################################################################################################
 def load_user_repositories(user_name, url, page, cache_days, force_fetch=False, complete=[]):
     """ Returns a dictionary of user's repositories """
     repos = {}
 
     try:
@@ -24,81 +25,87 @@
             cache_days=cache_days,
             cache_index=True,
             force_fetch=force_fetch,
             min_delay=REQUESTS_MIN_DELAY,
             max_per_hour=REQUESTS_PER_HOUR
         )
     except (LookupError, PermissionError) as error:
-        logging.error("libGH: %s", error)
+        logging.error("libgh: %s", error)
         return repos
     for item in response:
         if item[0].startswith("x-ratelimit"):
-            logging.debug("libGH: HTTP response: %s=%s", item[0], item[1])
+            logging.debug("libgh: HTTP response: %s=%s", item[0], item[1])
 
     soup = BeautifulSoup(data, "html.parser")
 
     # repositories list
     repos_list = soup.select_one('[id="user-repositories-list"]')
     items = repos_list.select("li")
     for item in items:
         # name
         html = item.select_one('[itemprop="name codeRepository"]')
         name = html.text.strip()
         repos[name] = {}
 
-        # archived?
-        li_class = item.get("class")
-        if "archived" in li_class:
-            repos[name]["archived"] = True
-
-        # forked from
-        html = item.select_one('[class="Link--muted Link--inTextBlock"]')
-        if html is not None:
-            repos[name]["forked_from"] = html.text.strip()
-
-        # description
-        html = item.select_one('[itemprop="description"]')
-        if html is not None:
-            repos[name]["description"] = html.text.strip()
-
         # topics
         repos[name]["topics"] = []
         html = item.select('[data-octo-click="topic_click"]')
         if html is not None:
             for html2 in html:
                 repos[name]["topics"].append(html2.text.strip())
 
-        # programming language
-        html = item.select_one('[itemprop="programmingLanguage"]')
-        if html is not None:
-            repos[name]["programming_language"] = html.text.strip()
+        # when there are 7 topics, it's probable than GitHub is only showing the first ones
+        # (can also happen with less when the topics character length is large)
+        if "topics" in repos[name] and len(repos[name]["topics"]) == 7 and "topics" in complete:
+            repos[name] = load_repository(user_name, name, cache_days, force_fetch)
 
-        # stargazers
-        repos[name]["stargazers"] = {}
-        html = item.select_one('[class="octicon octicon-star"]')
-        if html is None:
-            repos[name]["stargazers_count"] = 0
         else:
-            html2 = html.next_sibling
-            repos[name]["stargazers_count"] = int(html2.text.strip().replace(',', ''))
+            # archived?
+            li_class = item.get("class")
+            if "archived" in li_class:
+                repos[name]["archived"] = True
+
+            # forked from
+            html = item.select_one('[class="Link--muted Link--inTextBlock"]')
+            if html is not None:
+                repos[name]["forked_from"] = html.text.strip()
+
+            # description
+            html = item.select_one('[itemprop="description"]')
+            if html is not None:
+                repos[name]["description"] = html.text.strip()
+
+            # programming language
+            html = item.select_one('[itemprop="programmingLanguage"]')
+            if html is not None:
+                repos[name]["programming_language"] = html.text.strip()
+
+            # stargazers
+            repos[name]["stargazers"] = {}
+            html = item.select_one('[class="octicon octicon-star"]')
+            if html is None:
+                repos[name]["stargazers_count"] = 0
+            else:
+                html2 = html.next_sibling
+                repos[name]["stargazers_count"] = int(html2.text.strip().replace(',', ''))
 
-        # forks
-        repos[name]["forks"] = {}
-        html = item.select_one('[class="octicon octicon-repo-forked"]')
-        if html is None:
-            repos[name]["forks_count"] = 0
-        else:
-            html2 = html.next_sibling
-            repos[name]["forks_count"] = int(html2.text.strip().replace(',', ''))
+            # forks
+            repos[name]["forks"] = {}
+            html = item.select_one('[class="octicon octicon-repo-forked"]')
+            if html is None:
+                repos[name]["forks_count"] = 0
+            else:
+                html2 = html.next_sibling
+                repos[name]["forks_count"] = int(html2.text.strip().replace(',', ''))
 
-        # license
-        html = item.select_one('[class*="octicon octicon-law"]')
-        if html is not None:
-            html2 = html.next_sibling
-            repos[name]["license"] = html2.text.strip()
+            # license
+            html = item.select_one('[class*="octicon octicon-law"]')
+            if html is not None:
+                html2 = html.next_sibling
+                repos[name]["license"] = html2.text.strip()
 
         # updated
         html = item.select_one('relative-time')
         if html is not None:
             repos[name]["last_updated"] = html.get("datetime")
 
     # is there a next page?
@@ -354,13 +361,13 @@
         most_used_topics.items(),
         key=lambda item: item[1],
         reverse=True
     ))
 
     if len(account["repositories"]) != account["repositories_count"]:
         logging.warning(
-            "libGH: Loaded %d/%d repositories",
+            "libgh: Loaded %d/%d repositories",
             len(account["repositories"]),
             account["repositories_count"]
         )
 
     return account
```

### Comparing `pnu_libgh-0.9.0/src/libgh/repositories.py` & `pnu_libgh-0.9.1/src/libgh/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
             cache_days=cache_days,
             cache_index=True,
             force_fetch=force_fetch,
             min_delay=REQUESTS_MIN_DELAY,
             max_per_hour=REQUESTS_PER_HOUR
         )
     except (LookupError, PermissionError) as error:
-        logging.error("libGH: %s", error)
+        logging.error("libgh: %s", error)
         return repository
     for item in response:
         if item[0].startswith("x-ratelimit"):
-            logging.debug("libGH: HTTP response: %s=%s", item[0], item[1])
+            logging.debug("libgh: HTTP response: %s=%s", item[0], item[1])
 
     soup = BeautifulSoup(data, "html.parser")
 
     #html = soup.select_one('[itemprop="author"]')
     #html = soup.select_one('[itemprop="name"]')
 
     # Forked from (if relevant)
@@ -201,26 +201,30 @@
             repository["commits_count"] = 1
 
     return repository
 
 ####################################################################################################
 def load_repositories(repositories_list, cache_days, force_fetch=False):
     """ Returns a dictionary of repositories information """
-    repositories = {}
+    accounts = {}
 
     for item in repositories_list:
         if item.count('/') == 1:
-            account_name = item.split('/')[0]
-            repository_name = item.split('/')[1]
-            repositories[item] = load_repository(
-                account_name,
-                repository_name,
+            account = item.split('/')[0]
+            repository = item.split('/')[1]
+
+            if account not in accounts:
+                accounts[account] = {"repositories":{}}
+
+            accounts[account]["repositories"][repository] = load_repository(
+                account,
+                repository,
                 cache_days,
                 force_fetch=force_fetch
             )
         else:
             logging.error(
-                "libGH: Repositories parameters must be in 'account/repo' form. '%s' discarded",
+                "libgh: Repositories parameters must be in 'account/repo' form. '%s' discarded",
                 item
             )
 
-    return repositories
+    return accounts
```

### Comparing `pnu_libgh-0.9.0/src/pnu_libgh.egg-info/PKG-INFO` & `pnu_libgh-0.9.1/src/pnu_libgh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-libgh
-Version: 0.9.0
+Version: 0.9.1
 Summary: GitHub scraping library and tool
 Home-page: https://github.com/HubTou/libgh/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/libgh/issues
 Keywords: pnu-project
@@ -23,16 +23,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: bs4
 Requires-Dist: pnu-libpnu
 
-[![Servier Inspired](https://raw.githubusercontent.com/servierhub/.github/main/badges/inspired.svg)](https://github.com/ServierHub/)
 [![PyPI package](https://repology.org/badge/version-for-repo/pypi/python:pnu-libgh.svg)](https://repology.org/project/python:pnu-libgh/versions)
+[![Servier Inspired](https://raw.githubusercontent.com/servierhub/.github/main/badges/inspired.svg)](https://github.com/ServierHub/)
 
 # libGH(1), libGH(3) - GitHub scraping tool and library
 
 This repository includes a command-line utility:
 * [libgh(1)](https://github.com/HubTou/libgh/blob/main/LIBGH.1.md) - GitHub scraping tool
   (returning data as [text](https://www.frbsd.org/xch/libgh.txt),
   [JSON](https://www.frbsd.org/xch/libgh.json)
```


# Comparing `tmp/etm-dgraham-6.2.4.tar.gz` & `tmp/etm-dgraham-6.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.2.4.tar", last modified: Fri May 10 18:50:48 2024, max compression
+gzip compressed data, was "etm-dgraham-6.2.5.tar", last modified: Sat May 18 17:38:14 2024, max compression
```

## Comparing `etm-dgraham-6.2.4.tar` & `etm-dgraham-6.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.099150 etm-dgraham-6.2.4/
--rw-r--r--   0 dag        (501) staff       (20)     5468 2024-05-10 18:50:43.000000 etm-dgraham-6.2.4/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-10 18:50:48.098201 etm-dgraham-6.2.4/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   144578 2024-05-07 12:58:43.000000 etm-dgraham-6.2.4/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.4/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.4/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.091148 etm-dgraham-6.2.4/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.094185 etm-dgraham-6.2.4/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.4/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-10 18:50:43.000000 etm-dgraham-6.2.4/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-05 16:45:06.000000 etm-dgraham-6.2.4/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.4/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.4/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   331023 2024-05-10 18:50:43.000000 etm-dgraham-6.2.4/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.4/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.4/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126267 2024-05-09 23:14:48.000000 etm-dgraham-6.2.4/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.096586 etm-dgraham-6.2.4/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-10 18:50:48.000000 etm-dgraham-6.2.4/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.4/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.4/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/namedcolors.py
--rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.2.4/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.4/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-10 18:50:48.099192 etm-dgraham-6.2.4/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.4/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.096701 etm-dgraham-6.2.4/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.4/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-10 18:50:48.097673 etm-dgraham-6.2.4/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.4/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.4/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.4/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.4/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.946382 etm-dgraham-6.2.5/
+-rw-r--r--   0 dag        (501) staff       (20)     5532 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-18 17:38:14.946169 etm-dgraham-6.2.5/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   144578 2024-05-07 12:58:43.000000 etm-dgraham-6.2.5/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.5/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.5/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.939442 etm-dgraham-6.2.5/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.942321 etm-dgraham-6.2.5/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.5/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-18 16:18:38.000000 etm-dgraham-6.2.5/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.5/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.5/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   330183 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.5/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.5/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126487 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.944588 etm-dgraham-6.2.5/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.5/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.5/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/namedcolors.py
+-rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.2.5/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-18 17:38:14.946418 etm-dgraham-6.2.5/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.5/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.944725 etm-dgraham-6.2.5/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.5/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.945647 etm-dgraham-6.2.5/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.5/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.5/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.5/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.2.4/CHANGES.txt` & `etm-dgraham-6.2.5/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-2024-05-10 8dcf3ad Daniel Graham
+2024-05-18 6376025 Daniel Graham
+    Tagged version 6.2.5.
+
+2024-05-18 b2713d0 Daniel Graham
+    Fixed bug in which pressing 'E' without an item selected, would
+    open the last item
+
+2024-05-18 4b525cd Daniel Graham
+    template tweaks
+
+2024-05-17 0d351be Daniel Graham
+    Fixed bug in allowing invalid duplicate entries
+
+2024-05-10 d71ca52 Daniel Graham
     Tagged version 6.2.4.
 
 2024-05-10 d5e475a Daniel Graham
     Fixed bug in processing alerts for tasks with @s and @+ entries
     but without @r
 
 2024-05-09 3026c51 Daniel Graham
@@ -183,19 +196,7 @@
     only past due after that.
 
 2024-03-19 0f628dc Daniel Graham
     setup_logging __main__ -> common
 
 2024-03-18 2285c8f Daniel Graham
     ETMQuery class view.py -> data.py
-
-2024-03-18 baaaa53 Daniel Graham
-    ETM_CHAR dict -> EtmChar class.
-
-2024-03-17 bc95722 Daniel Graham
-    Recognize vi vs emacs setting.
-
-2024-03-14 bfe10f2 Daniel Graham
-    Tagged version 6.1.22.
-
-2024-03-14 f702181 Daniel Graham
-    Tagged version 6.1.21.
```

### Comparing `etm-dgraham-6.2.4/PKG-INFO` & `etm-dgraham-6.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.4
+Version: 6.2.5
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-6.2.4/README.md` & `etm-dgraham-6.2.5/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/bump.py` & `etm-dgraham-6.2.5/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/docs/index_konnections.md` & `etm-dgraham-6.2.5/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/docs/index_usedtime.md` & `etm-dgraham-6.2.5/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/docs/multiple_timers.md` & `etm-dgraham-6.2.5/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/__main__.py` & `etm-dgraham-6.2.5/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/common.py` & `etm-dgraham-6.2.5/etm/common.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/data.py` & `etm-dgraham-6.2.5/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/make_examples.py` & `etm-dgraham-6.2.5/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/model.py` & `etm-dgraham-6.2.5/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,14 +672,15 @@
         self.object_hsh = {}  # key, val -> object version for tinydb
         self.askreply = {}     # key, val -> display version raw string
         self.pos_hsh = {}     # (beg, end) -> (key, val)
         self.keyvals = []
 
         self.messages = []
         self.active = ()
+        self.allowed = []
         self.interval = ()
         self.item_hsh = {}      # key -> obj
         # Note: datetime(s) require timezone and at requires itemtype
         # all else do not need item_hsh
         self.keys = {
             'itemtype': [
                 'item type',
@@ -1391,15 +1392,15 @@
     def text_changed(self, s, pos, modified=True):
         """ """
         # self.is_modified = modified
         # logger.debug(f"\n### starting text_changed with s: {s} and self.keyvals: {self.keyvals}")
         self.entry = s
         self.pos_hsh, keyvals = process_entry(s, self.settings)
         removed, changed = listdiff(self.keyvals, keyvals)
-        # logger.debug(f" pos_hsh: {self.pos_hsh}; keyvals: {keyvals}\nremoved: {removed}; changed: {changed}")
+        # logger.debug(f"{self.pos_hsh = };\n{keyvals = }\n{removed = };\n{changed = }")
         # if removed + changed != []:
         if self.init_entry != self.entry:
             self.is_modified = True
         # only process changes for kv entries
         update_timezone = False
         for kv in removed + changed:
             if kv[0] == 'z':
@@ -1414,14 +1415,15 @@
             if kv in self.object_hsh:
                 del self.object_hsh[kv]
             if kv in self.askreply:
                 del self.askreply[kv]
             if kv in keyvals:
                 keyvals.remove(kv)
         self.keyvals = []
+        # for kv in [x for x in changed if x not in removed]:
         for kv in [x for x in keyvals if x not in removed]:
             # logger.debug(f"updating kv: {kv}")
             self.update_keyval(kv)
             self.keyvals.append(kv)
         # logger.debug(f"### leaving text_changed with self.keyvals: {self.keyvals}\n")
 
     def update_keyval(self, kv):
@@ -1435,18 +1437,20 @@
 
         # logger.debug(f"checking kv: {kv}")
         if key in self.keys:
             # logger.debug(f"found kv: {kv}")
             a, r, do = self.keys[key]
             ask = a
             msg = self.check_allowed(key)
-            # logger.debug(f"got msg: {msg} when checking {kv} allowed")
+            # logger.debug(f"got {msg = } when checking {kv = } allowed")
             if msg:
                 obj = None
+                ask = 'error'
                 reply = msg
+                self.object_hsh[kv] = None
             else:   # only do this for allowed keys
                 msg = self.check_requires(key)
                 # logger.debug(f"got msg: {msg} checking required for {key}")
                 if msg:
                     # logger.debug(f"failed required, self: {self}")
                     obj = None
                     reply = msg
@@ -1458,15 +1462,17 @@
                     if obj is not None:
                         self.object_hsh[kv] = obj
                         # logger.debug(f"added {kv[0]}: {obj} to obj_hsh: {self.object_hsh}")
                         # self.item_hsh[kv[0]] = obj
                     else:
                         if kv in self.object_hsh:
                             del self.object_hsh[kv]
+            # logger.debug(f"{kv = }; {ask = }; {reply = }")
             self.askreply[kv] = (ask, reply)
+            # logger.debug(f"{self.askreply = }")
         else:
             display_key = f'@{key}' if len(key) == 1 else f'&{key[-1]}'
             self.askreply[kv] = (
                 'unrecognized key',
                 f'{display_key} is invalid',
             )
 
@@ -1476,15 +1482,16 @@
         self.item_hsh = {'created': created}
         cur_hsh = {}
         cur_key = None
         msg = []
         for pos, (k, v) in self.pos_hsh.items():
             obj = self.object_hsh.get((k, v))
             if obj is None:
-                msg.append(f'bad entry for {k}: {v}')
+                # logger.debug(f"{self.askreply.get((k,v), '')}")
+                msg.append(f'bad entry for {k}: {v}\n{self.askreply.get((k,v), ["", ""])[-1]}')
                 return msg
                 # continue
             elif k in ['a', 'u', 'n', 't', 'k', 'K']:
                 self.item_hsh.setdefault(k, []).append(obj)
             elif k in ['rr', 'jj']:
                 if cur_hsh:
                     # starting new rrule or job - append the old
@@ -1614,18 +1621,21 @@
 
 
             numuses = {}
             duplicates = []
             for k, v in self.keyvals:
                 numuses.setdefault(k, 0)
                 numuses[k] += 1
+            # logger.debug(f"{numuses = }")
             duplicates = [
-                k for (k, v) in numuses.items() if v > 1 and k not in [
+                k for (k, v) in numuses.items() if v > 0 and k not in [
                     'a', 'u', 't', 'k', 'K', 'jj', 'rr', 'ji', 'js', 'jb', 'jp', 'ja', 'jd', 'je', 'jf', 'jl', 'jm', 'ju']
                 ]
+            # logger.debug(f"{key = }; {duplicates = }")
+
             if key in duplicates:
                 display_key = f'@{key}' if len(key) == 1 else f'&{key[-1]}'
                 return f'{display_key} has already been entered'
             else:
                 return ''
         else:
             return 'missing itemtype'
@@ -1800,15 +1810,15 @@
         obj = None
         m = quota_regex.match(arg)
         if m:
             obj = [int(x) for x in arg.split(',') if x.strip()]
             weeks = f"for {obj[1]} weeks" if len(obj) > 1 else "indefinitely" 
             rep = f'{obj[0]} times/week {weeks}'
             self.item_hsh['q'] = obj                
-            logger.debug(f"{self.item_hsh = }")
+            # logger.debug(f"{self.item_hsh = }")
         else:
             rep = "goal: instances per week optionally followed by a comma and the number of weeks"
         return obj, rep
         
 
     def do_datetime(self, arg):
         """
@@ -4056,16 +4066,18 @@
         item_id = res[0]
         item = self.db.get(doc_id=item_id)
         if 'doc_id' in item:
             return item['doc_id']
 
     def get_details(self, row=None, edit=False):
         res = self.get_row_details(row)
+        logger.debug(f"{res = }")
         if not (res and res[0]):
             return None, ''
+        
         item_id = res[0]
 
         if not edit and item_id in self.itemcache:
             return item_id, self.itemcache[item_id]
         item = self.db.get(doc_id=item_id)
         if item:
             item_hsh = item_details(item, edit)
@@ -4815,52 +4827,14 @@
         self.refreshCalendar()
 
     def currcal(self):
         self.calAdv = date.today().month // 13
         self.refreshCalendar()
 
 
-# def nowrap(txt, indent=3, width=shutil.get_terminal_size()[0] - 3):
-#     return txt
-
-
-# def wrap(txt, indent=3, width=shutil.get_terminal_size()[0] - 3):
-#     """
-#     Wrap text to terminal width using indent spaces before each line.
-#     >>> txt = "Now is the time for all good men to come to the aid of their country. " * 5
-#     >>> res = wrap(txt, 4, 60)
-#     >>> print(res)
-#     Now is the time for all good men to come to the aid of
-#         their country. Now is the time for all good men to
-#         come to the aid of their country. Now is the time
-#         for all good men to come to the aid of their
-#         country. Now is the time for all good men to come
-#         to the aid of their country. Now is the time for
-#         all good men to come to the aid of their country.
-#     """
-#     para = [x.rstrip() for x in txt.split('\n')]
-#     tmp = []
-#     first = True
-#     for p in para:
-#         if first:
-#             initial_indent = ''
-#             first = False
-#         else:
-#             initial_indent = ' ' * indent
-#         tmp.append(
-#             textwrap.fill(
-#                 p,
-#                 initial_indent=initial_indent,
-#                 subsequent_indent=' ' * indent,
-#                 width=width - indent - 1,
-#             )
-#         )
-#     return '\n'.join(tmp)
-
-
 def set_summary(summary='', start=None, relevant=None, freq=''):
     """ """
     if not (
         '{XXX}' in summary
         and isinstance(start, date)
         and isinstance(relevant, date)
         and freq in ['y', 'm', 'w', 'd']
@@ -5198,18 +5172,17 @@
 @o {{ h['o'] }}{% endif %} \
 {% endif %}\
 {% for k in ['+', '-'] %} \
 {% if k in h and h[k] %}
 @{{ k }} {{ nowrap(dtlst2str(h[k])) }} \
 {%- endif %} \
 {%- endfor %}\
-{% if 'd' in h %}\
-
-@d {{ nowrap(h['d'], 0) }} \
-{% endif -%}
+{%- if 'd' in h %}
+@d {{ h['d'] }} 
+{%- endif -%}
 {%- if 'j' in h %}\
 {%- for x in h['j'] %}\
 {%- set job -%}\
 {{ x['j'] }}\
 {%- for k in ['s', 'e'] -%}
 {%- if k in x and x[k] %} {{ "&{} {}".format(k, in2str(x[k])) }}{% endif %}\
 {%- endfor %}
@@ -5259,15 +5232,15 @@
 {% for x in h['u'] %}{{ "@u {}: {} ".format(in2str(x[0]), dt2str(x[1])[1]) }}{% endfor %}\
 {% endset %}
 {{ wrap(used) }} \
 {% endif %}\
 {%- set is = namespace(found=false) -%}\
 {%- set index -%}\
 {%- for k in ['c', 'i'] -%}\
-{%- if k in h %}@{{ k }} {{ h[k] }}{% set is.found = true %} {% endif %}\
+{%- if k in h %}@{{ k }} {{ h[k] }} {% set is.found = true %}{% endif %}\
 {%- endfor %}\
 {%- endset %}\
 {% if is.found %}
 {{ wrap(index) }} \
 {% endif %}\
 {%- if 't' in h %}\
 {% for x in h['t'] %}{{ "@t {} ".format(x) }}{% endfor %}\
@@ -5310,30 +5283,30 @@
 @o {{ h['o'] }}{% endif %} \
 {% endif %}\
 {% for k in ['+', '-'] %} \
 {% if k in h and h[k] %}
 @{{ k }} {{ wrap(dtlst2str(h[k])) }} \
 {%- endif %} \
 {%- endfor %}\
-{% if 'd' in h %}\
-{% set description -%} \
-@d {{ h['d'] }} \
-{%- endset %}
-{{ wrap(description) }} \
-{% endif -%}\
+{%- if 'd' in h -%}\
+{% set description %}\
+{{ h['d'] }}\
+{% endset %}
+@d {{ wrap(description) }} \
+{%- endif -%}\
 {%- if 'j' in h %}\
 {%- for x in h['j'] %}\
 {%- set job -%}\
 {{ x['j'] }}\
 {%- for k in ['s', 'e'] -%}
 {%- if k in x and x[k] %} {{ "&{} {}".format(k, in2str(x[k])) }}{% endif %}\
 {%- endfor %}
-{%- for k in ['b', 'd', 'l', 'i', 'p'] %}
-{%- if k in x and x[k] %} {{ "&{} {}".format(k, one_or_more(x[k])) }}{% endif %}\
-{%- endfor %}
+{%- for k in ['b', 'd', 'l', 'i', 'p'] %}\
+{%- if k in x and x[k] %} {{ "&{} {}".format(k, one_or_more(x[k])) }}{% endif %}
+{%- endfor %}\
 {%- if 'a' in x %}\
 {%- for a in x['a'] %} {{ "&a {}: {}".format( inlst2str(a[0]), one_or_more(a[1]) ) }}{% endfor %}\
 {%- endif %}\
 {% if 'u' in x %}\
 {%- set used %}\
 {% for u in x['u'] %}{{ "&u {}: {} ".format(in2str(u[0]), dt2str(u[1])[1]) }}{% endfor %}\
 {% endset %}\
```

### Comparing `etm-dgraham-6.2.4/etm/options.py` & `etm-dgraham-6.2.5/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/report.py` & `etm-dgraham-6.2.5/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm/view.py` & `etm-dgraham-6.2.5/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -2628,21 +2628,26 @@
     global item
     global starting_buffer_text
     global text_area
     app = get_app()
     app.editing_mode = (
         EditingMode.VI if settings['vi_mode'] else EditingMode.EMACS
     )
+    doc_id, entry = dataview.get_details(
+        text_area.document.cursor_position_row, True
+    )
+    logger.debug(f"{text_area.document.cursor_position_row = }; {doc_id = }; {entry = }")
+    if not doc_id:
+        logger.debug(f"returning None")
+        return None
+
     if dataview.is_showing_details:
         application.layout.focus(text_area)
         dataview.hide_details()
     dataview.is_editing = True
-    doc_id, entry = dataview.get_details(
-        text_area.document.cursor_position_row, True
-    )
     item.edit_item(doc_id, entry)
     edit_buffer.text = item.entry
     starting_buffer_text = item.entry
     default_buffer_changed(event)
     default_cursor_position_changed(event)
     application.layout.focus(edit_buffer)
 
@@ -3191,14 +3196,15 @@
 """
 
     get_choice(title, text, options)
 
     def coroutine():
         keypress = dataview.details_key_press
         done = keypress in (['escape', '0'] + [x for x in values.keys()])
+        logger.debug(f"{keypress = }; {done = }")
         if done:
             if keypress == '0':
                 ok, msg = import_file('lorem')
                 if ok:
                     dataview.refreshRelevant()
                     dataview.refreshAgenda()
                     if dataview.mk_current:
```

### Comparing `etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.4
+Version: 6.2.5
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-6.2.4/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.2.5/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etmlogo.png` & `etm-dgraham-6.2.5/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etmlogo_small.png` & `etm-dgraham-6.2.5/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/etmview_agenda.png` & `etm-dgraham-6.2.5/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/namedcolors.py` & `etm-dgraham-6.2.5/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/new.png` & `etm-dgraham-6.2.5/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/setup.py` & `etm-dgraham-6.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/test/test_parser.py` & `etm-dgraham-6.2.5/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/utilities/colons_to_slashes.py` & `etm-dgraham-6.2.5/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/utilities/etm_in` & `etm-dgraham-6.2.5/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/utilities/inbasket` & `etm-dgraham-6.2.5/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.4/utilities/open_in_mutt` & `etm-dgraham-6.2.5/utilities/open_in_mutt`

 * *Files identical despite different names*


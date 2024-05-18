# Comparing `tmp/funcy_typing-2.0.0.tar.gz` & `tmp/funcy_typing-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcy_typing-2.0.0.tar", max compression
+gzip compressed data, was "funcy_typing-2.0.1.tar", max compression
```

## Comparing `funcy_typing-2.0.0.tar` & `funcy_typing-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/LICENSE
--rw-r--r--   0        0        0      333 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/README.md
--rw-r--r--   0        0        0     5917 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/__init__.pyi
--rw-r--r--   0        0        0     1041 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/_types.py
--rw-r--r--   0        0        0     1024 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/calc.pyi
--rw-r--r--   0        0        0     9455 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/colls.pyi
--rw-r--r--   0        0        0     3899 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/debug.pyi
--rw-r--r--   0        0        0      351 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/decorators.pyi
--rw-r--r--   0        0        0     3662 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/flow.pyi
--rw-r--r--   0        0        0     1556 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/funcmakers.pyi
--rw-r--r--   0        0        0     6511 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/funcs.pyi
--rw-r--r--   0        0        0      894 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/objects.pyi
--rw-r--r--   0        0        0      650 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/primitives.pyi
--rw-r--r--   0        0        0    25370 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/seqs.pyi
--rw-r--r--   0        0        0     1555 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/strings.pyi
--rw-r--r--   0        0        0      784 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/tree.pyi
--rw-r--r--   0        0        0     1530 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/funcy-stubs/types.pyi
--rw-r--r--   0        0        0     1865 2024-05-10 16:51:41.513655 funcy_typing-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 funcy_typing-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/LICENSE
+-rw-r--r--   0        0        0      344 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/README.md
+-rw-r--r--   0        0        0     6196 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/__init__.pyi
+-rw-r--r--   0        0        0     1041 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/_types.py
+-rw-r--r--   0        0        0     1024 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/calc.pyi
+-rw-r--r--   0        0        0     9455 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/colls.pyi
+-rw-r--r--   0        0        0     3899 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/debug.pyi
+-rw-r--r--   0        0        0      351 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/decorators.pyi
+-rw-r--r--   0        0        0     3662 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/flow.pyi
+-rw-r--r--   0        0        0     1556 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/funcmakers.pyi
+-rw-r--r--   0        0        0     6511 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/funcs.pyi
+-rw-r--r--   0        0        0      894 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/objects.pyi
+-rw-r--r--   0        0        0      650 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/primitives.pyi
+-rw-r--r--   0        0        0    25370 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/seqs.pyi
+-rw-r--r--   0        0        0     1555 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/strings.pyi
+-rw-r--r--   0        0        0      784 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/tree.pyi
+-rw-r--r--   0        0        0     1530 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/funcy-stubs/types.pyi
+-rw-r--r--   0        0        0     1865 2024-05-18 17:29:17.735479 funcy_typing-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 funcy_typing-2.0.1/PKG-INFO
```

### Comparing `funcy_typing-2.0.0/LICENSE` & `funcy_typing-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/__init__.pyi` & `funcy_typing-2.0.1/funcy-stubs/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     get_lax,
     has_path,
     invoke,
     is_distinct,
     iteritems,
     itervalues,
     join,
+    join_with,
     linvoke,
     lpluck,
     lpluck_attr,
     lwhere,
     merge,
+    merge_with,
     none,
     omit,
     one,
     pluck,
     pluck_attr,
     project,
     select,
@@ -72,14 +74,15 @@
     retry,
     silent,
     suppress,
     throttle,
     wrap_with,
 )
 from .funcmakers import make_func, make_pred
+from .funcools import all_fn, any_fn, none_fn, one_fn, some_fn
 from .funcs import (
     autocurry,
     caller,
     complement,
     compose,
     constantly,
     curry,
@@ -122,16 +125,19 @@
     iterate,
     keep,
     last,
     lcat,
     lchunks,
     lconcat,
     ldistinct,
+    lfilter,
     lflatten,
     lkeep,
+    lmap,
+    lmapcat,
     lpartition,
     lpartition_by,
     lreductions,
     lremove,
     lsplit,
     lsplit_at,
     lsplit_by,
@@ -182,200 +188,210 @@
     is_set,
     is_tuple,
     isa,
     iterable,
 )
 
 __all__ = (
-    "tree_leaves",
-    "ltree_leaves",
-    "tree_nodes",
-    "ltree_nodes",
-    "ContextDecorator",
-    "ErrorRateExceeded",
-    "LazyObject",
-    "accumulate",
-    "all",
-    "any",
-    "autocurry",
-    "butlast",
+    "memoize",
+    "make_lookuper",
+    "silent_lookuper",
     "cache",
-    "cached_property",
-    "cached_readonly",
-    "caller",
-    "cat",
-    "chain",
-    "chunks",
-    "collecting",
-    "compact",
-    "complement",
-    "compose",
-    "concat",
-    "constantly",
-    "contextmanager",
-    "count",
-    "count_by",
-    "count_reps",
-    "curry",
-    "cut_prefix",
-    "cut_suffix",
-    "cycle",
-    "dec",
-    "decorator",
-    "del_in",
-    "distinct",
-    "drop",
-    "dropwhile",
     "empty",
-    "even",
-    "fallback",
-    "filter",
-    "first",
-    "flatten",
+    "iteritems",
+    "itervalues",
+    "join",
+    "merge",
+    "join_with",
+    "merge_with",
+    "walk",
+    "walk_keys",
+    "walk_values",
+    "select",
+    "select_keys",
+    "select_values",
+    "compact",
+    "is_distinct",
+    "all",
+    "any",
+    "none",
+    "one",
+    "some",
+    "zipdict",
     "flip",
-    "func_partial",
+    "project",
+    "omit",
+    "zip_values",
+    "zip_dicts",
+    "where",
+    "pluck",
+    "pluck_attr",
+    "invoke",
+    "lwhere",
+    "lpluck",
+    "lpluck_attr",
+    "linvoke",
     "get_in",
     "get_lax",
-    "group_by",
-    "group_by_keys",
-    "group_values",
+    "set_in",
+    "update_in",
+    "del_in",
     "has_path",
+    "tap",
+    "log_calls",
+    "print_calls",
+    "log_enters",
+    "print_enters",
+    "log_exits",
+    "print_exits",
+    "log_errors",
+    "print_errors",
+    "log_durations",
+    "print_durations",
+    "log_iter_durations",
+    "print_iter_durations",
+    "decorator",
+    "wraps",
+    "unwrap",
+    "ContextDecorator",
+    "contextmanager",
+    "raiser",
+    "ignore",
+    "silent",
+    "suppress",
+    "nullcontext",
+    "reraise",
+    "retry",
+    "fallback",
+    "limit_error_rate",
+    "ErrorRateExceeded",
+    "throttle",
+    "post_processing",
+    "collecting",
+    "joining",
+    "once",
+    "once_per",
+    "once_per_args",
+    "wrap_with",
+    "make_func",
+    "make_pred",
+    "all_fn",
+    "any_fn",
+    "none_fn",
+    "one_fn",
+    "some_fn",
     "identity",
+    "constantly",
+    "caller",
+    "reduce",
+    "partial",
+    "rpartial",
+    "func_partial",
+    "curry",
+    "rcurry",
+    "autocurry",
     "iffy",
-    "ignore",
-    "ilen",
-    "inc",
-    "interleave",
-    "interpose",
-    "invoke",
-    "is_distinct",
-    "is_iter",
-    "is_list",
-    "is_mapping",
-    "is_seq",
-    "is_seqcoll",
-    "is_seqcont",
-    "is_set",
-    "is_tuple",
-    "isa",
+    "compose",
+    "rcompose",
+    "complement",
+    "juxt",
+    "ljuxt",
+    "cached_property",
+    "cached_readonly",
+    "wrap_prop",
+    "monkey",
+    "LazyObject",
     "isnone",
-    "iterable",
+    "notnone",
+    "inc",
+    "dec",
+    "even",
+    "odd",
+    "count",
+    "cycle",
+    "repeat",
+    "repeatedly",
     "iterate",
-    "iteritems",
-    "itervalues",
-    "join",
-    "joining",
-    "juxt",
-    "keep",
+    "take",
+    "drop",
+    "first",
+    "second",
+    "nth",
     "last",
-    "lcat",
-    "lchunks",
+    "rest",
+    "butlast",
+    "ilen",
+    "map",
+    "filter",
+    "lmap",
+    "lfilter",
+    "remove",
+    "lremove",
+    "keep",
+    "lkeep",
+    "without",
+    "lwithout",
+    "concat",
     "lconcat",
-    "ldistinct",
+    "chain",
+    "cat",
+    "lcat",
+    "flatten",
     "lflatten",
-    "limit_error_rate",
-    "linvoke",
-    "ljuxt",
-    "lkeep",
-    "log_calls",
-    "log_durations",
-    "log_enters",
-    "log_errors",
-    "log_exits",
-    "log_iter_durations",
-    "lpartition",
-    "lpartition_by",
-    "lpluck",
-    "lpluck_attr",
-    "lreductions",
-    "lremove",
+    "mapcat",
+    "lmapcat",
+    "interleave",
+    "interpose",
+    "distinct",
+    "ldistinct",
+    "dropwhile",
+    "takewhile",
+    "split",
     "lsplit",
+    "split_at",
     "lsplit_at",
+    "split_by",
     "lsplit_by",
-    "lsums",
-    "lwhere",
-    "lwithout",
-    "lzip",
-    "make_func",
-    "make_lookuper",
-    "make_pred",
-    "map",
-    "mapcat",
-    "memoize",
-    "merge",
-    "monkey",
-    "none",
-    "notnone",
-    "nth",
-    "nullcontext",
-    "odd",
-    "omit",
-    "once",
-    "once_per",
-    "once_per_args",
-    "one",
-    "pairwise",
-    "partial",
+    "group_by",
+    "group_by_keys",
+    "group_values",
+    "count_by",
+    "count_reps",
     "partition",
+    "lpartition",
+    "chunks",
+    "lchunks",
     "partition_by",
-    "pluck",
-    "pluck_attr",
-    "post_processing",
-    "print_calls",
-    "print_durations",
-    "print_enters",
-    "print_errors",
-    "print_exits",
-    "print_iter_durations",
-    "project",
-    "raiser",
-    "rcompose",
-    "rcurry",
+    "lpartition_by",
+    "with_prev",
+    "with_next",
+    "pairwise",
+    "lzip",
+    "reductions",
+    "lreductions",
+    "sums",
+    "lsums",
+    "accumulate",
+    "re_iter",
     "re_all",
     "re_find",
     "re_finder",
-    "re_iter",
     "re_test",
     "re_tester",
-    "reduce",
-    "reductions",
-    "remove",
-    "repeat",
-    "repeatedly",
-    "reraise",
-    "rest",
-    "retry",
-    "rpartial",
-    "second",
-    "select",
-    "select_keys",
-    "select_values",
-    "set_in",
-    "silent",
-    "silent_lookuper",
-    "some",
-    "split",
-    "split_at",
-    "split_by",
     "str_join",
-    "sums",
-    "suppress",
-    "take",
-    "takewhile",
-    "tap",
-    "throttle",
-    "unwrap",
-    "update_in",
-    "walk",
-    "walk_keys",
-    "walk_values",
-    "where",
-    "with_next",
-    "with_prev",
-    "without",
-    "wrap_prop",
-    "wrap_with",
-    "wraps",
-    "zip_dicts",
-    "zip_values",
-    "zipdict",
+    "cut_prefix",
+    "cut_suffix",
+    "tree_leaves",
+    "ltree_leaves",
+    "tree_nodes",
+    "ltree_nodes",
+    "isa",
+    "is_mapping",
+    "is_set",
+    "is_seq",
+    "is_list",
+    "is_tuple",
+    "is_seqcoll",
+    "is_seqcont",
+    "iterable",
+    "is_iter",
 )
```

### Comparing `funcy_typing-2.0.0/funcy-stubs/_types.py` & `funcy_typing-2.0.1/funcy-stubs/_types.py`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/calc.pyi` & `funcy_typing-2.0.1/funcy-stubs/calc.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/colls.pyi` & `funcy_typing-2.0.1/funcy-stubs/colls.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/debug.pyi` & `funcy_typing-2.0.1/funcy-stubs/debug.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/flow.pyi` & `funcy_typing-2.0.1/funcy-stubs/flow.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/funcmakers.pyi` & `funcy_typing-2.0.1/funcy-stubs/funcmakers.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/funcs.pyi` & `funcy_typing-2.0.1/funcy-stubs/funcs.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/objects.pyi` & `funcy_typing-2.0.1/funcy-stubs/objects.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/primitives.pyi` & `funcy_typing-2.0.1/funcy-stubs/primitives.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/seqs.pyi` & `funcy_typing-2.0.1/funcy-stubs/seqs.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/strings.pyi` & `funcy_typing-2.0.1/funcy-stubs/strings.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/tree.pyi` & `funcy_typing-2.0.1/funcy-stubs/tree.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/funcy-stubs/types.pyi` & `funcy_typing-2.0.1/funcy-stubs/types.pyi`

 * *Files identical despite different names*

### Comparing `funcy_typing-2.0.0/pyproject.toml` & `funcy_typing-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcy-typing"
-version = "2.0.0"
+version = "2.0.1"
 description = "Stubs for funcy package"
 authors = ["Ratschew Fedor <feodor.ra@me.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "funcy-stubs"}
 ]
```

### Comparing `funcy_typing-2.0.0/PKG-INFO` & `funcy_typing-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcy-typing
-Version: 2.0.0
+Version: 2.0.1
 Summary: Stubs for funcy package
 Home-page: https://github.com/feodor-ra/funcy-stubs
 License: MIT
 Keywords: funcy,types,typing,stubs
 Author: Ratschew Fedor
 Author-email: feodor.ra@me.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -31,14 +31,15 @@
 
 - calc
 - colls
 - debug
 - decorators
 - flow
 - funcmakers
+- funcools
 - funcs
 - objects
 - primitives
 - seqs
 - strings
 - tree
 - types
```


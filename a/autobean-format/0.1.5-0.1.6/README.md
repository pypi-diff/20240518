# Comparing `tmp/autobean-format-0.1.5.tar.gz` & `tmp/autobean-format-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autobean-format-0.1.5.tar", last modified: Tue Aug 15 16:54:09 2023, max compression
+gzip compressed data, was "autobean-format-0.1.6.tar", last modified: Sat May 18 13:47:26 2024, max compression
```

## Comparing `autobean-format-0.1.5.tar` & `autobean-format-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2023-08-15 16:53:48.800082 autobean-format-0.1.5/LICENSE
--rw-r--r--   0        0        0     3668 2023-08-15 16:53:48.800082 autobean-format-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/__init__.py
--rw-r--r--   0        0        0      460 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatter.py
--rw-r--r--   0        0        0      183 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/__init__.py
--rw-r--r--   0        0        0      966 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/balance.py
--rw-r--r--   0        0        0     1690 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/base.py
--rw-r--r--   0        0        0      822 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/cost.py
--rw-r--r--   0        0        0     2620 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/file.py
--rw-r--r--   0        0        0      567 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/number.py
--rw-r--r--   0        0        0     1008 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/open.py
--rw-r--r--   0        0        0     1573 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/posting.py
--rw-r--r--   0        0        0      969 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/price.py
--rw-r--r--   0        0        0     1301 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/formatters/tokens.py
--rw-r--r--   0        0        0        0 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/internal/__init__.py
--rw-r--r--   0        0        0      655 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/internal/alignment.py
--rw-r--r--   0        0        0     1080 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/internal/chrono.py
--rw-r--r--   0        0        0      926 2023-08-15 16:53:48.800082 autobean-format-0.1.5/autobean_format/internal/iterating.py
--rw-r--r--   0        0        0    13810 2023-08-15 16:53:48.804082 autobean-format-0.1.5/autobean_format/internal/sorting.py
--rw-r--r--   0        0        0     2957 2023-08-15 16:53:48.804082 autobean-format-0.1.5/autobean_format/main.py
--rw-r--r--   0        0        0     3059 2023-08-15 16:53:48.804082 autobean-format-0.1.5/autobean_format/options_lib.py
--rw-r--r--   0        0        0      665 2023-08-15 16:53:48.804082 autobean-format-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 autobean-format-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-18 13:47:13.022442 autobean-format-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3668 2024-05-18 13:47:13.022442 autobean-format-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 13:47:13.022442 autobean-format-0.1.6/autobean_format/__init__.py
+-rw-r--r--   0        0        0      460 2024-05-18 13:47:13.022442 autobean-format-0.1.6/autobean_format/formatter.py
+-rw-r--r--   0        0        0      183 2024-05-18 13:47:13.022442 autobean-format-0.1.6/autobean_format/formatters/__init__.py
+-rw-r--r--   0        0        0      966 2024-05-18 13:47:13.022442 autobean-format-0.1.6/autobean_format/formatters/balance.py
+-rw-r--r--   0        0        0     1690 2024-05-18 13:47:13.022442 autobean-format-0.1.6/autobean_format/formatters/base.py
+-rw-r--r--   0        0        0      822 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/cost.py
+-rw-r--r--   0        0        0     2620 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/file.py
+-rw-r--r--   0        0        0      567 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/number.py
+-rw-r--r--   0        0        0     1008 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/open.py
+-rw-r--r--   0        0        0     1573 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/posting.py
+-rw-r--r--   0        0        0      969 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/price.py
+-rw-r--r--   0        0        0     1301 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/formatters/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/internal/__init__.py
+-rw-r--r--   0        0        0      655 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/internal/alignment.py
+-rw-r--r--   0        0        0     1080 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/internal/chrono.py
+-rw-r--r--   0        0        0      926 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/internal/iterating.py
+-rw-r--r--   0        0        0    14086 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/internal/sorting.py
+-rw-r--r--   0        0        0     2957 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/main.py
+-rw-r--r--   0        0        0     3059 2024-05-18 13:47:13.026442 autobean-format-0.1.6/autobean_format/options_lib.py
+-rw-r--r--   0        0        0      697 2024-05-18 13:47:13.026442 autobean-format-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 autobean-format-0.1.6/PKG-INFO
```

### Comparing `autobean-format-0.1.5/LICENSE` & `autobean-format-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/README.md` & `autobean-format-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/balance.py` & `autobean-format-0.1.6/autobean_format/formatters/balance.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/base.py` & `autobean-format-0.1.6/autobean_format/formatters/base.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/cost.py` & `autobean-format-0.1.6/autobean_format/formatters/cost.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/file.py` & `autobean-format-0.1.6/autobean_format/formatters/file.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/number.py` & `autobean-format-0.1.6/autobean_format/formatters/number.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/open.py` & `autobean-format-0.1.6/autobean_format/formatters/open.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/posting.py` & `autobean-format-0.1.6/autobean_format/formatters/posting.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/price.py` & `autobean-format-0.1.6/autobean_format/formatters/price.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/formatters/tokens.py` & `autobean-format-0.1.6/autobean_format/formatters/tokens.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/internal/alignment.py` & `autobean-format-0.1.6/autobean_format/internal/alignment.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/internal/chrono.py` & `autobean-format-0.1.6/autobean_format/internal/chrono.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/internal/iterating.py` & `autobean-format-0.1.6/autobean_format/internal/iterating.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/internal/sorting.py` & `autobean-format-0.1.6/autobean_format/internal/sorting.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
 import abc
 import bisect
 import decimal
 import functools
 import heapq
 import itertools
-from typing import TYPE_CHECKING, Any, Generic, Iterable, Iterator, Optional, Self, Sequence, TypeAlias, TypeVar, cast, get_args
+from typing import TYPE_CHECKING, Any, Generic, Iterable, Iterator, Optional, Sequence, TypeAlias, TypeVar, cast, get_args
+from typing_extensions import Self
 
 from autobean_refactor import models
 from . import chrono
 if TYPE_CHECKING:
     from _typeshed import SupportsDunderLT, SupportsDunderGT
 
 _T = TypeVar('_T')
@@ -76,15 +77,15 @@
     def can_go_before(self, other: Self) -> bool:
         """Tests if this entity can go before the other entity."""
 
     @classmethod
     @abc.abstractmethod
     def min(cls, a: Self, b: Self) -> Self:
         """An associative function to summarize the lower bound for can_go_before.
-        
+
         Formally:
         forall x: x.can_go_before(a) && x.can_go_before(b) <=> x.can_go_before(min(a, b))
         """
 
     @classmethod
     @abc.abstractmethod
     def max(cls, a: Self, b: Self) -> Self:
@@ -136,15 +137,15 @@
             running_max = i
             if j:
                 if entity.max(entity, entities[m[j - 1][0]]) is not entity:
                     running_max = m[j - 1][0]
                 p[(running_max, i)] = m[j - 1]
             m[j:j+1] = [(running_max, i)]
             j -= 1
-        
+
     last = m[-1] if m else None
     sorted_i, sorted, unsorted = [], [], []
     while last:
         sorted_i.append(last[1])
         last = p.get(last)
     sorted_i.reverse()
 
@@ -196,18 +197,19 @@
         yield sorted[cursor_sorted:]
     if cursor_unsorted < len(unsorted):
         yield unsorted[cursor_unsorted:]
 
 
 class _OrderedEntry(_Ordered[_Entry]):
 
-    def __init__(self, entry: _Entry) -> None:
+    def __init__(self, entry: _Entry, initial_index: int) -> None:
         super().__init__(entry)
         self.date = entry.date
         self.time = _get_entry_time(entry)
+        self.initial_index = initial_index
 
     def more_successor_permissive_than(self, other: Self) -> bool:
         return self.date < other.date or (self.date == other.date and (
             self.time is None and other.time is not None or
             self.time is not None and other.time is not None and self.time < other.time))
 
     def can_go_before(self, other: Self) -> bool:
@@ -242,22 +244,14 @@
 
 class _OrderedBlock(_Ordered[_Block]):
 
     def __init__(self, block: _Block) -> None:
         super().__init__(block)
         self.entries = cast(Sequence[_OrderedEntry], block) if isinstance(block[0], _OrderedEntry) else None
 
-    @classmethod
-    def from_raw_block(cls, block: Sequence[_TopLevelEntitiy]) -> Self:
-        if isinstance(block[0], get_args(_Entry)):
-            return cls(_OrderedEntry.sort([
-                _OrderedEntry(entry) for entry in cast(list[_Entry], block)]))
-        else:
-            return cls(block)
-
     @functools.cached_property
     def _max(self) -> Optional['_OrderedEntry']:
         if not self.entries:
             return None
         return functools.reduce(_OrderedEntry.max, self.entries)
 
     @functools.cached_property
@@ -285,42 +279,45 @@
         )
 
     def can_go_before(self, other: Self) -> bool:
         return bool(not self._max or not other._min or self._max.can_go_before(other._min))
 
     def simple_sort_key(self) -> Any:
         assert self._min and self._max  # undated blocks must be part of sorted
-        return (self._min.simple_sort_key(), self._max.simple_sort_key())
+        first_entry_index = -1
+        if self.entries:
+            first_entry_index = self.entries[0].initial_index
+        return (self._min.simple_sort_key(), self._max.simple_sort_key(), first_entry_index)
 
     @classmethod
     def merge(cls, sorted: list['_OrderedBlock'], unsorted: list['_OrderedBlock']) -> Iterator['_OrderedBlock']:
-        keyed_unsorted = [(block.simple_sort_key(), i, block) for i, block in enumerate(unsorted)]
+        keyed_unsorted = [(block.simple_sort_key(), block) for block in unsorted]
         heapq.heapify(keyed_unsorted)
         cursor_sorted = 0
         while cursor_sorted < len(sorted) and keyed_unsorted:
-            if sorted[cursor_sorted].can_go_before(keyed_unsorted[0][2]):
+            if sorted[cursor_sorted].can_go_before(keyed_unsorted[0][-1]):
                 yield sorted[cursor_sorted]
                 cursor_sorted += 1
-            elif keyed_unsorted[0][2].can_go_before(sorted[cursor_sorted]):
-                yield heapq.heappop(keyed_unsorted)[2]
+            elif keyed_unsorted[0][-1].can_go_before(sorted[cursor_sorted]):
+                yield heapq.heappop(keyed_unsorted)[-1]
             else:
                 sorted_head_entries = sorted[cursor_sorted].entries
                 cursor_sorted += 1
                 unsorted_block = heapq.heappop(keyed_unsorted)
-                unsorted_head_entries = unsorted_block[2].entries
+                unsorted_head_entries = unsorted_block[-1].entries
                 assert sorted_head_entries is not None
                 assert unsorted_head_entries is not None
                 split_blocks = _merge_entries(sorted_head_entries, unsorted_head_entries)
                 for block in split_blocks:
                     ordered_block = _OrderedBlock(block)
-                    heapq.heappush(keyed_unsorted, (ordered_block.simple_sort_key(), unsorted_block[1], ordered_block))
+                    heapq.heappush(keyed_unsorted, (ordered_block.simple_sort_key(), ordered_block))
         if cursor_sorted < len(sorted):
             yield from sorted[cursor_sorted:]
         while keyed_unsorted:
-            yield heapq.heappop(keyed_unsorted)[2]
+            yield heapq.heappop(keyed_unsorted)[-1]
 
 
 def _sort_compartment(blocks: list[_OrderedBlock]) -> list[Sequence[_TopLevelEntitiy]]:
     blocks = _OrderedBlock.sort(blocks)
 
     sorted_blocks = list[Sequence[_TopLevelEntitiy]]()
     for ordered_block in blocks:
@@ -330,17 +327,26 @@
             sorted_blocks.append(cast(Sequence[_TopLevelEntitiy], ordered_block.value))
     return sorted_blocks
 
 
 def sort_blocks(blocks: Iterable[Sequence[_TopLevelEntitiy]]) -> list[Sequence[_TopLevelEntitiy]]:
     results = []
     compartment = list[_OrderedBlock]()
+    first_entry_index = 0
     for block in blocks:
         if isinstance(block[0], get_args(_CompartmentSplitter)):
             results.extend(_sort_compartment(compartment))
             compartment.clear()
             results.append(block)
+        elif isinstance(block[0], get_args(_Entry)):
+            # sort within block
+            sorted_entries = _OrderedEntry.sort([
+                _OrderedEntry(entry, first_entry_index + offset)
+                for offset, entry in enumerate(cast(list[_Entry], block))
+            ])
+            compartment.append(_OrderedBlock(sorted_entries))
         else:
-            compartment.append(_OrderedBlock.from_raw_block(block))
+            compartment.append(_OrderedBlock(block))
+        first_entry_index += len(block)
     if compartment:
         results.extend(_sort_compartment(compartment))
     return results
```

### Comparing `autobean-format-0.1.5/autobean_format/main.py` & `autobean-format-0.1.6/autobean_format/main.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/autobean_format/options_lib.py` & `autobean-format-0.1.6/autobean_format/options_lib.py`

 * *Files identical despite different names*

### Comparing `autobean-format-0.1.5/pyproject.toml` & `autobean-format-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "autobean-format"
-version = "0.1.5"
+version = "0.1.6"
 description = "Yet another formatter for beancount"
 authors = [
     { name = "SEIAROTg", email = "seiarotg@gmail.com" },
 ]
 dependencies = [
     "autobean-refactor>=0.2.3",
+    "typing-extensions>=4.4.0",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `autobean-format-0.1.5/PKG-INFO` & `autobean-format-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autobean-format
-Version: 0.1.5
+Version: 0.1.6
 Summary: Yet another formatter for beancount
 License: MIT
 Author-email: SEIAROTg <seiarotg@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # autobean-format
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autobean-format Version: 0.1.5 Summary: Yet another
+Metadata-Version: 2.1 Name: autobean-format Version: 0.1.6 Summary: Yet another
 formatter for beancount License: MIT Author-email: SEIAROTg
 gmail.com> Requires-Python: >=3.11 Description-Content-Type: text/markdown #
 autobean-format [![build](https://github.com/SEIAROTg/autobean-format/actions/
 workflows/build.yml/badge.svg)](https://github.com/SEIAROTg/autobean-format/
 actions/workflows/build.yml) [![pypi](https://img.shields.io/pypi/v/autobean-
 format)](https://pypi.org/project/autobean-format/) [![Test Coverage](https://
 api.codeclimate.com/v1/badges/0c09f58b4d6735d7d991/test_coverage)](https://
```


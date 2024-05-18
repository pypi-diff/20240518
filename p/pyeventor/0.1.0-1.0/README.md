# Comparing `tmp/pyeventor-0.1.0.tar.gz` & `tmp/pyeventor-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeventor-0.1.0.tar", max compression
+gzip compressed data, was "pyeventor-1.0.tar", max compression
```

## Comparing `pyeventor-0.1.0.tar` & `pyeventor-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2024-04-15 18:10:13.173560 pyeventor-0.1.0/LICENSE
--rw-r--r--   0        0        0       48 2024-04-15 18:10:13.173648 pyeventor-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2024-05-12 20:50:35.423821 pyeventor-0.1.0/pyeventor/.DS_Store
--rw-r--r--   0        0        0        0 2024-05-06 11:48:46.121034 pyeventor-0.1.0/pyeventor/__init__.py
--rw-r--r--   0        0        0     3887 2024-05-13 15:41:39.870028 pyeventor-0.1.0/pyeventor/aggregate.py
--rw-r--r--   0        0        0     2359 2024-05-13 15:57:11.434785 pyeventor-0.1.0/pyeventor/asyncio/aggregate.py
--rw-r--r--   0        0        0     6607 2024-05-13 21:00:59.786895 pyeventor-0.1.0/pyeventor/asyncio/event_store.py
--rw-r--r--   0        0        0     3382 2024-05-12 15:42:08.769928 pyeventor-0.1.0/pyeventor/decorator.py
--rw-r--r--   0        0        0     1807 2024-05-12 17:46:53.581503 pyeventor-0.1.0/pyeventor/event.py
--rw-r--r--   0        0        0     6431 2024-05-13 21:00:59.797146 pyeventor-0.1.0/pyeventor/event_store.py
--rw-r--r--   0        0        0      154 2024-05-10 12:45:07.424824 pyeventor-0.1.0/pyeventor/exceptions.py
--rw-r--r--   0        0        0     1852 2024-05-13 21:00:59.767763 pyeventor-0.1.0/pyeventor/handler.py
--rw-r--r--   0        0        0     6148 2024-05-12 17:19:33.554601 pyeventor-0.1.0/pyeventor/plugins/.DS_Store
--rw-r--r--   0        0        0     2459 2024-05-13 21:00:59.778990 pyeventor-0.1.0/pyeventor/plugins/in_memory_store.py
--rw-r--r--   0        0        0     5158 2024-05-13 21:00:59.796569 pyeventor-0.1.0/pyeventor/plugins/postgres_store.py
--rw-r--r--   0        0        0      975 2024-05-13 21:41:25.041471 pyeventor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 pyeventor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-15 18:10:13.173560 pyeventor-1.0/LICENSE
+-rw-r--r--   0        0        0       98 2024-05-18 14:59:48.973411 pyeventor-1.0/README.md
+-rw-r--r--   0        0        0     6148 2024-05-12 20:50:35.423821 pyeventor-1.0/pyeventor/.DS_Store
+-rw-r--r--   0        0        0        0 2024-05-06 11:48:46.121034 pyeventor-1.0/pyeventor/__init__.py
+-rw-r--r--   0        0        0     4149 2024-05-16 23:32:02.421882 pyeventor-1.0/pyeventor/aggregate.py
+-rw-r--r--   0        0        0     2535 2024-05-16 23:32:02.421234 pyeventor-1.0/pyeventor/asyncio/aggregate.py
+-rw-r--r--   0        0        0     6596 2024-05-16 23:32:02.421890 pyeventor-1.0/pyeventor/asyncio/event_store.py
+-rw-r--r--   0        0        0     3476 2024-05-16 23:31:55.393876 pyeventor-1.0/pyeventor/decorator.py
+-rw-r--r--   0        0        0     1796 2024-05-16 23:32:02.420493 pyeventor-1.0/pyeventor/event.py
+-rw-r--r--   0        0        0     6431 2024-05-16 22:31:22.958019 pyeventor-1.0/pyeventor/event_store.py
+-rw-r--r--   0        0        0      154 2024-05-10 12:45:07.424824 pyeventor-1.0/pyeventor/exceptions.py
+-rw-r--r--   0        0        0     1972 2024-05-16 23:15:29.046139 pyeventor-1.0/pyeventor/handler.py
+-rw-r--r--   0        0        0     6148 2024-05-12 17:19:33.554601 pyeventor-1.0/pyeventor/plugins/.DS_Store
+-rw-r--r--   0        0        0     2414 2024-05-16 23:32:02.421871 pyeventor-1.0/pyeventor/plugins/in_memory_store.py
+-rw-r--r--   0        0        0     5228 2024-05-16 23:32:02.421001 pyeventor-1.0/pyeventor/plugins/postgres_store.py
+-rw-r--r--   0        0        0     1036 2024-05-18 14:59:05.163433 pyeventor-1.0/pyproject.toml
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 pyeventor-1.0/PKG-INFO
```

### Comparing `pyeventor-0.1.0/LICENSE` & `pyeventor-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeventor-0.1.0/pyeventor/.DS_Store` & `pyeventor-1.0/pyeventor/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyeventor-0.1.0/pyeventor/aggregate.py` & `pyeventor-1.0/pyeventor/aggregate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from pyeventor.event import Event, Snapshot, JsonSnapshot, SnapshotI
+from pyeventor.event import Event, Snapshot, JsonSnapshot
 from uuid import uuid4
 from pyeventor.exceptions import HandlerException
 from typing import Generic, TypeVar, Optional, Protocol, Type
 from pyeventor.handler import EventHandler
 import inspect
 from abc import abstractmethod
 
@@ -26,16 +26,21 @@
     def id(self) -> IdTypeHint:
         return self._aggregate_id
 
 
 class ApplyI(Protocol):
     def _apply_without_saving(self, event: Event) -> "ApplyI":
         if handler := EventHandler.get_handler(type(self), type(event)):
-            handler(self, event)
-            return self
+            for _, v in inspect.signature(handler).parameters.items():
+                if issubclass(v.annotation, self.__class__):
+                    handler(event, self)
+                    return self
+                if issubclass(v.annotation, Event):
+                    handler(self, event)
+                    return self
         raise HandlerException(f"handler for {event.__class__.__name__} not found")
 
     @abstractmethod
     def apply(self, event: Event) -> "ApplyI":
         ...
```

### Comparing `pyeventor-0.1.0/pyeventor/asyncio/aggregate.py` & `pyeventor-1.0/pyeventor/asyncio/aggregate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from abc import ABC, abstractmethod
-from pyeventor.event import Event, Snapshot, JsonSnapshot, SnapshotI
-from uuid import uuid4
+from pyeventor.event import Event
 from pyeventor.exceptions import HandlerException
-from typing import Generic, TypeVar, Optional, Protocol, Type
+from typing import Optional, Protocol
 from pyeventor.handler import EventHandler
 import inspect
 from pyeventor.aggregate import (
     AttributesI,
     SnapshotFromJsonI,
-    SnapshotCreateI,
     IdTypeHint,
     SnapshotCreateJsonI,
 )
 
 
 class ApplyAsyncI(Protocol):
     async def _apply_without_saving(self, event: Event) -> "ApplyAsyncI":
         if handler := EventHandler.get_handler(type(self), type(event)):
-            await handler(self, event)
-            return self
+            for _, v in inspect.signature(handler).parameters.items():
+                if issubclass(v.annotation, self.__class__):
+                    await handler(event, self)
+                    return self
+                if issubclass(v.annotation, Event):
+                    await handler(self, event)
+                    return self
         raise HandlerException(f"handler for {event.__class__.__name__} not found")
 
     @abstractmethod
     async def apply(self, event: Event) -> "ApplyAsyncI":
         ...
```

### Comparing `pyeventor-0.1.0/pyeventor/asyncio/event_store.py` & `pyeventor-1.0/pyeventor/asyncio/event_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Generic, TypeVar, List, Optional, Type, Protocol
 from pyeventor.event import Event, Snapshot
-from pyeventor.aggregate import Aggregate, Projection, IdTypeHint
+from pyeventor.aggregate import Projection, IdTypeHint
 from pyeventor.asyncio.aggregate import AsyncAggregate
 from pyeventor.handler import EventHandler
 from contextlib import asynccontextmanager
 
 AggregateAsyncHint = TypeVar("AggregateAsyncHint", bound=AsyncAggregate)
 SequenceHint = TypeVar("SequenceHint")
```

### Comparing `pyeventor-0.1.0/pyeventor/decorator.py` & `pyeventor-1.0/pyeventor/decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pyeventor.event import Event
 from pyeventor.aggregate import Aggregate, Projection
 from pyeventor.exceptions import RegisterException
 from pyeventor.handler import EventHandler
-
+from pyeventor.asyncio.aggregate import AsyncAggregate
 
 from typing import Union, Type, Callable
 
 
 def register_handler(*register_objects: Union[Type[Event], Type[Aggregate]]):
     class wrapper:
         def __init__(self, handler: Callable):
             self.handler = handler
 
         def __set_name__(
             self, handler_class: Union[Type[Event], Type[Aggregate]], name: str
         ):
             if all(
                 map(
-                    lambda x: isinstance(x, type) and issubclass(x, Event),
+                    lambda x: isinstance(x, type) and issubclass(x, (Event)),
                     register_objects,
                 )
             ):
                 class_handlers = EventHandler.get_aggregate_handlers(handler_class)
                 for event_class in register_objects:
                     existed_handler = class_handlers.get(event_class)
                     if (
@@ -30,15 +30,16 @@
                     ):
                         raise RegisterException(
                             "Register of the same event more than once for the same class is not allowed"
                         )
                     EventHandler.set_handler(handler_class, event_class, self.handler)
             elif all(
                 map(
-                    lambda x: isinstance(x, type) and issubclass(x, Aggregate),
+                    lambda x: isinstance(x, type)
+                    and issubclass(x, (Aggregate, AsyncAggregate)),
                     register_objects,
                 )
             ):
                 for aggregate_class in register_objects:
                     class_handlers = EventHandler.get_aggregate_handlers(
                         aggregate_class
                     )
```

### Comparing `pyeventor-0.1.0/pyeventor/event.py` & `pyeventor-1.0/pyeventor/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from abc import ABC
 from typing import TypeVar, Generic, TYPE_CHECKING, Optional, Protocol
 from datetime import datetime
 import inspect
 
 if TYPE_CHECKING:
-    from pyeventor.aggregate import Aggregate, SnapshotCreateI
+    from pyeventor.aggregate import SnapshotCreateI
 
 
 SequenceHint = TypeVar("SequenceHint")
 EventDataTypeHint = TypeVar("EventDataTypeHint")
 
 
 class SequenceI(Protocol, Generic[SequenceHint]):
```

### Comparing `pyeventor-0.1.0/pyeventor/event_store.py` & `pyeventor-1.0/pyeventor/event_store.py`

 * *Files identical despite different names*

### Comparing `pyeventor-0.1.0/pyeventor/handler.py` & `pyeventor-1.0/pyeventor/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from collections import defaultdict
 
 import inspect
 from typing import Type, Callable, Optional
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, get_args, Any
 
 if TYPE_CHECKING:
     from pyeventor.aggregate import Aggregate
     from pyeventor.event import Event
 
 
 class EventHandler:
@@ -42,16 +42,18 @@
     @classmethod
     def copy_handlers(
         cls, copy_from: Type[Aggregate], copy_to: Type[Aggregate]
     ) -> None:
         cls.__event_handlers__[copy_to] = cls.get_aggregate_handlers(copy_from)
 
     @classmethod
-    def get_event_class_by_name(cls, event_class_name: str) -> Type[Event]:
+    def get_event_class_by_name(cls, event_class_name: str) -> tuple[Type[Event], Any]:
         for event_dict in cls.__event_handlers__.values():
             for event_class in event_dict.keys():
                 if event_class.__name__ == event_class_name:
-                    return event_class
-        return None
+                    type_data = get_args(event_class.__orig_bases__[0])[1]
+                    return event_class, type_data
+
+        return None, None
 
 
 # TODO change back to names from classes as more stable option
```

### Comparing `pyeventor-0.1.0/pyeventor/plugins/.DS_Store` & `pyeventor-1.0/pyeventor/plugins/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyeventor-0.1.0/pyeventor/plugins/in_memory_store.py` & `pyeventor-1.0/pyeventor/plugins/in_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
     EventStore,
     IdTypeHint,
     SequenceHint,
     Event,
     Snapshot,
     AggregateHint,
 )
-from typing import Type, List, Optional, Generic
-from datetime import datetime
+from typing import Type, List, Optional
 from contextlib import contextmanager
 
 
 class InMemoryEventStore(EventStore[AggregateHint, SequenceHint, IdTypeHint]):
     def __init__(self):
         self.events = {}
         self.snapshots = {}
@@ -66,8 +65,8 @@
             snapshots = self.snapshots[aggregate_id]
             if snapshot_type:
                 snapshots = [s for s in snapshots if isinstance(s[1], snapshot_type)]
             if load_at:
                 snapshots = [s for s in snapshots if s[1].sequence_order <= load_at]
             if snapshots:
                 return snapshots[-1][1]
-        return None, None
+        return None
```

### Comparing `pyeventor-0.1.0/pyeventor/plugins/postgres_store.py` & `pyeventor-1.0/pyeventor/plugins/postgres_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.future import select
+import json
 from sqlalchemy import (
     Column,
     Integer,
     String,
     DateTime,
     JSON,
-    ForeignKey,
     Table,
     MetaData,
 )
-import asyncio
 from datetime import datetime
 from contextlib import asynccontextmanager
 from pyeventor.asyncio.event_store import (
     AsyncEventStore,
     IdTypeHint,
     Snapshot,
     SequenceHint,
@@ -69,20 +68,21 @@
                     await session.rollback()  # Rollback transaction on errors
                     raise e
                 else:
                     await session.commit()  # Explicit commit if no errors
 
     async def save_events(self, events: List[Event], aggregate_id: IdTypeHint) -> None:
         async with self.transaction() as session:
+
             for event in events:
                 await session.execute(
                     event_table.insert().values(
                         aggregate_id=aggregate_id,
                         type=event.__class__.__name__,
-                        data=event.data,
+                        data=json.dumps(event.data),
                         sequence_order=event.sequence_order,
                     )
                 )
 
     async def save_snapshots(
         self, snapshots: list[Snapshot], aggregate_id: IdTypeHint
     ) -> None:
@@ -114,16 +114,18 @@
                 stmt = stmt.where(event_table.c.sequence_order > gt)
             if lte:
                 stmt = stmt.where(event_table.c.sequence_order <= lte)
             result = await session.execute(stmt)
 
             events = []
             for r in result.all():
-                event_class = EventHandler.get_event_class_by_name(r[2])
-                event = event_class(data=r[3], sequence_order=r[4])
+                event_class, event_data = EventHandler.get_event_class_by_name(r[2])
+                event = event_class(
+                    data=event_data(**json.loads(r[3])), sequence_order=r[4]
+                )
                 events.append(event)
 
             return events
 
     async def get_last_snapshot(
         self,
         aggregate_id: IdTypeHint,
```

### Comparing `pyeventor-0.1.0/pyproject.toml` & `pyeventor-1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyeventor"
-version = "0.1.0"
+version = "1.0"
 description = ""
 authors = ["darkllen <yankiniigor@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sqlalchemy = "^2.0.30"
@@ -15,22 +15,25 @@
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 mypy = "^1.10.0"
 ruff = "^0.4.4"
 pytest-asyncio = "^0.23.6"
 build = "^1.2.1"
 uv = "^0.1.42"
+twine = "^5.0.0"
+sphinx = "^7.3.7"
+sphinx-rtd-theme = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "pyeventor"
-version = "0.1"
+version = "1.0"
 authors = [
   { name="Ihor Yankin", email="yankiniigor@gmail.com" },
 ]
 description = "Event sourcing package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pyeventor-0.1.0/PKG-INFO` & `pyeventor-1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeventor
-Version: 0.1.0
+Version: 1.0
 Summary: 
 Author: darkllen
 Author-email: yankiniigor@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,7 +15,8 @@
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pyeventor
 Event Sourcing framework for Python
 
+docs: https://pyeventor.readthedocs.io/en/latest/
```


# Comparing `tmp/beanqueue-0.1.0.tar.gz` & `tmp/beanqueue-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanqueue-0.1.0.tar", max compression
+gzip compressed data, was "beanqueue-0.1.2.tar", max compression
```

## Comparing `beanqueue-0.1.0.tar` & `beanqueue-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2024-05-12 18:00:40.830995 beanqueue-0.1.0/LICENSE
--rw-r--r--   0        0        0       80 2024-05-12 18:00:40.830995 beanqueue-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-12 19:24:59.909458 beanqueue-0.1.0/bq/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 18:35:44.235893 beanqueue-0.1.0/bq/cmds/__init__.py
--rw-r--r--   0        0        0      609 2024-05-16 18:19:43.340992 beanqueue-0.1.0/bq/cmds/create_tables.py
--rw-r--r--   0        0        0     5879 2024-05-17 00:56:24.037787 beanqueue-0.1.0/bq/cmds/process.py
--rw-r--r--   0        0        0     1148 2024-05-17 01:33:52.347825 beanqueue-0.1.0/bq/cmds/submit.py
--rw-r--r--   0        0        0     1508 2024-05-17 01:27:40.690776 beanqueue-0.1.0/bq/config.py
--rw-r--r--   0        0        0     1558 2024-05-16 19:04:30.101750 beanqueue-0.1.0/bq/container.py
--rw-r--r--   0        0        0        0 2024-05-12 19:42:53.784431 beanqueue-0.1.0/bq/db/__init__.py
--rw-r--r--   0        0        0       88 2024-05-12 20:03:37.248757 beanqueue-0.1.0/bq/db/base.py
--rw-r--r--   0        0        0      157 2024-05-16 02:56:09.121086 beanqueue-0.1.0/bq/db/session.py
--rw-r--r--   0        0        0      114 2024-05-13 01:07:30.189418 beanqueue-0.1.0/bq/models/__init__.py
--rw-r--r--   0        0        0      184 2024-05-12 20:03:37.259285 beanqueue-0.1.0/bq/models/helpers.py
--rw-r--r--   0        0        0     3604 2024-05-17 01:26:03.881801 beanqueue-0.1.0/bq/models/task.py
--rw-r--r--   0        0        0     1940 2024-05-16 02:31:35.393950 beanqueue-0.1.0/bq/models/worker.py
--rw-r--r--   0        0        0        0 2024-05-15 16:16:07.381088 beanqueue-0.1.0/bq/processors/__init__.py
--rw-r--r--   0        0        0     4554 2024-05-17 01:26:03.861149 beanqueue-0.1.0/bq/processors/registry.py
--rw-r--r--   0        0        0        0 2024-05-13 00:24:49.883632 beanqueue-0.1.0/bq/services/__init__.py
--rw-r--r--   0        0        0     3463 2024-05-16 18:55:34.032165 beanqueue-0.1.0/bq/services/dispatch.py
--rw-r--r--   0        0        0     2554 2024-05-16 19:08:19.470126 beanqueue-0.1.0/bq/services/worker.py
--rw-r--r--   0        0        0      643 2024-05-17 01:51:45.334551 beanqueue-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 beanqueue-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-17 03:55:03.999015 beanqueue-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9488 2024-05-17 03:55:03.999015 beanqueue-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/cmds/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/cmds/create_tables.py
+-rw-r--r--   0        0        0     5879 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/cmds/process.py
+-rw-r--r--   0        0        0     1148 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/cmds/submit.py
+-rw-r--r--   0        0        0     1508 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/config.py
+-rw-r--r--   0        0        0     1558 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/container.py
+-rw-r--r--   0        0        0        0 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/db/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/db/base.py
+-rw-r--r--   0        0        0      152 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/db/session.py
+-rw-r--r--   0        0        0      110 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/models/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/models/helpers.py
+-rw-r--r--   0        0        0     3604 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/models/task.py
+-rw-r--r--   0        0        0     1871 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/models/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/processors/__init__.py
+-rw-r--r--   0        0        0     4418 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/processors/registry.py
+-rw-r--r--   0        0        0        0 2024-05-17 03:55:03.999015 beanqueue-0.1.2/bq/services/__init__.py
+-rw-r--r--   0        0        0     3463 2024-05-17 03:55:04.003015 beanqueue-0.1.2/bq/services/dispatch.py
+-rw-r--r--   0        0        0     2485 2024-05-17 03:55:04.003015 beanqueue-0.1.2/bq/services/worker.py
+-rw-r--r--   0        0        0      643 2024-05-17 03:55:04.003015 beanqueue-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10242 1970-01-01 00:00:00.000000 beanqueue-0.1.2/PKG-INFO
```

### Comparing `beanqueue-0.1.0/LICENSE` & `beanqueue-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/cmds/create_tables.py` & `beanqueue-0.1.2/bq/cmds/create_tables.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/cmds/process.py` & `beanqueue-0.1.2/bq/cmds/process.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/cmds/submit.py` & `beanqueue-0.1.2/bq/cmds/submit.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/config.py` & `beanqueue-0.1.2/bq/config.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/container.py` & `beanqueue-0.1.2/bq/container.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/models/task.py` & `beanqueue-0.1.2/bq/models/task.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/models/worker.py` & `beanqueue-0.1.2/bq/models/worker.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import enum
-
-from sqlalchemy import Column
-from sqlalchemy import DateTime
-from sqlalchemy import Enum
-from sqlalchemy import func
-from sqlalchemy import String
-from sqlalchemy.dialects.postgresql import ARRAY
-from sqlalchemy.dialects.postgresql import UUID
-from sqlalchemy.orm import relationship
-
-from ..db.base import Base
-from .helpers import make_repr_attrs
-
-
-class WorkerState(enum.Enum):
-    # the worker is running
-    RUNNING = "RUNNING"
-    # the worker shuts down normally
-    SHUTDOWN = "SHUTDOWN"
-    # The worker has no heartbeat for a while
-    NO_HEARTBEAT = "NO_HEARTBEAT"
-
-
-class Worker(Base):
-    id = Column(
-        UUID(as_uuid=True), primary_key=True, server_default=func.gen_random_uuid()
-    )
-    # current state of the worker
-    state = Column(
-        Enum(WorkerState),
-        nullable=False,
-        default=WorkerState.RUNNING,
-        server_default=WorkerState.RUNNING.value,
-        index=True,
-    )
-    # name of the worker
-    name = Column(String, nullable=False)
-    # the channels we are processing
-    channels = Column(ARRAY(String), nullable=False)
-    # last heartbeat of this worker
-    last_heartbeat = Column(
-        DateTime(timezone=True),
-        nullable=False,
-        server_default=func.now(),
-        index=True,
-    )
-    # created datetime of the worker
-    created_at = Column(
-        DateTime(timezone=True), nullable=False, server_default=func.now()
-    )
-
-    tasks = relationship(
-        "Task",
-        back_populates="worker",
-        cascade="all,delete",
-        order_by="Task.created_at",
-    )
-
-    __tablename__ = "bq_workers"
-
-    def __repr__(self) -> str:
-        items = [
-            ("id", self.id),
-            ("name", self.name),
-            ("channels", self.channels),
-            ("state", self.state),
-        ]
-        return f"<{self.__class__.__name__} {make_repr_attrs(items)}>"
+import enum
+
+from sqlalchemy import Column
+from sqlalchemy import DateTime
+from sqlalchemy import Enum
+from sqlalchemy import func
+from sqlalchemy import String
+from sqlalchemy.dialects.postgresql import ARRAY
+from sqlalchemy.dialects.postgresql import UUID
+from sqlalchemy.orm import relationship
+
+from ..db.base import Base
+from .helpers import make_repr_attrs
+
+
+class WorkerState(enum.Enum):
+    # the worker is running
+    RUNNING = "RUNNING"
+    # the worker shuts down normally
+    SHUTDOWN = "SHUTDOWN"
+    # The worker has no heartbeat for a while
+    NO_HEARTBEAT = "NO_HEARTBEAT"
+
+
+class Worker(Base):
+    id = Column(
+        UUID(as_uuid=True), primary_key=True, server_default=func.gen_random_uuid()
+    )
+    # current state of the worker
+    state = Column(
+        Enum(WorkerState),
+        nullable=False,
+        default=WorkerState.RUNNING,
+        server_default=WorkerState.RUNNING.value,
+        index=True,
+    )
+    # name of the worker
+    name = Column(String, nullable=False)
+    # the channels we are processing
+    channels = Column(ARRAY(String), nullable=False)
+    # last heartbeat of this worker
+    last_heartbeat = Column(
+        DateTime(timezone=True),
+        nullable=False,
+        server_default=func.now(),
+        index=True,
+    )
+    # created datetime of the worker
+    created_at = Column(
+        DateTime(timezone=True), nullable=False, server_default=func.now()
+    )
+
+    tasks = relationship(
+        "Task",
+        back_populates="worker",
+        cascade="all,delete",
+        order_by="Task.created_at",
+    )
+
+    __tablename__ = "bq_workers"
+
+    def __repr__(self) -> str:
+        items = [
+            ("id", self.id),
+            ("name", self.name),
+            ("channels", self.channels),
+            ("state", self.state),
+        ]
+        return f"<{self.__class__.__name__} {make_repr_attrs(items)}>"
```

### Comparing `beanqueue-0.1.0/bq/processors/registry.py` & `beanqueue-0.1.2/bq/processors/registry.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-import collections
-import dataclasses
-import inspect
-import logging
-import typing
-
-import venusian
-from sqlalchemy.orm import object_session
-
-from bq import models
-
-BQ_PROCESSOR_CATEGORY = "bq_processor"
-
-
-@dataclasses.dataclass(frozen=True)
-class Processor:
-    channel: str
-    module: str
-    name: str
-    func: typing.Callable
-    # should we auto complete the task or not
-    auto_complete: bool = True
-    # should we auto rollback the transaction when encounter unhandled exception
-    auto_rollback_on_exc: bool = True
-
-
-class ProcessorHelper:
-    def __init__(self, processor: Processor, task_cls: typing.Type = models.Task):
-        self._processor = processor
-        self._task_cls = task_cls
-
-    def __call__(self, *args, **kwargs):
-        return self._processor.func(*args, **kwargs)
-
-    def run(self, **kwargs) -> models.Task:
-        return self._task_cls(
-            channel=self._processor.channel,
-            module=self._processor.module,
-            func_name=self._processor.name,
-            kwargs=kwargs,
-        )
-
-
-def process_task(task: models.Task, processor: Processor):
-    logger = logging.getLogger(__name__)
-    db = object_session(task)
-    func_signature = inspect.signature(processor.func)
-    base_kwargs = {}
-    if "task" in func_signature.parameters:
-        base_kwargs["task"] = task
-    if "db" in func_signature.parameters:
-        base_kwargs["db"] = db
-    with db.begin_nested() as savepoint:
-        try:
-            result = processor.func(**base_kwargs, **task.kwargs)
-            savepoint.commit()
-        except Exception as exc:
-            logger.error("Unhandled exception for task %s", task.id, exc_info=True)
-            if processor.auto_rollback_on_exc:
-                savepoint.rollback()
-            # TODO: add error event
-            task.state = models.TaskState.FAILED
-            task.error_message = str(exc)
-            db.add(task)
-            return
-    if processor.auto_complete:
-        logger.info("Task %s auto complete", task.id)
-        task.state = models.TaskState.DONE
-        task.result = result
-        db.add(task)
-    return result
-
-
-class Registry:
-    def __init__(self):
-        self.logger = logging.getLogger(__name__)
-        self.processors = collections.defaultdict(lambda: collections.defaultdict(dict))
-
-    def add(self, processor: Processor):
-        self.processors[processor.channel][processor.module][processor.name] = processor
-
-    def process(self, task: models.Task) -> typing.Any:
-        modules = self.processors.get(task.channel, {})
-        functions = modules.get(task.module, {})
-        processor = functions.get(task.func_name)
-        db = object_session(task)
-        if processor is None:
-            self.logger.error(
-                "Cannot find processor for task %s with module=%s, func=%s",
-                task.id,
-                task.module,
-                task.func_name,
-            )
-            # TODO: add error event
-            task.state = models.TaskState.FAILED
-            task.error_message = f"Cannot find processor for task with module={task.module}, func={task.func_name}"
-            db.add(task)
-            return
-        return process_task(task, processor)
-
-
-def processor(
-    channel: str,
-    auto_complete: bool = True,
-    auto_rollback_on_exc: bool = True,
-    task_cls: typing.Type = models.Task,
-) -> typing.Callable:
-    def decorator(wrapped: typing.Callable):
-        processor = Processor(
-            module=wrapped.__module__,
-            name=wrapped.__name__,
-            channel=channel,
-            func=wrapped,
-            auto_complete=auto_complete,
-            auto_rollback_on_exc=auto_rollback_on_exc,
-        )
-        helper_obj = ProcessorHelper(processor, task_cls=task_cls)
-
-        def callback(scanner: venusian.Scanner, name: str, ob: typing.Callable):
-            if processor.name != name:
-                raise ValueError("Name is not the same")
-            scanner.registry.add(processor)
-
-        venusian.attach(helper_obj, callback, category=BQ_PROCESSOR_CATEGORY)
-        return helper_obj
-
-    return decorator
-
-
-def collect(packages: list[typing.Any], registry: Registry | None = None) -> Registry:
-    if registry is None:
-        registry = Registry()
-    scanner = venusian.Scanner(registry=registry)
-    for package in packages:
-        scanner.scan(package, categories=(BQ_PROCESSOR_CATEGORY,))
-    return registry
+import collections
+import dataclasses
+import inspect
+import logging
+import typing
+
+import venusian
+from sqlalchemy.orm import object_session
+
+from bq import models
+
+BQ_PROCESSOR_CATEGORY = "bq_processor"
+
+
+@dataclasses.dataclass(frozen=True)
+class Processor:
+    channel: str
+    module: str
+    name: str
+    func: typing.Callable
+    # should we auto complete the task or not
+    auto_complete: bool = True
+    # should we auto rollback the transaction when encounter unhandled exception
+    auto_rollback_on_exc: bool = True
+
+
+class ProcessorHelper:
+    def __init__(self, processor: Processor, task_cls: typing.Type = models.Task):
+        self._processor = processor
+        self._task_cls = task_cls
+
+    def __call__(self, *args, **kwargs):
+        return self._processor.func(*args, **kwargs)
+
+    def run(self, **kwargs) -> models.Task:
+        return self._task_cls(
+            channel=self._processor.channel,
+            module=self._processor.module,
+            func_name=self._processor.name,
+            kwargs=kwargs,
+        )
+
+
+def process_task(task: models.Task, processor: Processor):
+    logger = logging.getLogger(__name__)
+    db = object_session(task)
+    func_signature = inspect.signature(processor.func)
+    base_kwargs = {}
+    if "task" in func_signature.parameters:
+        base_kwargs["task"] = task
+    if "db" in func_signature.parameters:
+        base_kwargs["db"] = db
+    with db.begin_nested() as savepoint:
+        try:
+            result = processor.func(**base_kwargs, **task.kwargs)
+            savepoint.commit()
+        except Exception as exc:
+            logger.error("Unhandled exception for task %s", task.id, exc_info=True)
+            if processor.auto_rollback_on_exc:
+                savepoint.rollback()
+            # TODO: add error event
+            task.state = models.TaskState.FAILED
+            task.error_message = str(exc)
+            db.add(task)
+            return
+    if processor.auto_complete:
+        logger.info("Task %s auto complete", task.id)
+        task.state = models.TaskState.DONE
+        task.result = result
+        db.add(task)
+    return result
+
+
+class Registry:
+    def __init__(self):
+        self.logger = logging.getLogger(__name__)
+        self.processors = collections.defaultdict(lambda: collections.defaultdict(dict))
+
+    def add(self, processor: Processor):
+        self.processors[processor.channel][processor.module][processor.name] = processor
+
+    def process(self, task: models.Task) -> typing.Any:
+        modules = self.processors.get(task.channel, {})
+        functions = modules.get(task.module, {})
+        processor = functions.get(task.func_name)
+        db = object_session(task)
+        if processor is None:
+            self.logger.error(
+                "Cannot find processor for task %s with module=%s, func=%s",
+                task.id,
+                task.module,
+                task.func_name,
+            )
+            # TODO: add error event
+            task.state = models.TaskState.FAILED
+            task.error_message = f"Cannot find processor for task with module={task.module}, func={task.func_name}"
+            db.add(task)
+            return
+        return process_task(task, processor)
+
+
+def processor(
+    channel: str,
+    auto_complete: bool = True,
+    auto_rollback_on_exc: bool = True,
+    task_cls: typing.Type = models.Task,
+) -> typing.Callable:
+    def decorator(wrapped: typing.Callable):
+        processor = Processor(
+            module=wrapped.__module__,
+            name=wrapped.__name__,
+            channel=channel,
+            func=wrapped,
+            auto_complete=auto_complete,
+            auto_rollback_on_exc=auto_rollback_on_exc,
+        )
+        helper_obj = ProcessorHelper(processor, task_cls=task_cls)
+
+        def callback(scanner: venusian.Scanner, name: str, ob: typing.Callable):
+            if processor.name != name:
+                raise ValueError("Name is not the same")
+            scanner.registry.add(processor)
+
+        venusian.attach(helper_obj, callback, category=BQ_PROCESSOR_CATEGORY)
+        return helper_obj
+
+    return decorator
+
+
+def collect(packages: list[typing.Any], registry: Registry | None = None) -> Registry:
+    if registry is None:
+        registry = Registry()
+    scanner = venusian.Scanner(registry=registry)
+    for package in packages:
+        scanner.scan(package, categories=(BQ_PROCESSOR_CATEGORY,))
+    return registry
```

### Comparing `beanqueue-0.1.0/bq/services/dispatch.py` & `beanqueue-0.1.2/bq/services/dispatch.py`

 * *Files identical despite different names*

### Comparing `beanqueue-0.1.0/bq/services/worker.py` & `beanqueue-0.1.2/bq/services/worker.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import datetime
-import typing
-
-from sqlalchemy import func
-from sqlalchemy.orm import Query
-from sqlalchemy.orm import Session
-
-from .. import models
-
-
-class WorkerService:
-    def __init__(self, session: Session):
-        self.session = session
-
-    def update_heartbeat(self, worker: models.Worker):
-        worker.last_heartbeat = func.now()
-        self.session.add(worker)
-
-    def make_dead_worker_query(self, timeout: int, limit: int = 5) -> Query:
-        return (
-            self.session.query(models.Worker.id)
-            .filter(
-                models.Worker.last_heartbeat
-                < (func.now() - datetime.timedelta(seconds=timeout))
-            )
-            .filter(models.Worker.state == models.WorkerState.RUNNING)
-            .limit(limit)
-            .with_for_update(skip_locked=True)
-        )
-
-    def make_update_dead_worker_query(self, worker_query: typing.Any):
-        return (
-            models.Worker.__table__.update()
-            .where(models.Worker.id.in_(worker_query))
-            .values(
-                state=models.WorkerState.NO_HEARTBEAT,
-            )
-            .returning(models.Worker.id)
-        )
-
-    def fetch_dead_workers(self, timeout: int, limit: int = 5) -> Query:
-        dead_worker_query = self.make_dead_worker_query(timeout=timeout, limit=limit)
-        dead_worker_subquery = dead_worker_query.scalar_subquery()
-        worker_ids = [
-            item[0]
-            for item in self.session.execute(
-                self.make_update_dead_worker_query(dead_worker_subquery)
-            )
-        ]
-        # TODO: ideally returning with (models.Task) should return the whole model, but SQLAlchemy is returning
-        #       it columns in rows. We can save a round trip if we can find out how to solve this
-        return self.session.query(models.Worker).filter(
-            models.Worker.id.in_(worker_ids)
-        )
-
-    def make_update_tasks_query(self, worker_query: typing.Any):
-        return (
-            models.Task.__table__.update()
-            .where(models.Task.worker_id.in_(worker_query))
-            .where(models.Task.state == models.TaskState.PROCESSING)
-            .values(
-                state=models.TaskState.PENDING,
-            )
-        )
-
-    def reschedule_dead_tasks(self, worker_query: typing.Any) -> int:
-        update_dead_task_query = self.make_update_tasks_query(worker_query=worker_query)
-        res = self.session.execute(update_dead_task_query)
-        return res.rowcount
+import datetime
+import typing
+
+from sqlalchemy import func
+from sqlalchemy.orm import Query
+from sqlalchemy.orm import Session
+
+from .. import models
+
+
+class WorkerService:
+    def __init__(self, session: Session):
+        self.session = session
+
+    def update_heartbeat(self, worker: models.Worker):
+        worker.last_heartbeat = func.now()
+        self.session.add(worker)
+
+    def make_dead_worker_query(self, timeout: int, limit: int = 5) -> Query:
+        return (
+            self.session.query(models.Worker.id)
+            .filter(
+                models.Worker.last_heartbeat
+                < (func.now() - datetime.timedelta(seconds=timeout))
+            )
+            .filter(models.Worker.state == models.WorkerState.RUNNING)
+            .limit(limit)
+            .with_for_update(skip_locked=True)
+        )
+
+    def make_update_dead_worker_query(self, worker_query: typing.Any):
+        return (
+            models.Worker.__table__.update()
+            .where(models.Worker.id.in_(worker_query))
+            .values(
+                state=models.WorkerState.NO_HEARTBEAT,
+            )
+            .returning(models.Worker.id)
+        )
+
+    def fetch_dead_workers(self, timeout: int, limit: int = 5) -> Query:
+        dead_worker_query = self.make_dead_worker_query(timeout=timeout, limit=limit)
+        dead_worker_subquery = dead_worker_query.scalar_subquery()
+        worker_ids = [
+            item[0]
+            for item in self.session.execute(
+                self.make_update_dead_worker_query(dead_worker_subquery)
+            )
+        ]
+        # TODO: ideally returning with (models.Task) should return the whole model, but SQLAlchemy is returning
+        #       it columns in rows. We can save a round trip if we can find out how to solve this
+        return self.session.query(models.Worker).filter(
+            models.Worker.id.in_(worker_ids)
+        )
+
+    def make_update_tasks_query(self, worker_query: typing.Any):
+        return (
+            models.Task.__table__.update()
+            .where(models.Task.worker_id.in_(worker_query))
+            .where(models.Task.state == models.TaskState.PROCESSING)
+            .values(
+                state=models.TaskState.PENDING,
+            )
+        )
+
+    def reschedule_dead_tasks(self, worker_query: typing.Any) -> int:
+        update_dead_task_query = self.make_update_tasks_query(worker_query=worker_query)
+        res = self.session.execute(update_dead_task_query)
+        return res.rowcount
```

### Comparing `beanqueue-0.1.0/pyproject.toml` & `beanqueue-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanqueue"
-version = "0.1.0"
+version = "0.1.2"
 description = "BeanQueue or BQ for short, PostgreSQL SKIP LOCK based worker queue library"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "bq" },
 ]
```


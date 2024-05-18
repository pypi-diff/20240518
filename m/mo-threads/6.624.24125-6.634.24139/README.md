# Comparing `tmp/mo_threads-6.624.24125.tar.gz` & `tmp/mo_threads-6.634.24139.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_threads-6.624.24125.tar", last modified: Sat May  4 20:10:39 2024, max compression
+gzip compressed data, was "mo_threads-6.634.24139.tar", last modified: Sat May 18 06:48:15 2024, max compression
```

## Comparing `mo_threads-6.624.24125.tar` & `mo_threads-6.634.24139.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 20:10:39.153215 mo_threads-6.624.24125/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:49:14.000000 mo_threads-6.624.24125/LICENSE
--rw-rw-rw-   0        0        0    15469 2024-05-04 20:10:39.152214 mo_threads-6.624.24125/PKG-INFO
--rw-rw-rw-   0        0        0    13826 2024-03-02 21:24:19.000000 mo_threads-6.624.24125/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 20:10:39.133511 mo_threads-6.624.24125/mo_threads/
--rw-rw-rw-   0        0        0     1410 2024-01-25 03:29:49.000000 mo_threads-6.624.24125/mo_threads/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-07-25 23:07:11.000000 mo_threads-6.624.24125/mo_threads/busy_lock.py
--rw-rw-rw-   0        0        0    13797 2024-02-04 22:43:25.000000 mo_threads-6.624.24125/mo_threads/commands.py
--rw-rw-rw-   0        0        0      869 2022-04-29 11:15:19.000000 mo_threads-6.624.24125/mo_threads/futures.py
--rw-rw-rw-   0        0        0     3389 2023-10-29 22:49:42.000000 mo_threads-6.624.24125/mo_threads/lock.py
--rw-rw-rw-   0        0        0    11882 2024-02-04 22:43:25.000000 mo_threads-6.624.24125/mo_threads/processes.py
--rw-rw-rw-   0        0        0     1118 2022-02-26 02:35:54.000000 mo_threads-6.624.24125/mo_threads/profile_utils.py
--rw-rw-rw-   0        0        0     2760 2023-07-25 23:07:11.000000 mo_threads-6.624.24125/mo_threads/profiles.py
--rw-rw-rw-   0        0        0     5858 2024-02-04 22:03:09.000000 mo_threads-6.624.24125/mo_threads/python.py
--rw-rw-rw-   0        0        0     4386 2024-01-25 03:29:49.000000 mo_threads-6.624.24125/mo_threads/python_worker.py
--rw-rw-rw-   0        0        0    18735 2023-10-29 22:49:42.000000 mo_threads-6.624.24125/mo_threads/queues.py
--rw-rw-rw-   0        0        0     2126 2023-07-25 23:07:11.000000 mo_threads-6.624.24125/mo_threads/repeat.py
--rw-rw-rw-   0        0        0     3778 2023-07-25 23:07:11.000000 mo_threads-6.624.24125/mo_threads/schedule.py
--rw-rw-rw-   0        0        0     8674 2024-01-07 17:48:41.000000 mo_threads-6.624.24125/mo_threads/signals.py
--rw-rw-rw-   0        0        0    25448 2024-02-05 05:39:50.000000 mo_threads-6.624.24125/mo_threads/threads.py
--rw-rw-rw-   0        0        0     4981 2023-12-16 17:20:59.000000 mo_threads-6.624.24125/mo_threads/till.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:10:39.150203 mo_threads-6.624.24125/mo_threads.egg-info/
--rw-rw-rw-   0        0        0    15469 2024-05-04 20:10:39.000000 mo_threads-6.624.24125/mo_threads.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-04 20:10:39.000000 mo_threads-6.624.24125/mo_threads.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 20:10:39.000000 mo_threads-6.624.24125/mo_threads.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:32:35.000000 mo_threads-6.624.24125/mo_threads.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      238 2024-05-04 20:10:39.000000 mo_threads-6.624.24125/mo_threads.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 20:10:39.000000 mo_threads-6.624.24125/mo_threads.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 20:10:39.153215 mo_threads-6.624.24125/setup.cfg
--rw-rw-rw-   0        0        0    15353 2024-05-04 20:10:34.000000 mo_threads-6.624.24125/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 06:48:15.772578 mo_threads-6.634.24139/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:49:14.000000 mo_threads-6.634.24139/LICENSE
+-rw-rw-rw-   0        0        0    15469 2024-05-18 06:48:15.772578 mo_threads-6.634.24139/PKG-INFO
+-rw-rw-rw-   0        0        0    13826 2024-03-02 21:24:19.000000 mo_threads-6.634.24139/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 06:48:15.746455 mo_threads-6.634.24139/mo_threads/
+-rw-rw-rw-   0        0        0     1436 2024-05-18 06:48:04.000000 mo_threads-6.634.24139/mo_threads/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-07-25 23:07:11.000000 mo_threads-6.634.24139/mo_threads/busy_lock.py
+-rw-rw-rw-   0        0        0    13797 2024-05-18 06:48:04.000000 mo_threads-6.634.24139/mo_threads/commands.py
+-rw-rw-rw-   0        0        0      869 2022-04-29 11:15:19.000000 mo_threads-6.634.24139/mo_threads/futures.py
+-rw-rw-rw-   0        0        0     3389 2023-10-29 22:49:42.000000 mo_threads-6.634.24139/mo_threads/lock.py
+-rw-rw-rw-   0        0        0    11882 2024-05-18 06:48:04.000000 mo_threads-6.634.24139/mo_threads/processes.py
+-rw-rw-rw-   0        0        0     1118 2022-02-26 02:35:54.000000 mo_threads-6.634.24139/mo_threads/profile_utils.py
+-rw-rw-rw-   0        0        0     2760 2023-07-25 23:07:11.000000 mo_threads-6.634.24139/mo_threads/profiles.py
+-rw-rw-rw-   0        0        0     5858 2024-05-18 06:48:04.000000 mo_threads-6.634.24139/mo_threads/python.py
+-rw-rw-rw-   0        0        0     4386 2024-01-25 03:29:49.000000 mo_threads-6.634.24139/mo_threads/python_worker.py
+-rw-rw-rw-   0        0        0    18735 2024-05-18 06:48:04.000000 mo_threads-6.634.24139/mo_threads/queues.py
+-rw-rw-rw-   0        0        0     2126 2023-07-25 23:07:11.000000 mo_threads-6.634.24139/mo_threads/repeat.py
+-rw-rw-rw-   0        0        0     3778 2023-07-25 23:07:11.000000 mo_threads-6.634.24139/mo_threads/schedule.py
+-rw-rw-rw-   0        0        0     8674 2024-01-07 17:48:41.000000 mo_threads-6.634.24139/mo_threads/signals.py
+-rw-rw-rw-   0        0        0    25427 2024-05-18 06:48:04.000000 mo_threads-6.634.24139/mo_threads/threads.py
+-rw-rw-rw-   0        0        0     4981 2023-12-16 17:20:59.000000 mo_threads-6.634.24139/mo_threads/till.py
+drwxrwxrwx   0        0        0        0 2024-05-18 06:48:15.767595 mo_threads-6.634.24139/mo_threads.egg-info/
+-rw-rw-rw-   0        0        0    15469 2024-05-18 06:48:15.000000 mo_threads-6.634.24139/mo_threads.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-18 06:48:15.000000 mo_threads-6.634.24139/mo_threads.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 06:48:15.000000 mo_threads-6.634.24139/mo_threads.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:32:35.000000 mo_threads-6.634.24139/mo_threads.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      238 2024-05-18 06:48:15.000000 mo_threads-6.634.24139/mo_threads.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 06:48:15.000000 mo_threads-6.634.24139/mo_threads.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 06:48:15.772578 mo_threads-6.634.24139/setup.cfg
+-rw-rw-rw-   0        0        0    15353 2024-05-18 06:48:09.000000 mo_threads-6.634.24139/setup.py
```

### Comparing `mo_threads-6.624.24125/LICENSE` & `mo_threads-6.634.24139/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/PKG-INFO` & `mo_threads-6.634.24139/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-threads
-Version: 6.624.24125
+Version: 6.634.24139
 Summary: More Threads! Simpler and faster threading.
 Home-page: https://github.com/klahnakoski/mo-threads
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,19 +13,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.623.24125
+Requires-Dist: mo-dots==10.632.24139
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.623.24125
-Requires-Dist: mo-math==7.623.24125
-Requires-Dist: mo-times==5.623.24125
+Requires-Dist: mo-logs==8.632.24139
+Requires-Dist: mo-math==7.632.24139
+Requires-Dist: mo-times==5.632.24139
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.587.24110; extra == "tests"
 Requires-Dist: jx-python>=4.586.24095; extra == "tests"
 Requires-Dist: psutil>=5.9.8; extra == "tests"
 Requires-Dist: objgraph>=3.6.1; extra == "tests"
 Requires-Dist: mo-files>=6.585.24095; extra == "tests"
 Requires-Dist: mo-json>=6.584.24095; extra == "tests"
```

### Comparing `mo_threads-6.624.24125/README.md` & `mo_threads-6.634.24139/README.md`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/__init__.py` & `mo_threads-6.634.24139/mo_threads/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 from mo_threads.futures import Future
 from mo_threads.lock import Lock
 from mo_threads.processes import Process
 from mo_threads.queues import Queue, ThreadedQueue
 from mo_threads.signals import Signal, DONE, NEVER
 from mo_threads.threads import (
     MainThread,
-    THREAD_STOP,
+    PLEASE_STOP,
     THREAD_TIMEOUT,
     Thread,
     stop_main_thread,
     register_thread,
     wait_for_shutdown_signal,
     start_main_thread,
     join_all_threads,
     current_thread,
 )
 from mo_threads.till import Till
 
+THREAD_STOP = PLEASE_STOP
 export("mo_threads.signals", threads)
 del threads
 
 
 def coverage_detector():
     try:
         # DETECT COVERAGE
```

### Comparing `mo_threads-6.624.24125/mo_threads/busy_lock.py` & `mo_threads-6.634.24139/mo_threads/busy_lock.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/commands.py` & `mo_threads-6.634.24139/mo_threads/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from mo_times import Date, SECOND
 
 from mo_threads import threads
 from mo_threads.lock import Lock
 from mo_threads.processes import os_path, Process
 from mo_threads.queues import Queue
 from mo_threads.signals import Signal
-from mo_threads.threads import THREAD_STOP, Thread
+from mo_threads.threads import PLEASE_STOP, Thread
 from mo_threads.till import Till
 
 DEBUG = False
 
 STALE_MAX_AGE = 60
 INUSE_TIMEOUT = 5
 AVAIL_TIMEOUT = 60 * 60
@@ -113,15 +113,15 @@
         try:
             line_count = 0
 
             while not please_stop:
                 value = source.pop(till=please_stop)
                 if value is None:
                     continue
-                elif value is THREAD_STOP:
+                elif value is PLEASE_STOP:
                     self.debug and logger.info("got thread stop")
                     return
                 elif line_count == 0 and "is not recognized as an internal or external command" in value:
                     self.debug and logger.info("exit with error")
                     logger.error("Problem with command: {desc}", desc=value)
                 elif PROMPT and value.startswith(PROMPT):
                     # DO NOT RETURN WHAT WAS SENT
@@ -131,34 +131,34 @@
                     self.returncode = int(source.pop(till=please_stop))
                     self.debug and logger.info("prompt located, {code}, clean finish", code=self.returncode)
                     return
                 else:
                     line_count += 1
                     destination.add(value)
         finally:
-            destination.add(THREAD_STOP)
-            # self.process.stderr.add(THREAD_STOP)
+            destination.add(PLEASE_STOP)
+            # self.process.stderr.add(PLEASE_STOP)
             self.stderr_thread.please_stop.go()
             self.stderr_thread.join()
             self.manager.return_process(self.process)
             self.debug and logger.info("command worker done")
 
 
 def _stderr_relay(source, destination, please_stop=None):
     while not please_stop:
         value = source.pop(till=please_stop)
-        if value is THREAD_STOP:
+        if value is PLEASE_STOP:
             break
         if value:
             destination.add(value)
     for value in source.pop_all():
-        if value and value is not THREAD_STOP:
+        if value and value is not PLEASE_STOP:
             destination.add(value)
 
-    destination.add(THREAD_STOP)
+    destination.add(PLEASE_STOP)
 
 
 class LifetimeManager:
     def __init__(self):
         global lifetime_manager
         DEBUG and logger.info("new manager")
         self.locker = Lock()
@@ -212,15 +212,15 @@
         # WAIT FOR START
         try:
             process.stdin.add("cd " + cmd_escape(cwd))
             process.stdin.add(LAST_RETURN_CODE)
             start_timeout = Till(seconds=START_TIMEOUT)
             while not start_timeout:
                 value = process.stdout.pop(till=start_timeout)
-                if value == THREAD_STOP:
+                if value == PLEASE_STOP:
                     process.kill_once()
                     process.join()
                     logger.error("Could not start command, stdout closed early")
                 if value and value.startswith(END_OF_COMMAND_MARKER):
                     break
             process.stdout.pop(till=start_timeout)  # GET THE ERROR LEVEL
             if start_timeout:
```

### Comparing `mo_threads-6.624.24125/mo_threads/futures.py` & `mo_threads-6.634.24139/mo_threads/futures.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/lock.py` & `mo_threads-6.634.24139/mo_threads/lock.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/processes.py` & `mo_threads-6.634.24139/mo_threads/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from mo_future import is_windows, utcnow
 from mo_logs import logger, strings
 from mo_logs.exceptions import Except
 from mo_times import Timer, Date
 
 from mo_threads.queues import Queue
 from mo_threads.signals import Signal
-from mo_threads.threads import THREAD_STOP, Thread, EndOfThread, ALL_LOCK, ALL
+from mo_threads.threads import PLEASE_STOP, Thread, EndOfThread, ALL_LOCK, ALL
 from mo_threads.till import Till
 
 DEBUG = False
 
 next_process_id_locker = allocate_lock()
 next_process_id = 0
 
@@ -280,17 +280,17 @@
             self.please_stop.go()
             receive.close()
             pipe.close()
 
     def _writer(self, pipe, send, please_stop):
         while not please_stop:
             line = send.pop(till=please_stop)
-            if line is THREAD_STOP:
+            if line is PLEASE_STOP:
                 please_stop.go()
-                self.debug and logger.info("got THREAD_STOP")
+                self.debug and logger.info("got PLEASE_STOP")
                 break
             elif line is None:
                 continue
             self.second_last_stdin = self.last_stdin
             self.last_stdin = line
             self.debug and logger.info(
                 "send line: {line}", process=self.name, line=line.rstrip(),
```

### Comparing `mo_threads-6.624.24125/mo_threads/profile_utils.py` & `mo_threads-6.634.24139/mo_threads/profile_utils.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/profiles.py` & `mo_threads-6.634.24139/mo_threads/profiles.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/python.py` & `mo_threads-6.634.24139/mo_threads/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import sys
 from json import dumps as value2json, loads as json2value
 
 from mo_dots import to_data, from_data
 from mo_future import is_windows
 from mo_logs import Except, logger
-from mo_threads import Lock, Process, Signal, THREAD_STOP, Thread, DONE, python_worker
+from mo_threads import Lock, Process, Signal, PLEASE_STOP, Thread, DONE, python_worker
 
 DEBUG = False
 
 
 class Python(object):
     def __init__(self, name, config, parent_thread=None):
         python_exe = sys.executable
@@ -44,15 +44,15 @@
             | {
                 "debug": {"trace": True},
                 "constants": {"mo_threads": {"signals": {"DEBUG": False}, "lock": {"DEBUG": False}}},
             }
         )))
         while True:
             line = self.process.stdout.pop()
-            if line == THREAD_STOP:
+            if line == PLEASE_STOP:
                 logger.error("problem starting python process: STOP detected on stdout")
             if line == '{"out":"ok"}':
                 break
             logger.info("waiting to start python: {line}", line=line)
         self.lock = Lock("wait for response from " + name)
         self.stop_error = None
         self.done = DONE
@@ -83,15 +83,15 @@
             self.response = None
             self.error = None
 
     def _watch_stdout(self, please_stop):
         while not please_stop:
             line = self.process.stdout.pop(till=please_stop)
             DEBUG and logger.info("stdout got {line}", line=line)
-            if line == THREAD_STOP:
+            if line == PLEASE_STOP:
                 please_stop.go()
                 break
             elif not line:
                 continue
 
             try:
                 data = to_data(json2value(line))
@@ -113,15 +113,15 @@
         DEBUG and logger.info("stdout reader is done")
 
     def _watch_stderr(self, please_stop):
         while not please_stop:
             try:
                 line = self.process.stderr.pop(till=please_stop)
                 DEBUG and logger.info("stderr got {line}", line=line)
-                if line is None or line == THREAD_STOP:
+                if line is None or line == PLEASE_STOP:
                     please_stop.go()
                     break
                 logger.info(
                     "Error line from {name}({pid}): {line}", line=line, name=self.process.name, pid=self.process.pid,
                 )
             except Exception as cause:
                 logger.error("could not process line", cause=cause)
```

### Comparing `mo_threads-6.624.24125/mo_threads/python_worker.py` & `mo_threads-6.634.24139/mo_threads/python_worker.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/queues.py` & `mo_threads-6.634.24139/mo_threads/queues.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from time import time
 
 from mo_dots import Null, coalesce
 from mo_logs import Except, logger
 
 from mo_threads.lock import Lock
 from mo_threads.signals import Signal
-from mo_threads.threads import THREAD_STOP, THREAD_TIMEOUT, Thread
+from mo_threads.threads import PLEASE_STOP, THREAD_TIMEOUT, Thread
 from mo_threads.till import Till
 
 DEBUG = False
 
 # MAX_DATETIME = datetime(2286, 11, 20, 17, 46, 39)
 DEFAULT_WAIT_TIME = 10 * 60  # SECONDS
 
@@ -59,30 +59,30 @@
         self.lock = Lock("lock for queue " + name)
         self.queue = deque()
 
     def __iter__(self):
         try:
             while True:
                 value = self.pop()
-                if value is THREAD_STOP:
+                if value is PLEASE_STOP:
                     break
                 if value is not None:
                     yield value
         except Exception as cause:
             logger.warning("Tell me about what happened here", cause)
 
     def add(self, value, timeout=None, force=False):
         """
         :param value:  ADDED THE THE QUEUE
         :param timeout:  HOW LONG TO WAIT FOR QUEUE TO NOT BE FULL
         :param force:  ADD TO QUEUE, EVEN IF FULL (USE ONLY WHEN CONSUMER IS RETURNING WORK TO THE QUEUE)
         :return: self
         """
         with self.lock:
-            if value is THREAD_STOP:
+            if value is PLEASE_STOP:
                 # INSIDE THE lock SO THAT EXITING WILL RELEASE wait()
                 self.queue.append(value)
                 self.closed.go()
                 return
 
             if not force:
                 self._wait_for_queue_space(timeout=timeout)
@@ -135,22 +135,22 @@
 
         with self.lock:
             # ONCE THE queue IS BELOW LIMIT, ALLOW ADDING MORE
             self._wait_for_queue_space()
             if not self.closed:
                 if self.unique:
                     for v in values:
-                        if v is THREAD_STOP:
+                        if v is PLEASE_STOP:
                             self.closed.go()
                             continue
                         if v not in self.queue:
                             self.queue.append(v)
                 else:
                     for v in values:
-                        if v is THREAD_STOP:
+                        if v is PLEASE_STOP:
                             self.closed.go()
                             continue
                         self.queue.append(v)
         return self
 
     def _wait_for_queue_space(self, timeout=None):
         """
@@ -188,24 +188,24 @@
 
     def __len__(self):
         with self.lock:
             return len(self.queue)
 
     def __nonzero__(self):
         with self.lock:
-            return any(r != THREAD_STOP for r in self.queue)
+            return any(r != PLEASE_STOP for r in self.queue)
 
     def pop(self, till=None):
         """
         WAIT FOR NEXT ITEM ON THE QUEUE
-        RETURN THREAD_STOP IF QUEUE IS CLOSED
+        RETURN PLEASE_STOP IF QUEUE IS CLOSED
         RETURN None IF till IS REACHED AND QUEUE IS STILL EMPTY
 
         :param till:  A `Signal` to stop waiting and return None
-        :return:  A value, or a THREAD_STOP or None
+        :return:  A value, or a PLEASE_STOP or None
         """
         if till is not None and not isinstance(till, Signal):
             logger.error("expecting a signal")
 
         with self.lock:
             while True:
                 if self.queue:
@@ -213,15 +213,15 @@
                 if self.closed:
                     break
                 if not self.lock.wait(till=self.closed | till):
                     if self.closed:
                         break
                     return None
         (DEBUG or not self.silent) and logger.info("{name} queue closed", name=self.name, stack_depth=1)
-        return THREAD_STOP
+        return PLEASE_STOP
 
     def pop_all(self):
         """
         NON-BLOCKING POP ALL IN QUEUE, IF ANY
         """
         with self.lock:
             output = list(self.queue)
@@ -231,20 +231,20 @@
 
     def pop_one(self):
         """
         NON-BLOCKING POP IN QUEUE, IF ANY
         """
         with self.lock:
             if self.closed:
-                return THREAD_STOP
+                return PLEASE_STOP
             elif not self.queue:
                 return None
             else:
                 v = self.queue.popleft()
-                if v is THREAD_STOP:  # SENDING A STOP INTO THE QUEUE IS ALSO AN OPTION
+                if v is PLEASE_STOP:  # SENDING A STOP INTO THE QUEUE IS ALSO AN OPTION
                     self.closed.go()
                 return v
 
     def close(self):
         self.closed.go()
 
     def commit(self):
@@ -275,27 +275,27 @@
             for _ in range(numpriorities)
         ]
 
     def __iter__(self):
         try:
             while True:
                 value = self.pop(self.closed)
-                if value is THREAD_STOP:
+                if value is PLEASE_STOP:
                     break
                 if value is not None:
                     yield value
         except Exception as cause:
             logger.warning("Tell me about what happened here", cause)
 
         if not self.silent:
             logger.info("queue iterator is done")
 
     def add(self, value, timeout=None, priority=0):
         with self.lock:
-            if value is THREAD_STOP:
+            if value is PLEASE_STOP:
                 # INSIDE THE lock SO THAT EXITING WILL RELEASE wait()
                 self.queue[priority].queue.append(value)
                 self.closed.go()
                 return
 
             self.queue[priority]._wait_for_queue_space(timeout=timeout)
             if self.closed and not self.queue[priority].allow_add_after_close:
@@ -323,30 +323,30 @@
 
     def __len__(self):
         with self.lock:
             return sum([len(q.queue) for q in self.queue])
 
     def __nonzero__(self):
         with self.lock:
-            return any(any(r != THREAD_STOP for r in q.queue) for q in self.queue)
+            return any(any(r != PLEASE_STOP for r in q.queue) for q in self.queue)
 
     def highest_entry(self):
         for count, q in enumerate(self.queue):
             if len(q) > 0:
                 return count
         return None
 
     def pop(self, till=None, priority=None):
         """
         WAIT FOR NEXT ITEM ON THE QUEUE
-        RETURN THREAD_STOP IF QUEUE IS CLOSED
+        RETURN PLEASE_STOP IF QUEUE IS CLOSED
         RETURN None IF till IS REACHED AND QUEUE IS STILL EMPTY
 
         :param till:  A `Signal` to stop waiting and return None
-        :return:  A value, or a THREAD_STOP or None
+        :return:  A value, or a PLEASE_STOP or None
         """
         if till is not None and not isinstance(till, Signal):
             logger.error("expecting a signal")
 
         with self.lock:
             while True:
                 if not priority:
@@ -357,15 +357,15 @@
                 if self.closed:
                     break
                 if not self.lock.wait(till=till | self.closed):
                     if self.closed:
                         break
                     return None
         (DEBUG or not self.silent) and logger.info(self.name + " queue stopped")
-        return THREAD_STOP
+        return PLEASE_STOP
 
     def pop_all(self, priority=None):
         """
         NON-BLOCKING POP ALL IN QUEUE, IF ANY
         """
         output = []
         with self.lock:
@@ -392,20 +392,20 @@
         """
         NON-BLOCKING POP IN QUEUE, IF ANY
         """
         with self.lock:
             if not priority:
                 priority = self.highest_entry()
             if self.closed:
-                return [THREAD_STOP]
+                return [PLEASE_STOP]
             elif not self.queue:
                 return None
             else:
                 v = self.pop(priority=priority)
-                if v is THREAD_STOP:  # SENDING A STOP INTO THE QUEUE IS ALSO AN OPTION
+                if v is PLEASE_STOP:  # SENDING A STOP INTO THE QUEUE IS ALSO AN OPTION
                     self.closed.go()
                 return v
 
 
 class ThreadedQueue(Queue):
     """
     DISPATCH TO ANOTHER (SLOWER) queue IN BATCHES OF GIVEN size
@@ -437,15 +437,15 @@
         self.thread = (
             Thread
             .run(f"threaded queue for {name}", self.worker_bee, batch_size, period, error_target, parent_thread=self)
             .release()
         )
 
     def worker_bee(self, batch_size, period, error_target, please_stop):
-        please_stop.then(lambda: self.add(THREAD_STOP))
+        please_stop.then(lambda: self.add(PLEASE_STOP))
 
         _buffer = []
         _post_push_functions = []
         now = time()
         next_push = Till(till=now + period)  # THE TIME WE SHOULD DO A PUSH
         last_push = now - period
 
@@ -466,15 +466,15 @@
                     now = time()
                     if now > last_push + period:
                         next_push = Till(till=now + period)
                 else:
                     item = self.pop(till=next_push)
                     now = time()
 
-                if item is THREAD_STOP:
+                if item is PLEASE_STOP:
                     push_to_queue()
                     please_stop.go()
                     break
                 elif isinstance(item, types.FunctionType):
                     _post_push_functions.append(item)
                 elif item is not None:
                     _buffer.append(item)
@@ -512,15 +512,15 @@
                         num=len(_buffer),
                         cause=cause,
                     )
 
         if _buffer:
             # ONE LAST PUSH, DO NOT HAVE TIME TO DEAL WITH ERRORS
             push_to_queue()
-        self.slow_queue.add(THREAD_STOP)
+        self.slow_queue.add(PLEASE_STOP)
 
     def add_child(self, child):
         pass
 
     def add(self, value, timeout=None):
         with self.lock:
             self._wait_for_queue_space(timeout=timeout)
@@ -538,16 +538,16 @@
                 logger.info("{name} has {num} items", name=self.name, num=len(self.queue))
         return self
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.add(THREAD_STOP)
+        self.add(PLEASE_STOP)
         if isinstance(exc_val, BaseException):
             self.thread.please_stop.go()
         self.thread.join()
 
     def stop(self):
-        self.add(THREAD_STOP)
+        self.add(PLEASE_STOP)
         self.thread.join()
         return self
```

### Comparing `mo_threads-6.624.24125/mo_threads/repeat.py` & `mo_threads-6.634.24139/mo_threads/repeat.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/schedule.py` & `mo_threads-6.634.24139/mo_threads/schedule.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/signals.py` & `mo_threads-6.634.24139/mo_threads/signals.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads/threads.py` & `mo_threads-6.634.24139/mo_threads/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 DEBUG = False
 KNOWN_DEBUGGERS = ["pydevd.py"]
 
 PLEASE_STOP = "please_stop"  # REQUIRED thread PARAMETER TO SIGNAL STOP
 PARENT_THREAD = "parent_thread"  # OPTIONAL PARAMETER TO ASSIGN THREAD TO SOMETHING OTHER THAN CURRENT THREAD
 MAX_DATETIME = datetime(2286, 11, 20, 17, 46, 39)
 DEFAULT_WAIT_TIME = timedelta(minutes=10)
-THREAD_STOP = "stop"
 THREAD_TIMEOUT = "Thread {name} timeout"
 COVERAGE_COLLECTOR = None  # Detect Coverage.py
 
 datetime.strptime("2012-01-01", "%Y-%m-%d")  # http://bugs.python.org/issue7980
 
 cprofiler_stats = None  # ACCUMULATION OF STATS FROM ALL THREADS
```

### Comparing `mo_threads-6.624.24125/mo_threads/till.py` & `mo_threads-6.634.24139/mo_threads/till.py`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/mo_threads.egg-info/PKG-INFO` & `mo_threads-6.634.24139/mo_threads.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-threads
-Version: 6.624.24125
+Version: 6.634.24139
 Summary: More Threads! Simpler and faster threading.
 Home-page: https://github.com/klahnakoski/mo-threads
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,19 +13,19 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.623.24125
+Requires-Dist: mo-dots==10.632.24139
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.623.24125
-Requires-Dist: mo-math==7.623.24125
-Requires-Dist: mo-times==5.623.24125
+Requires-Dist: mo-logs==8.632.24139
+Requires-Dist: mo-math==7.632.24139
+Requires-Dist: mo-times==5.632.24139
 Provides-Extra: tests
 Requires-Dist: mo-testing>=7.587.24110; extra == "tests"
 Requires-Dist: jx-python>=4.586.24095; extra == "tests"
 Requires-Dist: psutil>=5.9.8; extra == "tests"
 Requires-Dist: objgraph>=3.6.1; extra == "tests"
 Requires-Dist: mo-files>=6.585.24095; extra == "tests"
 Requires-Dist: mo-json>=6.584.24095; extra == "tests"
```

### Comparing `mo_threads-6.624.24125/mo_threads.egg-info/SOURCES.txt` & `mo_threads-6.634.24139/mo_threads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mo_threads-6.624.24125/setup.py` & `mo_threads-6.634.24139/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Threads! Simpler and faster threading.',
     extras_require={"tests":["mo-testing>=7.587.24110","jx-python>=4.586.24095","psutil>=5.9.8","objgraph>=3.6.1","mo-files>=6.585.24095","mo-json>=6.584.24095"]},
     include_package_data=True,
-    install_requires=["mo-dots==10.623.24125","mo-future==7.584.24095","mo-logs==8.623.24125","mo-math==7.623.24125","mo-times==5.623.24125"],
+    install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095","mo-logs==8.632.24139","mo-math==7.632.24139","mo-times==5.632.24139"],
     license='MPL 2.0',
     long_description='\n# More Threads!\n\n\n|Branch      | Status                                                                                                                                                                                                                                                                                                                                         |\n|------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n|master      |  [![Build Status](https://github.com/klahnakoski/mo-threads/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-threads/actions/workflows/build.yml)                                                                                                                                                                                                     |\n|dev         | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-threads.svg?branch=dev)](https://travis-ci.com/github/klahnakoski/mo-threads)  [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-threads/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-threads?branch=dev) ← child thread coverage is missing |\n\n## Module `threads`\n\nThe main benefits over Python\'s threading library is:\n\n1. **Multi-threaded queues do not use serialization** - Serialization is \ngreat in the general case, where you may also be communicating between \nprocesses, but it is a needless overhead for single-process multi-threading. \nIt is left to the programmer to ensure the messages put on the queue are \nnot changed, which is not ominous demand.\n2. **Shutdown order is deterministic and explicit** - Python\'s threading \nlibrary is missing strict conventions for controlled and orderly shutdown. \nEach thread can shutdown on its own terms, but is expected to do so expediently.\n    * All threads are required to accept a `please_stop` signal; are \n    expected to test it in a timely manner; and expected to exit when signalled.\n    * All threads have a parent - The parent is responsible for ensuring their children get the `please_stop` signal, and are dead, before stopping themselves. This responsibility is baked into the thread spawning process, \n  so you need not deal with it unless you want.\n3. Uses [**Signals**](#signal-class) to simplify logical \ndependencies among multiple threads, events, and timeouts.\n4. **Logging and Profiling is Integrated** - Logging and exception handling \nis seamlessly integrated: This means logs are centrally handled, and thread \nsafe. Parent threads have access to uncaught child thread exceptions, and \nthe cProfiler properly aggregates results from the multiple threads.\n\n\n### What\'s it used for\n\nA good amount of time is spent waiting for underlying C libraries and OS\nservices to respond to network and file access requests. Multiple\nthreads can make your code faster, despite the GIL, when dealing with those\nrequests. For example, by moving logging off the main thread, we can get\nup to 15% increase in overall speed because we no longer have the main thread\nwaiting for disk writes or remote logging posts. Please note, this level of\nspeed improvement can only be realized if there is no serialization happening\nat the multi-threaded queue.  \n\n### Do not use Async\n\n[Actors](http://en.wikipedia.org/wiki/Actor_model) are easier to reason about than [async tasks](https://docs.python.org/3/library/asyncio-task.html). Mixing regular methods and co-routines (with their `yield from` pollution) is dangerous because:\n\n1. calling styles between synchronous and asynchronous methods can be easily confused\n2. actors can use blocking methods, async can not\n3. there is no way to manage resource priority with co-routines.\n4. stack traces are lost with co-routines\n5. async scope easily escapes lexical scope, which promotes bugs \n\nPython\'s async efforts are still immature; a re-invention of threading functionality by another name. Expect to experience a decade of problems that are already solved by threading; [here is an example](https://www.python.org/dev/peps/pep-0550/).  \n\n## Reading\n\n* Fibers were an async experiment using a stack, as opposed to the state-machine-based async Python uses now. It does not apply to my argument, but is an interesting read: [[Fibers are] not an appropriate solution for writing scalable concurrent software](http://www.open-std.org/JTC1/SC22/WG21/docs/papers/2018/p1364r0.pdf)\n\n\n## Writing threaded functions\n\nAll threaded functions must accept a `please_stop` parameter, which is a `Signal` to indicate the desire to stop.  The function should check this signal often, and do it\'s best to promptly return. \n\n#### Simple work loop\n\nFor threaded functions that perform small chunks of work in some loop; the chunks are small enough that they will complete soon enough. Simply check the `please_stop` signal at the start of each loop:\n\n    def worker(p1, p2, please_stop):\n        while not please_stop:\n            do_some_small_chunk_of_work(p1)\n            \n#### One-time work\n            \nSometimes, threads are launched to perform low priority, one-time work. You may not need to check the `please_stop` signal: \n    \n    def worker(p1, p2, please_stop):\n         do_some_work_and_exit(p1, p2)\n\n#### Passing signals to others\n         \nThere are many times a more complex `please_stop` checks are required. For example, we want to wait on an input queue for the next task.  Many of the methods in `mo-threads` accept `Signals` instead of timeouts so they return quickly when signalled. You may pass the `please_stop` signal to these methods, or make your own.  Be sure to check if the method returned because it is done, or it returned because it was signaled to stop early.\n         \n```python \ndef worker(source, please_stop):\n     while not please_stop:\n        data = source.pop(till=please_stop)\n        if please_stop:  # did pop() return because of please_stop?\n            return\n        chunk_of_work(data)\n```\n\n#### Combining signals\n            \nWork might be done on some regular interval: The threaded function will sleep for a period and perform some work. In these cases you can combine Signals and `wait()` on either of them:\n\n```python \ndef worker(please_stop):\n    while not please_stop:\n        next_event = Till(seconds=1000)\n        (next_event | please_stop).wait()\n        if please_stop:  # is wait done because of please_stop?\n            return\n        chunk_of_work()\n```\n\n## Spawning threads\n\nMost threads will be declared and run in a single line. It is much like Python\'s threading library, except it demands a name for the thread: \n\n    thread = Thread.run("name", function, p1, p2, ...)\n    \nSometimes you want to separate creation from starting:\n\n    thread = Thread("name", function, p1, p2, ...)\n    thread.start()\n    \n   \n### `join()` vs `release()`\n\nOnce a thread is created, a few actions can be performed with the thread object:\n\n* `join()` - Join on `thread` will make the caller thread wait until `thread` has stopped. Then, return the resulting value or to re-raise `thread`\'s exception in the caller.\n\n      result = thread.join()     # may raise exception\n\n* `release()` - Will ignore any return value, and post any exception to logging. Tracking is still performed; released threads are still properly stopped.  You may still `join()` to guarantee the caller will wait for thread completion, but you risk being too late: The thread may have already completed and logged it\'s failure.\n\n      thread.release()     # release thread resources asap, when done\n  \n* `stopped.wait()` - Every thread has a `stopped` Signal, which can be used for coordination by other threads. This allows a thread to wait for another to be complete and then resume. No errors or return values are captured\n\n      thread.stopped.wait()\n  \n### Registering Threads\n\nThreads created without this module can call your code; You want to ensure these "alien" threads have finished their work, released the locks, and exited your code before stopping. If you register alien threads, then `mo-threads` will ensure the alien work is done for a clean stop. \n\n    def my_method():\n        with RegisterThread():\n            t = Thread.current()   # we can now use mo-threads on this thread \n            print(t.name)          # a name is always given to the alien thread \n\n\n## Synchronization Primitives\n\nThere are three major aspects of a synchronization primitive:\n\n* **Resource** - Monitors and locks can only be owned by one thread at a time\n* **Binary** - The primitive has only two states\n* **Irreversible** - The state of the primitive can only be set, or advanced, never reversed\n\nThe last, *irreversibility* is very useful, but ignored in many threading\nlibraries. The irreversibility allows us to model progression; and\nwe can allow threads to poll for progress, or be notified of progress. \n\nThese three aspects can be combined to give us 8 synchronization primitives:\n\n* `- - -` - Semaphore\n* `- B -` - Event\n* `R - -` - Monitor\n* `R B -` - **[Lock](#lock-class)**\n* `- - I` - Iterator/generator\n* `- B I` - **[Signal](#signal-class)** (or Promise)\n* `R - I` - Private Iterator \n* `R B I` - Private Signal (best implemented as `is_done` Boolean flag)\n\n## `Lock` Class\n\nLocks are identical to [threading monitors](https://en.wikipedia.org/wiki/Monitor_(synchronization)), except for two differences: \n\n1. The `wait()` method will **always acquire the lock before returning**. This is an important feature, it ensures every line inside a `with` block has lock acquisition, and is easier to reason about.\n2. Exiting a lock via `__exit__()` will **always** signal a waiting thread to resume. This ensures no signals are missed, and every thread gets an opportunity to react to possible change.\n3. `Lock` is **not reentrant**! This is a feature to ensure locks are not held for long periods of time.\n\n**Example**\n```python\nlock = Lock()\nwhile not please_stop:\n    with lock:\n        while not todo:\n            lock.wait(seconds=1)\n        # DO SOME WORK\n```\nIn this example, we look for stuff `todo`, and if there is none, we wait for a second. During that time others can acquire the `lock` and add `todo` items. Upon releasing the the `lock`, our example code will immediately resume to see what\'s available, waiting again if nothing is found.\n\n\n## `Signal` Class\n\n[The `Signal` class](mo_threads/signals.py) is a binary semaphore that can be signalled only once; subsequent signals have no effect.\n  * It can be signalled by any thread; \n  * any thread can wait on a `Signal`; and \n  * once signalled, all waiting threads are unblocked, including all subsequent waiting threads. \n  * A Signal\'s current state can be accessed by any thread without blocking.\n   \n`Signal` is used to model thread-safe state advancement. It initializes to `False`, and when signalled (with `go()`) becomes `True`. It can not be reversed.  \n\nSignals are like a Promise, but more explicit \n\n|   Signal     |      Promise       | Python Event |\n|:------------:|:------------------:|:------------:|\n|   s.go()     |    p.resolve()     |    e.set()   |\n| s.then(f)    |     p.then(m)      |              |\n|  s.wait()    |      await p       |   e.wait()   |\n|  bool(s)     |                    |  e.is_set()  |\n|   s & t      | Promise.all(p, q)  |              |\n| s &vert; t   | Promise.race(p, q) |              |\n\n\nHere is simple worker that signals when work is done. It is assumed `do_work` is executed by some other thread.\n\n```python\nclass Worker:\n    def __init__(self):\n        self.is_done = Signal()\n  \n    def do_work(self):\n        do_some_work()\n        self.is_done.go()\n```\n\nYou can attach methods to a `Signal`, which will be run, just once, upon `go()`. If already signalled, then the method is run immediately.\n\n```python\nworker = Worker()\nworker.is_done.then(lambda: print("done"))\n```\n\nYou may also wait on a `Signal`, which will block the current thread until the `Signal` is a go\n\n```python\nworker.is_done.wait()\nprint("worker thread is done")\n```\n\n`Signals` are first class, they can be passed around and combined with other Signals. For example, using the `__or__` operator (`|`):  `either = lhs | rhs`; `either` will be triggered when `lhs` or `rhs` is triggered.\n\n```python\ndef worker(please_stop):\n    while not please_stop:\n        #DO WORK \n\nuser_cancel = Signal("user cancel")\n...\nworker(user_cancel | Till(seconds=360))\n```\n\n`Signal`s can also be combined using logical and (`&`):  `both = lhs & rhs`; `both` is triggered only when both `lhs` and `rhs` are triggered:\n\n```python\n(workerA.stopped & workerB.stopped).wait()\nprint("both threads are done")\n```\n\n### Differences from Python\'s `Event`\n\n* `Signal` is not reversable, while `Event` has a `clear()` method\n* `Signal` allows function chaining using the `then` method\n* Complex signals can be composed from simple signals using boolean logic  \n\n\n\n## `Till` Class\n\n[The `Till` class](mo-threads/till.py) (short for "until") is a special `Signal` used to represent timeouts.  \n\n```python\nTill(seconds=20).wait()\nTill(till=Date("21 Jan 2016").unix).wait()\n```\n\nUse `Till` rather than `sleep()` because you can combine `Till` objects with other `Signals`. \n\n**Beware that all `Till` objects will be triggered before expiry when the main thread is asked to shutdown**\n\n\n## `Command` Class\n\nIf you find process creation is too slow, the `Command` class can be used to recycle existing processes.  It has the same interface as `Process`, yet it manages a `bash` (or `cmd.exe`) session for you in the background.\n\n ',
     long_description_content_type='text/markdown',
     name='mo-threads',
     packages=["mo_threads"],
     url='https://github.com/klahnakoski/mo-threads',
-    version='6.624.24125',
+    version='6.634.24139',
     zip_safe=False
 )
```


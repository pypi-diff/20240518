# Comparing `tmp/PKDevTools-0.13.20240517.119.tar.gz` & `tmp/PKDevTools-0.13.20240517.120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240517.119.tar", last modified: Fri May 17 03:22:41 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240517.120.tar", last modified: Fri May 17 17:27:24 2024, max compression
```

## Comparing `PKDevTools-0.13.20240517.119.tar` & `PKDevTools-0.13.20240517.120.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 03:22:41.187640 PKDevTools-0.13.20240517.119/
--rw-rw-rw-   0        0        0     1086 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-17 03:22:41.172017 PKDevTools-0.13.20240517.119/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:22:41.187640 PKDevTools-0.13.20240517.119/PKDevTools/classes/
--rw-rw-rw-   0        0        0     4960 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2577 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2860 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    14576 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    11018 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-17 03:22:35.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:22:41.172017 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-17 03:22:41.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2024-05-17 03:22:41.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 03:22:41.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-17 03:22:41.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-17 03:22:34.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-17 03:22:41.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 03:22:41.000000 PKDevTools-0.13.20240517.119/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-17 03:22:41.187640 PKDevTools-0.13.20240517.119/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/README.md
--rw-rw-rw-   0        0        0       86 2024-05-17 03:22:41.187640 PKDevTools-0.13.20240517.119/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-17 03:21:16.000000 PKDevTools-0.13.20240517.119/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/
+-rw-rw-rw-   0        0        0     1086 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.645833 PKDevTools-0.13.20240517.120/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     4960 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2608 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2860 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    14576 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5243 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    11651 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-17 17:27:20.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:27:24.645833 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-17 17:27:18.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-17 17:27:24.000000 PKDevTools-0.13.20240517.120/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-17 17:27:24.661450 PKDevTools-0.13.20240517.120/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-17 17:25:41.000000 PKDevTools-0.13.20240517.120/setup.py
```

### Comparing `PKDevTools-0.13.20240517.119/LICENSE` & `PKDevTools-0.13.20240517.120/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/__init__.py` & `PKDevTools-0.13.20240517.120/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/FunctionTimeouts.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     def outer(fn):
         def inner(*args, **kwargs):
             timer = threading.Timer(s, cdquit, args=[fn.__name__])
             timer.start()
             timer_mid = threading.Timer(INTERMEDIATE_NUM_SECONDS_WARN, intermediateMessage, args=[fn.__name__])
             timer_mid.start()
             try:
+                result = None
                 result = fn(*args, **kwargs)
             finally:
                 timer.cancel()
                 timer_mid.cancel()
             return result
         return inner
     return outer
```

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKJoinableQueue.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
 from multiprocessing.queues import JoinableQueue
+from queue import Empty
 import multiprocessing
 
 # The following implementation of custom MyQueue to avoid NotImplementedError
 # when calling queue.qsize() in MacOS X comes almost entirely from this github
 # discussion: https://github.com/keras-team/autokeras/issues/368
 # Necessary modification is made to make the code compatible with Python3.
 
@@ -108,7 +109,14 @@
     def qsize(self):
         """ Reliable implementation of multiprocessing.Queue.qsize() """
         return self.size.value
 
     def empty(self):
         """ Reliable implementation of multiprocessing.Queue.empty() """
         return not self.qsize()
+
+    def clear(self):
+        try:
+            while True:
+                self.get_nowait()
+        except Empty:
+            pass
```

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,14 +113,33 @@
         self.progressCallbackHandler = progressCallbackHandler
         self.fetcher = fetcher
         self.intradayNSEFetcher = None
         self.configManager = configManager
         self.candlePatterns = candlePatterns
         self.screener = screener
         self.refreshDatabase = True
+        self.paused = False
+
+    def _clear(self):
+        self.paused = True
+        try:
+            while True:
+                self.task_queue.get_nowait()
+        except Empty:
+            if self.default_logger is not None:
+                self.default_logger.debug("task_queue empty.")
+            pass
+        try:
+            while True:
+                self.result_queue.get_nowait()
+        except Empty:
+            if self.default_logger is not None:
+                self.default_logger.debug("result_queue empty.")
+            pass
+        self.paused = False
 
     def _setupLogger(self):
         # create the logger to use.
         logger = logging.getLogger('PKDevTools.subprocess')
         # The only handler desired is the SubProcessLogHandler.  If any others
         # exist, remove them. In this case, on Unix and Linux the StreamHandler
         # will be inherited.
@@ -196,20 +215,20 @@
                     self.default_logger.debug(e, exc_info=True)
                     sys.exit(0)
                 if next_task is None:
                     self.default_logger.info("No next task in queue")
                     if self.task_queue is not None:
                         self.task_queue.task_done()
                     break
-                if self.processorMethod is not None:
+                if self.processorMethod is not None and not self.paused:
                     answer = self.processorMethod(*(next_task))
                 if self.task_queue is not None:
                     self.task_queue.task_done()
                 # self.default_logger.info(f"Task done. Result:{answer}")
-                if self.result_queue is not None:
+                if self.result_queue is not None and not self.paused:
                     self.result_queue.put(answer)
         except Exception as e:
             self.default_logger.debug(e, exc_info=True)
             sys.exit(0)
 
     def multiprocessingForWindows(self):
         if sys.platform.startswith("win"):
```

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240517.120/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240517.120/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240517.119
+Version: 0.13.20240517.120
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240517.119.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240517.120.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240517.119/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240517.120/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/PKG-INFO` & `PKDevTools-0.13.20240517.120/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240517.119
+Version: 0.13.20240517.120
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240517.119.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240517.120.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240517.119/README.md` & `PKDevTools-0.13.20240517.120/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240517.119/setup.py` & `PKDevTools-0.13.20240517.120/setup.py`

 * *Files identical despite different names*


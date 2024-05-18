# Comparing `tmp/logtools_vrb-0.0.1.tar.gz` & `tmp/logtools_vrb-0.8.0.tar.gz`

## Comparing `logtools_vrb-0.0.1.tar` & `logtools_vrb-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/src/logtools_vrb/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/src/logtools_vrb/__version__.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/src/logtools_vrb/formatting.py
--rw-r--r--   0        0        0    14655 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/src/logtools_vrb/logtools.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/src/logtools_vrb/mailloghandler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/src/logtools_vrb/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/LICENSE
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/README.md
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 logtools_vrb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/src/logtools_vrb/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/src/logtools_vrb/__version__.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/src/logtools_vrb/formatting.py
+-rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/src/logtools_vrb/logtools.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/src/logtools_vrb/mailloghandler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/src/logtools_vrb/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/LICENSE
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 logtools_vrb-0.8.0/PKG-INFO
```

### Comparing `logtools_vrb-0.0.1/src/logtools_vrb/formatting.py` & `logtools_vrb-0.8.0/src/logtools_vrb/formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         Args:
             level (int): log level (logging.INFO, logging.DEBUG etc.)
         """
         # remove Formatter object from _formatters[level]. 
         if level in self._formatters:
             self._formatters.pop(level)
 
-    def use_with(self, handler: Handler, *,
+    def apply_to(self, handler: Handler, *,
                  logger: Logger|None = None) -> LevelAwareFormatter:
         """ Sets self as the formatter for the given handler.
         If a logger is given as well, the handler is added to the logger.
 
         Args:
             handler (Handler): handler for which to set the formatter.
             logger (Logger, optional): logger to which the handler shall be added. Defaults to None.
@@ -118,12 +118,7 @@
         none, use the default formatter by calling super().format().
 
         For more details see Formatter.format() """
         if record.levelno in self._formatters:
             return self._formatters[record.levelno].format(record)
         else:
             return super().format(record)
-
-# SAMPLE USAGE
-if True:
-
-
```

### Comparing `logtools_vrb-0.0.1/src/logtools_vrb/logtools.py` & `logtools_vrb-0.8.0/src/logtools_vrb/logtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-"""
-# logtools_vrb
-
-Logging tools.
-
-```class CallerRecord:```
-
-Information regarding current position in program
-
-```class ExcInfo```
-
-Enhanced handling of exception information in logging etc.
-
-```class LogUtils```
-
-Misc Utils concerning logging and exceptions
-
-```class LevelFormatter(Formatter)```
-Formatter for use with the logging module supporting
-different format strings depending on the log level.
-"""
 from __future__ import annotations
 
 from datetime import datetime
 import typing
 if typing.TYPE_CHECKING:
     from logging import _SysExcInfoType, _ArgsType
 
@@ -81,22 +60,23 @@
         self.linenum: int = -1
         self.codeline: str = ""
         self.context: str = ""
         self.comment: str = comment
         self.verbosity = verbosity
 
         if isinstance(exc_info, BaseException):
-            # then we only have an exception object, but no line number, no traceback
+            # then we only have an exception object
             self.exc = exc_info
+            # get traceback from exception:
             self.tb = self.exc.__traceback__
         elif isinstance(exc_info, tuple) and (len(exc_info) > 1):
-            # then we have an exception object
+            # then we have an exception object ...
             self.exc = exc_info[1]
             if self.exc is not None:
-                # and probably traceback and line number information
+                # ... plus probably traceback information
                 self.tb = exc_info[2] if len(exc_info) > 2 else None
         if self.tb is not None:
             self.linenum = self.tb.tb_lineno
             stack = traceback.extract_tb(self.tb, 1)
             self.filename = stack[0].filename
             self.context = stack[0].name
             self.codeline = stack[0].line if stack[0].line else ""
@@ -184,23 +164,14 @@
 
     def __str__(self) -> str:
         return self.to_str()         
            
 class LogUtils:
     """ Misc Utils concerning logging and exceptions """
 
-    #####################
-    # PUBLIC
-    #####################    
-
-    PROGRAM_NAME: str = program_name
-    """ Name of running program (basename version without full path) """
-    PROGRAM_PID: int = program_pid
-    """ process id of currently running program """
-
     @classmethod
     def now(cls, datefmt: str="%Y-%m-%d %H:%M:%S") -> str:
         return datetime.now().strftime(datefmt)
     
     @classmethod
     def clear_log_handlers(cls, logger: Logger|None = None) -> Logger:
         """ Remove all log handlers from the given logger.
@@ -217,40 +188,41 @@
         for h in logger.handlers:
             logger.removeHandler(h)
         return logger
 
     
     @classmethod
     def make_log_record(cls, level: int = logging.NOTSET, 
-                        msg: str = "", *args: object, 
+                        msg: str = "", *args: object,
                         logger: Logger|None = None, 
                         exc_info: BaseException|_SysExcInfoType|bool = False, 
                         extra: Mapping[str, object]|None = None, 
                         stack_info: bool = False,
                         stacklevel: int = 1) -> LogRecord:
         """ Make log record from the given information. The record can either
         be used directly or information can be extracted using the get...(, LogRecord)
         class methods.
 
         Args:
             level (int): logging level (INFO, DEBUG, ...)
             msg (str): log message
+            args: Used together with msg to create the message field of the record (using msg % args)
             logger (Logger, optional): logger to use. Defaults to None (means root logger).
             exc_info (BaseException|_SysExcInfoType|bool, optional): include given exception info 
                 (if exc_info is of type BaseException or _SysExcInfoType) or get it 
                 from sys.exc_info() (if exc_info == True). Defaults to False.
             extra (Mapping[str, object], optional): additional key-value pairs for the record's __dict__. Defaults to None.
             stack_info (bool, optional): include stack_info?. Defaults to False.
             stacklevel (int, optional): stack level to use. Defaults to 1.
 
         Returns:
             LogRecord: Record containing information about the current position
             in the program's run, inluding stack and exception information, if wanted
         """
-        return cls._make_log_record(level, msg, args, 
+        return cls._make_log_record(level, msg, *args, 
                                     logger=logger, 
                                     exc_info=exc_info, 
                                     extra=extra, 
                                     stack_info=stack_info, 
                                     stacklevel=stacklevel)
 
     @classmethod
@@ -298,20 +270,16 @@
             stacklevel (int, optional): stack level to use. Defaults to 1.
 
         Returns:
             CallerRecord: position information
         """
         return cls._find_caller(stack_info, stacklevel)
 
-    #####################
-    # PRIVATE
-    #####################    
-    
     @classmethod
-    def _make_log_record(cls, level: int, msg: object, args: _ArgsType, 
+    def _make_log_record(cls, level: int, msg: object, *args: object,
                          logger: Logger|None = None, 
                          exc_info: BaseException|_SysExcInfoType|bool = False, 
                          extra: Mapping[str, object]|None = None, 
                          stack_info: bool = False,
                          stacklevel: int = 1):
         """
         Construct LogRecord. The implementaion is taken from logging._log.
```

### Comparing `logtools_vrb-0.0.1/src/logtools_vrb/mailloghandler.py` & `logtools_vrb-0.8.0/src/logtools_vrb/mailloghandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-"""
-## logtools_vrb.mailloghandler
-
-```class MailLogHandler```
-
-Log handler which mails log messages to a given recipient.
-"""
-
 from __future__ import annotations
-import logging, os, ssl, sys, socket
+import logging, ssl, socket
 
 from mailtools_vrb import EasySSLSendmail
-from logtools_vrb import program_name
-from logtools_vrb.logtools import ExcInfo
+from logtools_vrb import program_name, ExcInfo
 
 from typing import TYPE_CHECKING 
 if TYPE_CHECKING: 
     from _typeshed import FileDescriptorOrPath as FileDescriptorOrPath
 
 # get fqdn and hostname of localhost
 _fqdn = socket.getfqdn()
@@ -31,15 +22,16 @@
     if logging has been disabled by calling logging.disable(), since the default 
     argument to logging.disable() is CRITICAL and LOG_ALWAYS is CRITICAL+1.
     Can be disabled by calling logging.disable(MailLogHandler.LOG_ALWAYS) """
 
     DEFLT_SUB_START_FMT: str = '[%(fqdn)s] %(program)s: '
     """ Default format string for start portion of the mail subject """
 
-    def __init__(self, mail_to: str, json_mail_info: dict|FileDescriptorOrPath|None = None,
+    def __init__(self, mail_to: str, *,
+                 json_mail_info: dict|FileDescriptorOrPath|None = None,
                  host: str|None = None, port: int|None = None, 
                  ssl_context: ssl.SSLContext|None = None,
                  user: str|None = None, password: str|None = None, 
                  sender: str|None = None, minpause: int|None = None,
                  level: int|str = logging.NOTSET,
                  sub_start_fmt: str = DEFLT_SUB_START_FMT,
                  add_log_always_level: int = True) -> None:
```

### Comparing `logtools_vrb-0.0.1/LICENSE` & `logtools_vrb-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logtools_vrb-0.0.1/README.md` & `logtools_vrb-0.8.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 # logtools_vrb
 
 Logging tools.
 
+  - On PyPI: https://pypi.org/project/logtools-vrb/
+  - On GitHub: https://github.com/v-r-b/logtools_vrb 
+
+## \_\_init__.py
+
+```program_name, program_pid```
+
+Name and process ID of currently running program
+
+## logtools.py
+
 ```class CallerRecord:```
 
 Information regarding current position in program
 
 ```class ExcInfo```
 
 Enhanced handling of exception information in logging etc.
 
 ```class LogUtils```
 
 Misc Utils concerning logging and exceptions
 
-```class LevelFormatter(Formatter)```
+## formatting.py
+
+```class LevelAwareFormatter```
+
 Formatter for use with the logging module supporting
 different format strings depending on the log level.
 
-## logtools_vrb.mailloghandler
+## mailloghandler.py
 
 ```class MailLogHandler```
 
 Log handler which mails log messages to a given recipient.
```

